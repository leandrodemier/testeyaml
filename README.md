#Teste proposto de Ansible com códigos yml

Desafios:

1.1 - Efetuar a alteração de IP, máscara de sub rede e gateway em servidores Linux e Windows
 *_Código no arquivo AlterIPSubMaskGTW-Win-Lnx.yml_*

1.2 - Instalar zabbix-agent. 
 - Preencher o parâmetro “Server” com diferentes valores no arquivo de configuração, baseado no terceiro octeto do IP, onde está sendo instalado zabbix-agent.
 *_Código no arquivo InstallZabbixAgent.yml_*
 
2 - A resposta para o erro reportado é que se usou o winRM para conectar em Linux, quando deveria ser SSH. Por padrão o Ansible utiliza SSH para se conectar aos hosts, em máquinas Windows é necessário definir que a comunicação será por winRM, do contrário, caso não haja o SSH habilitado, não haverá comunicação.
