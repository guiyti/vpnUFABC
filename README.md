# vpnUFABC

O **vpnUFABC** é um aplicativo que automatiza a conexão à VPN da UFABC no macOS, utilizando o OpenConnect, uma alternativa de código aberto ao cliente oficial AnyConnect.

## Descrição

O aplicativo `vpnUFABC.app` simplifica o processo de conexão à VPN da UFABC no macOS. Para acessar a VPN é necessário ter dois componentes essenciais: o **OpenConnect**, que é a ferramenta utilizada para a conexão, e o **Homebrew**, que é o gerenciador de pacotes responsável pela instalação e execução do OpenConnect.

O aplicativo `vpnUFABC` realiza automaticamente a verificação da presença do Homebrew e do OpenConnect no sistema. Caso algum desses componentes não esteja instalado, o pacote cuida da instalação de forma prática e eficiente, permitindo que o usuário se conecte à VPN sem complicações adicionais.

## Por que usar Homebrew e OpenConnect?

A **UFABC** utiliza o protocolo **AnyConnect** da **Cisco** para conexões VPN, mas o cliente oficial pode não estar disponível ou ser complicado de instalar em alguns sistemas. O **OpenConnect** é uma solução compatível com o protocolo AnyConnect, garantindo a conexão VPN à universidade sem problemas.

O **Homebrew** é um gerenciador de pacotes que facilita a instalação e atualização de softwares no macOS, como o OpenConnect.

## Requisitos

- macOS 10.13 (High Sierra) ou posterior
- `osascript` (geralmente já incluído no macOS)
- Acesso à internet para baixar o Homebrew e o OpenConnect

## Uso

1. **Baixar o Repositório:**
   - Faça o download do repositório como um arquivo ZIP em **Code > Download ZIP**.

2. **Instalar o Aplicativo:**
   - Descompacte o arquivo ZIP.
   - Arraste o `vpnUFABC.app` para a pasta Aplicativos.

3. **Executar o Aplicativo:**
   - Dê um duplo clique no `vpnUFABC.app` para iniciar o aplicativo.
   - Se uma janela de segurança informar que o aplicativo foi baixado da internet e que o macOS não pode verificá-lo, abra **Ajustes > Segurança e Privacidade** e clique em **Abrir Mesmo Assim** para permitir a execução. Para mais detalhes, consulte [este link](https://macmagazine.com.br/post/2021/09/20/como-instalar-apps-de-desenvolvedores-nao-identificados-no-mac/), ou então visualize a sequência de imagens da pasta `readme_imgs`.

4. **Seguir as Instruções:**
   - O aplicativo solicitará sua senha de administrador para garantir as permissões necessárias para a instalação, configuração e execução.
   - Em seguida, insira suas credenciais da VPN conforme solicitado.

## Funcionalidades

- Instala automaticamente o Homebrew, se não estiver presente.
- Instala automaticamente o OpenConnect, se não estiver presente.
- Conecta à VPN utilizando as credenciais fornecidas pelo usuário.

## Recomendações

Caso você encontre problemas durante a instalação do Homebrew, recomenda-se visitar o [site oficial do Homebrew](https://brew.sh/) para obter mais informações. Se você não tiver familiaridade com a linha de comando, pode optar por executar o instalador automático mais recente. Para isso, basta procurar pelo arquivo `.pkg` mais recente no [repositório de lançamentos](https://github.com/Homebrew/brew/releases/latest), como, por exemplo, `Homebrew-4.3.7.pkg`, que pode facilitar a instalação manual.

Além disso, se houver problemas relacionados à necessidade do Command Line Tools, você pode instalar o Xcode Command Line Tools executando o comando `xcode-select --install` no Terminal. Isso pode ajudar a resolver qualquer questão relacionada à instalação do Homebrew.

## Para usuários avançados

Se você preferir trabalhar diretamente com o script, o código-fonte está disponível no arquivo `vpnUFABC.sh`. No entanto, a execução do aplicativo é recomendada para uma experiência simplificada.

## Autor

O **vpnUFABC** foi desenvolvido por Giulio Suzumura. Este projeto tem como objetivo facilitar o acesso à VPN da UFABC, proporcionando uma solução simples e prática para usuários do macOS.


## Licença

Este projeto é um software de código aberto, licenciado sob a [MIT License](https://opensource.org/licenses/MIT).

**Uso Indevido:** Este software não deve ser utilizado para fins ilegais ou prejudiciais. O autor não se responsabiliza por quaisquer consequências decorrentes do uso do software para tais propósitos.