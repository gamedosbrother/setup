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

### Testar

Para testar, tente clonar esse projeto:  
`$ git clone git@github.com:gamedosbrother/setup.git`  
Entre no diretório do projeto:  
`$ cd setup`  

Crie um arquivo com seu nome e uma mensagem legal e divertida!  
Após isso, verifique se o git identificou o seu arquivo:  
`$ git status`  

Esse comando irá exibir todos os arquivos modificados/criados.  
Caso seu arquivo esteja lá, adicione ele nos arquivos a serem commitados:  
`$ git add meunome.txt`  

Agora commite o arquivo para salvar as alterações no versionamento:  
`$ git commit -m "Testing my git!"`  

Tente pushar para o remoto (github), salvando essas alterações na núvem:  
`$ git push origin master`  

Esperamos que tudo de certo. Caso contrário, google it!  

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

Para usar o VSCode com o Unity, tu precisa instalar algumas extensões:
_`ctrl+shift+x` para abrir o menu de extensões_

#### Omnisharp
Extension do VSCode que funciona para conseguir ler o projeto C#. MUST HAVE se for usar o VSCode para unity.  
No VSCode, procurar por **C# (powered by Omnisharp)**  
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

#### Outros

É interessante instalar um Theme diferente, já que o do VSCode é meio blé.  
Eu sugiro o **Cobalt Next**, que é o que eu uso.  
Após instalar, aperte `ctrl+p` e digite `>Color theme`  
Vai abrir uma lista de todos os seus temas, selecione o **Cobalt Next** ou qualquer outro que tu instalou.  

Apertando `ctrl+,` tu abre as configurações do VSCode.  
Altere as configurações de acordo com o que tu ache melhor.  
O que eu sugiro:
* Tab size: 4
* Minimap Enabled: false