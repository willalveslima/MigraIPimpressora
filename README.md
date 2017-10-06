# MigraImpressorasIP.ps1
Script PowerShell para alterações de IPs de impressoras em Estações.

.Synopsis
  Script Para Migração de endereços de IPs de impressoras em VLANs de Rede XXXX em Migração 

 .Description
  O Script lista as portas TCP/IP das impressoras instaladas na estação Windows 7, identifica os endereços que devem ser alterados.
  Exclui as instãncias de impressoras que terão os Endereço alterados e cria clones das impressoras com o endereço IP já migrado. 
  
  !!!!!!!!!!!!!
  !! Atenção !!
  !!!!!!!!!!!!!
  
  O Script está configurado para alterar somente o Terceiro octeto do endereço IP da Impressora, O FINAL DO ENDEREÇO IP SERÁ MANTIDO !
  Exemplo:
  
  192.168.240.222 -> 192.168.236.222 
  
  O ultimo octeto deve possuir 3 digitos (x.x.x.123)
     
  
 .Example
   .\MigraImpressorasIP.ps1
   
 .Link
  --------------

 .Notes
  v1.0 - 10/02/2016 
