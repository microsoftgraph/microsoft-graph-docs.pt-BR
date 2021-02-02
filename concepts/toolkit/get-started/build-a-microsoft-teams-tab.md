---
title: Criar uma guia do Microsoft Teams com o Kit de Ferramentas do Microsoft Graph
description: Começar a criar uma guia do Microsoft Teams usando o Kit de Ferramentas do Microsoft Graph.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 96a820fa26697d360128b86ea8ba7cbd4d3c1cd8
ms.sourcegitcommit: 7dc8ca82a8b2c25c5084e6b3121688766c9c14a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/02/2021
ms.locfileid: "50072349"
---
# <a name="build-a-microsoft-teams-tab-with-the-microsoft-graph-toolkit"></a>Criar uma guia do Microsoft Teams com o Kit de Ferramentas do Microsoft Graph

Este tópico aborda como começar a usar o Microsoft Graph Toolkit em uma solução do Microsoft Teams. A iniciação envolve as seguintes etapas:

1. Crie um novo aplicativo teams com uma guia personalizada.
2. Configurar o ngrok e criar um túnel.
3. Adicione o Microsoft Graph Toolkit.
4. Inicialize o provedor do Microsoft Teams.
5. Crie a página pop-up de auth.
6. Adicione componentes.
7. Teste seu aplicativo.

## <a name="create-a-new-teams-application-with-a-custom-tab"></a>Criar um novo aplicativo teams com uma guia personalizada

