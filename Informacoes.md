# Informações #

## Chaves de configuração ##
Esse projeto tem duas chaves externas, uma delas liga ou desliga a memória de 512KiB. Se desligar, você fica somente com a interface SD, podendo ligar em slots expandidos ou não. Se ligar a memória, você usa a outra chave para escolher entre megaram ou mapper.

Se ligar a memória você liga o expansor interno (para poder ter dois dispositivos ao mesmo tempo), mas só poderá usar em slots não-expandidos.

## Clock próprio ##
No hardware há um cristal oscilador de 25MHz, fazendo a interface ser assíncrona e independente do clock do barramento.

## Memória SRAM e Flash ##
Na lista de componentes, a flash indicada é a `AM29F010`, porém o projeto e o atualizador suporta outros tipos de flash, desde que seja invólucro PLCC:

  * `AT49F002(T)`;
  * `AT49(H)F010`;
  * `SST39SF020`;
  * `W49F002U/N`;
  * `W49F002B`;
  * `W39F010`.

A memória SRAM pode ser substituída pela `AS6C4008`.

## Sistema Operacional ##
O sistema operacional é o Nextor, na sua última versão estável. A flash interna pode ser atualizada pelo próprio MSX. Para isso você precisa de outra interface de armazenamento em massa (floppy, ide, etc) e usar o atualizador `sdmupd.com`.

## Cartões SD ##
Há duas entradas para cartão SD. Suporta cartões SD ou SDHC e foi testado com cartões de 128MB até 8GB. O Nextor tem a mesma regra do DOS2, se tiver 128K de mapper dá para usar sub-diretórios e FAT16 nativo, assim você pode ter até 4 partições em cada cartão, e cada partição pode ter até 4GB.

## Etiquetas ##
Há um desenho de uma etiqueta para impressão colorida em papel fotográfico auto-colante para fazer um acabamento em caixas Patola. Essa etiqueta está em PDF na versão com uma etiqueta e outra versão com seis etiquetas, para aproveitar o papel. Há a etiqueta frontal e a superior e está em alta qualidade.