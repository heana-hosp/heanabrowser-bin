# heanabrowser-bin
# Navegador desenvolvido para suporte aos Sistemas MV - Suportar o Flashão Véio. 

Observações Importantes: Para o funcionamento do utilitário las(utilitário MV - mvupdate) é necessário a instalação do Oracle Java. A versão OpenJDK/JRE não funciona devido a ausência do utilitário(bin) que permite a instalação de aplicativo Install4J. Instalando a versão da Oracle, funcionará/executará independente do sistema operacional.


Windows 
:link: [Download Instalador](https://github.com/heana-hosp/heanabrowser-bin/releases/download/HEANA/HEANABrowser-win32-x64.zip) (316 MB) 

Linux (tested on Ubuntu/Debian)
:link: [Download Instalador](https://github.com/heana-hosp/heanabrowser-bin/releases/download/HEANA/HEANABrowser-linux-x64.zip) (160 MB) 

MacOS(darwin) - Fase de teste

- Consideração importante sobre a versão Linux: Ao descompactar a pasta, necessário atribuir à estrutura de pasta(chown) a mesma permissão do usuário comum(readme.txt/leiame.txt dentro do arquivo compactado - recomenda-se instalar na pasta padrão home). Não use como root. No linux há um mecanismo de proteção que não permite executar a sandbox do chrome(engine a qual o electron é baseado), protegendo a nível de SUID/GUID, evitando que o navegador execute arquivos que não tem permissão e também não renderize as páginas web. Essas tratativas de permissões são necessárias nos pacotes deb/rpm por instalar na estrutura do do sistema operacional como root, porém, não é o caso destes arquivos neste repositório. 


# Outras considerações:

- No Windows 11 costuma aparece a mensagem do Smarth Screen criticando "Fornecedor desconhecido" e pode ser ignorado pela primeira vez. Necessário certificados e etc, que não é o nosso caso e necessidade. 

- Versões deb/rpm/dmg apenas no repositório privado. Requer várias validações, portanto, não disponíveis no repositório aberto. 

- Sabe-se que a emissão de relatório no Gestor de Fluxo não funciona - Devido a invocação de um método defasado win.getWebContents(deprecated no electron) mas não impossível de implementar. Não temos urgência ou necessidade de inserir essa função no momento, talvez em necessidades futuras. 