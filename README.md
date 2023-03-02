# Apache24

An Apache 2.4 configured to microsoft Windows.

 1. descompacte o diretório do apache e do php em alguma pasta como no C:\ (ficará C:\Apache24\ e C:\php) .
 2. edite o arquivo $diretorio_criado$\conf\httpd.conf e na linha 39 (ou linha que tenha a diretiva Define SRVROOT) aponte para o endereço criado (ex: Define SRVROOT = "c:/Apache24") 
 3. No arquivo $diretorio_criado$\conf\httpd.conf aponte os endereços do php para o caminho do php criado no passo 1. (ex. LoadFile "c:\php\libpq.dll; LoadModulo php7_module "c:\php7apache2_4.dll"; PHPIniDir "c:\php") 
 5. Pela linha de comando do windows (cmd) vá na pasta bin diretório criado. (cd \apache24\bin)
 6. Adiciona o apache como serviço digitado o comando httpd -k install. O windows pedirá permissão para utilizar o serviço. Permita em todas as redes.
 7. No browser escreve http://localhost:80, o resultado deve ser It Works!
 8. Caso necessite parar ou reiniciar o serviço, vá aos serviços do windows (digite services na barra de busca) e selecione o serviço Apache2.4. 


alisoncf@gmail.com
