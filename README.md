# Setup

## Git

### Baixar e Instalar

**Windows**  
https://git-scm.com/download/win

_Instalar o gitbash, ajuda muito no desenvolvimento no windows ter um bash decente_

**Mac**  
https://git-scm.com/download/mac

### Criar conta no github

https://github.com/join?source=header-home

### Gerar uma SSH Key

Para conseguirmos usar o repositório remoto (Github), precisamos criar uma SSH Key

https://help.github.com/en/enterprise/2.16/user/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent

## Unity

### Unity HUB

Para facilitar o controle das versões do Unity, iremos usar o Unity HUB.

https://store.unity.com/download?ref=personal&_ga=2.110824589.920793428.1552409301-2076064889.1511476959

### Versões

No Unity HUB, baixar a versão do Unity 2018.3.
Selecione para qual sistema vc quer poder buildar. Sugiro:
* Windows/Mac
* WebGL

## Optionals

### VS Code

Normalmente, o Unity instala o Visual Studio para programar.
Eu não curto muito, é muito pesado e, para programar coisas fora de C#/Java, não curto muito IDEs.

Eu uso o VSCode. Um editor de texto muito bom para programar e funciona muito bem com Unity.

**Baixar**
https://code.visualstudio.com/

Após isso, vai ser necessário configurar o Unity para usar o VSCode:
![Configurar VSCode no Unity](https://raw.githubusercontent.com/gamedosbrother/setup/master/config_unity_vscode.png)

* No Unity, entrar no Menu Edit/Preferences...
* Selecionar a aba External Tools
* Selecionar o Vistual Studio Code se estiver disponível
* Caso contrário, vai em Browse e procura o executavel
  * Normalmente, fica em C:\Users\USER\AppData\Local\Programs\Microsoft VS Code\Code.exe

Para usar o VSCode com o Unity, tu precisa instalar alguns pacotes:

#### Omnisharp
Extension do VSCode que funciona para conseguir ler o projeto C#. MUST HAVE se for usar o VSCode para unity.  
_No Mac, vai precisar instalar o Mono_

#### .NET 4.5

Também é necessario baixar o .net 4.5 para as versões mais novas do Unity.

Nesse link:
https://dotnet.microsoft.com/download/archives

Baixa o .NET Framework 4.5.2 e instala.  

Aqui vem uma pequena **gambiarra**.  
O VSCode não vai conseguir achar o .NET 4.5, pq tu baixou o 4.5.2.  
Para fazer funcionar você deve copiar a versão 4.5.2:  
`C:\Program Files (x86)\Reference Assemblies\Microsoft\Framework\.NETFramework\v4.5.2`  

Para a pasta:  
`C:\Program Files (x86)\Reference Assemblies\Microsoft\Framework\.NETFramework\v4.5.`  
Dessa forma, o VSCode vai conseguir achar.  

Infelizmente, nunca fiz essa parte no mac/linux, então não sei como funciona.