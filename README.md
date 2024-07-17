# vpnUFABC

O **vpnUFABC** é um aplicativo que automatiza a conexão à VPN da UFABC no macOS, utilizando o OpenConnect, uma alternativa de código aberto ao cliente oficial AnyConnect.

## Descrição

O aplicativo `vpnUFABC.app` simplifica o processo de conexão à VPN, gerenciando automaticamente a instalação do Homebrew e do OpenConnect, se necessário. Com uma interface amigável, ele solicita as credenciais do usuário e realiza a conexão de forma eficiente.

## Por que usar Homebrew e OpenConnect?

A **UFABC** utiliza o protocolo **AnyConnect** para conexões VPN, mas o cliente oficial pode não estar disponível ou ser complicado de instalar em alguns sistemas. O **OpenConnect** é uma solução compatível com o protocolo AnyConnect, garantindo que você possa se conectar à VPN da universidade sem problemas.

O **Homebrew** é um gerenciador de pacotes que facilita a instalação e atualização de softwares no macOS, como o OpenConnect.

## Requisitos

- macOS 10.13 (High Sierra) and later
- `osascript` (geralmente já incluído no macOS)
- Acesso à internet para baixar o Homebrew e o OpenConnect

## Uso

1. **Baixe o aplicativo:**
   - Faça o download de `vpnUFABC.app` do repositório.

2. **Execute o aplicativo:**
   - Dê um duplo clique no `vpnUFABC.app` para iniciar o processo.

3. **Siga as instruções:**
   - O aplicativo solicitará de administrador e depois as credenciais da VPN. Insira os dados corretamente para se conectar.

## Funcionalidades

- Instala automaticamente o Homebrew, se não estiver presente.
- Instala automaticamente o OpenConnect, se não estiver presente.
- Conecta à VPN utilizando as credenciais fornecidas pelo usuário.


## Recomendações

Caso você encontre problemas durante a instalação do Homebrew, recomenda-se visitar o [site oficial do Homebrew](https://brew.sh/) para obter mais informações. Caso você não tenha familiaridade com a linha de comando, pode optar por executar o instalador automático mais recente. Para isso, basta procurar pelo arquivo `.pkg` mais recente no [repositório de lançamentos](https://github.com/Homebrew/brew/releases/latest), como, por exemplo, `Homebrew-4.3.7.pkg`, que pode facilitar a instalação manual.

Além disso, se houver problemas relacionados à necessidade do Command Line Tools, você pode instalar o Xcode Command Line Tools executando o comando `xcode-select --install` no Terminal.

Isso pode ajudar a resolver qualquer questão relacionada à instalação do Homebrew.


## Para usuários avançados

Se você preferir trabalhar diretamente com o script, o código-fonte está disponível no arquivo `vpnUFABC.sh`. No entanto, a execução do aplicativo é recomendada para uma experiência simplificada.


## Autor

O **vpnUFABC** foi desenvolvido por [Seu Nome]. Este projeto tem como objetivo facilitar o acesso à VPN da UFABC, proporcionando uma solução simples e prática para usuários do macOS.

### Contato

Você pode entrar em contato comigo através do meu e-mail: [seuemail@exemplo.com] ou pelo meu perfil no GitHub: [seuusuario](https://github.com/seuusuario).

## Licença

Este projeto é um software de código aberto, licenciado sob a [MIT License](https://opensource.org/licenses/MIT).

**Uso Indevido:** Este software não deve ser utilizado para fins ilegais ou prejudiciais. O autor não se responsabiliza por quaisquer consequências decorrentes do uso do software para tais propósitos.