A maneira mais fácil de criar um novo aplicativo teams é usar a extensão do Kit de [Ferramentas do Microsoft Teams](https://marketplace.visualstudio.com/items?itemName=TeamsDevApp.ms-teams-vscode-extension) para o Visual Studio Code. Siga as instruções para [configurar um novo projeto do Teams.](/microsoftteams/platform/toolkit/visual-studio-code-overview#set-up-a-new-teams-project) Quando você chegar à tela **Adicionar recursos,** selecione **Tab** e, em seguida, **a guia Pessoal.**

## <a name="set-up-ngrok-and-create-a-tunnel"></a>Configurar o ngrok e criar um túnel

Para testar seu aplicativo posteriormente, você precisará hospedar seu aplicativo em uma URL voltada para o público usando HTTPS. Instale [o ngrok](https://ngrok.com/download) e crie um túnel da Internet para o localhost:3000 com o seguinte comando:

```bash
ngrok http 3000
```
No diretório do projeto, localize `.publish\Development.env` o arquivo e substitua o valor pela URL do `baseUrl0` ngrok.

## <a name="add-the-microsoft-graph-toolkit"></a>Adicionar o Kit de Ferramentas do Microsoft Graph

Você pode usar o Microsoft Graph Toolkit em seu aplicativo fazendo referência ao carregador diretamente (via unpkg) ou instalando o pacote npm. Para usar o Kit de Ferramentas, você também precisará do [SDK](/javascript/api/overview/msteams-client?view=msteams-client-js-latest)do Microsoft Teams.

### <a name="use-via-mgt-loader"></a>Usar via mgt-loader
Para usar o Kit de Ferramentas e o SDK do Teams por meio dos carregadores, adicione as seguintes referências `public/index.html` a:

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```

### <a name="use-via-npm-es6-modules"></a>Usar via npm (módulos ES6)
Usar o Kit de Ferramentas por meio de módulos ES6 dará a você controle total do processo de empacotamento e permitirá agrupar apenas o código necessário para seu aplicativo. Para usar os módulos ES6, adicione os pacotes npm para o Kit de Ferramentas e o SDK do Microsoft Teams ao seu projeto:

```bash
npm install @microsoft/mgt @microsoft/teams-js
```

## <a name="initialize-the-teams-provider"></a>Inicializar o provedor do Teams

Os provedores do Microsoft Graph Toolkit permitem autenticação e acesso ao Microsoft Graph para os componentes. Para saber mais, consulte [Usando os provedores.](../providers/providers.md) O [provedor do Teams](../providers/teams.md) lida com toda a lógica e interações que precisam ser implementadas com o SDK do Teams para autenticar o usuário.

Você pode optar por inicializar o provedor no código HTML ou JavaScript. 

### <a name="initialize-in-html"></a>Inicializar em HTML

Em `public/index.html` , adicione o provedor do Teams conforme mostrado.

```html
<mgt-teams-provider
  client-id="<YOUR_CLIENT_ID>"
  auth-popup-url="https://<YOUR_NGROK_URL>/auth.html"
></mgt-teams-provider>
```

Substitua `<YOUR_CLIENT_ID>` pela ID do cliente para seu aplicativo e pela `<YOUR_NGROK_URL>` URL ngrok que você criou.

### <a name="initialize-in-javascript"></a>Inicializar em JavaScript

Para inicializar o provedor no código JavaScript, localize o `src/components/App.js` arquivo no diretório do projeto. Importe o Provedor do Teams e inicialize o provedor.

```js
import * as microsoftTeams from "@microsoft/teams-js/dist/MicrosoftTeams";
import { Providers, TeamsProvider } from '@microsoft/mgt';

TeamsProvider.microsoftTeamsLib = microsoftTeams;
Providers.globalProvider = new TeamsProvider ({
    clientId: '<YOUR_CLIENT_ID>',
    authPopupUrl: '/auth.html'
})
```
Substitua `<YOUR_CLIENT_ID>` pela ID do cliente do aplicativo.

### <a name="creating-an-appclient-id"></a>Criando uma ID de aplicativo/cliente
Para obter uma ID do cliente, você precisa registrar [seu aplicativo](../../auth-register-app-v2.md) no Azure AD. Certifique-se de adicionar sua URL ngrok com o caminho completo para a página pop-up de autenticação para seus URIs de redirecionamento (por exemplo, `https://<YOUR_NGROK_URL>/auth.html` ).
>**Observação:** A MSAL só dá suporte ao Fluxo Implícito para OAuth. Certifique-se de habilitar o Fluxo Implícito em seu aplicativo no Portal do Azure (ele não está habilitado por padrão). Em **Autenticação,** encontre a **seção concessão implícita** e marque as caixas de seleção para **tokens do Access** e **tokens de ID.** 

## <a name="create-the-auth-popup-page"></a>Criar a página pop-up de auth

Para permitir que os usuários se inscrevam, você precisa fornecer uma URL que o aplicativo teams abrirá em um pop-up para seguir o fluxo de autenticação. A URL precisa estar em seu domínio, e tudo o que essa página precisa fazer é chamar o `TeamsProvider.handleAuth()` método.

Você pode fazer isso em seu HTML adicionando um novo arquivo na pasta (que deve estar no mesmo nível que ) e adicionando `auth.html` `public` o seguinte `index.html` código: 

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<script>
  mgt.TeamsProvider.handleAuth();
</script>
```

## <a name="add-components"></a>Adicionar componentes

Agora você está pronto para adicionar qualquer um dos componentes do Microsoft Graph Toolkit à guia. 

Você pode adicionar componentes ao HTML como faria normalmente. Por exemplo, para adicionar o componente de logon, adicione o código a seguir ao corpo do `index.html` seu:

```html
<mgt-login></mgt-login>
```

Ou você pode adicionar os componentes no JSX ao componente Tab. Recomendamos usar a biblioteca se você tiver criado seu aplicativo Teams usando a extensão do Kit de `mgt-react` Ferramentas do Microsoft Teams. Para saber mais, confira [Como usar o Kit de Ferramentas do Microsoft Graph com o React](./use-toolkit-with-react.md)

Primeiro, `mgt-react` instale:

```bash
npm install @microsoft/mgt-react
```

Localize `src/components/Tab.js` o arquivo e importe os componentes que você deseja usar da `mgt-react` biblioteca. Por exemplo, para adicionar o `Login` uso do componente:

```js
import { Login } from "@microsoft/mgt-react"
```

Em seguida, adicione o componente à `return()` instrução do `render()` método `Tab` de:

```jsx
render() {
  return(
    <Login />
  );
}
```

## <a name="test-your-application"></a>Testar seu aplicativo

Crie e execute seu aplicativo usando os seguintes comandos:
```bash
npm install
npm start
```

Para testar seu aplicativo, você precisa carregar seu aplicativo para o Teams. Abra o cliente do Microsoft Teams, selecione **o...** no menu à esquerda e vá para **o App Studio.** Clique na **guia Editor de** Manifesto e selecione Importar um aplicativo **existente.**

Localize o diretório do projeto **e carregue oDevelopment.zip** arquivo dentro da pasta **.publish.**

Depois que seu aplicativo tiver carregado, role para baixo no menu à esquerda e selecione **Testar e Distribuir.** Clique no **botão Instalar** e clique em **Adicionar.** Você será redirecionado para a guia que você criou.

## <a name="next-steps"></a>Próximas Etapas
- Confira este tutorial passo a passo sobre como [criar uma guia do Teams.](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-10-microsoft-graph-toolkit-teams-provider/)
- Experimente os componentes no [playground.](https://mgt.dev)
- Faça uma pergunta no [Stack Overflow](https://aka.ms/mgt-question).
- Relatar bugs ou deixar uma solicitação de recurso [no GitHub.](https://aka.ms/mgt)
