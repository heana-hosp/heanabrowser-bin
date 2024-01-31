# heanabrowser-bin
# Navegador desenvolvido para suporte aos Sistemas MV / Projeto SES - Suportar o Flashão Véio. 

Observações Importantes: Para o funcionamento do utilitário las(utilitário MV - mvupdate) é necessário a instalação do Oracle Java. A versão OpenJDK/JRE não funciona devido a ausência do utilitário(bin) que permite a instalação de aplicativo Install4J. Instalando a versão da Oracle, funcionará/executará independente do sistema operacional.


Windows 
:link: [Download ZIP](https://github.com/heana-hosp/heanabrowser-bin/releases/download/HEANA/HEANABrowser-win32-x64.zip) (316 MB) 

Linux (tested on Ubuntu/Debian)
:link: [Download ZIP](https://github.com/heana-hosp/heanabrowser-bin/releases/download/HEANA/HEANABrowser-linux-x64.zip) (160 MB) 

MacOS(darwin) - Fase de teste



# Considerações Importantes:

- Consideração importante sobre a versão Linux: Ao descompactar a pasta, necessário atribuir à estrutura de pasta(chown) a mesma permissão do usuário comum(readme.txt/leiame.txt dentro do arquivo compactado - recomenda-se instalar na pasta padrão home). Não use como root. No linux há um mecanismo de proteção que não permite executar a sandbox do chrome(engine a qual o electron é baseado), protegendo a nível de SUID/GUID, evitando que o navegador execute arquivos que não tem permissão e também não renderize as páginas web. Essas tratativas de permissões são necessárias nos pacotes deb/rpm por instalar na estrutura do do sistema operacional como root, porém, não é o caso destes arquivos neste repositório. 

- No Windows 11 costuma aparece a mensagem do Smarth Screen criticando "Fornecedor desconhecido" e pode ser ignorado pela primeira vez. Necessário certificados e etc, que não é o nosso caso e necessidade. O problema ocorre quando o arquivo fica disponível para download(ativa flag), porém, no ambiente interno da unidade não ocorre o problema. 

- Versões deb/rpm/dmg apenas no repositório privado. Requer várias validações, portanto, não disponíveis no repositório aberto. 

- Sabe-se que a emissão de relatório no Gestor de Fluxo não funciona - Devido a invocação de um método defasado win.getWebContents(deprecated no electron) mas não impossível de implementar. Não temos urgência ou necessidade de inserir essa função no momento, talvez em necessidades futuras. 

- Versão MacOS validada no Sonoma. Não disponibilizaremos a versão MacOS(demonstrado no vídeo abaixo) pois requer adaptação do utilitário las(jars) para tratar o sistema operacional MacOS. O código pertence a MV, por isso não disponibilizaremos ou orientaremos sobre resolver esta situação

# Demonstração de Uso

Versão Debian  - Clique na Imagem para ver o Vídeo:

[![HEANA Browser Debian](https://github.com/heana-hosp/heanabrowser-bin/assets/5917784/e83bbe9f-ea74-4a01-b7d8-271826a60afe)](https://youtu.be/MT5WmscDlZU "HEANA Browser Debian")


Versão MacOS Sonoma - Clique na Imagem para ver o Vídeo:

[![HEANA Browser MacOS Sonoma](https://github.com/heana-hosp/heanabrowser-bin/assets/5917784/6f4a2ae2-0b2a-499c-9891-1640ea8d2fcd)](https://youtu.be/sa7r9XR_pgQ "HEANA Browser Mac OS Sonoma")


