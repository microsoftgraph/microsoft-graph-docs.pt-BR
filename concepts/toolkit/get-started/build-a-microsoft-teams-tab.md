---
title: Criar uma guia do Microsoft Teams com o kit de ferramentas do Microsoft Graph
description: Introdução à criação de uma guia do Microsoft Teams usando o kit de ferramentas do Microsoft Graph.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: c4ed3396d05c865fd483bc8b007cdc743c0e8419
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2020
ms.locfileid: "48288536"
---
# <a name="build-a-microsoft-teams-tab-with-the-microsoft-graph-toolkit"></a>Criar uma guia do Microsoft Teams com o kit de ferramentas do Microsoft Graph

Este tópico aborda como começar a usar o Microsoft Graph Toolkit em uma solução do Microsoft Teams. Introdução envolve as seguintes etapas:

1. Criar um novo aplicativo do teams com uma guia personalizada.
2. Configure o ngrok e crie um túnel.
3. Adicione o Microsoft Graph Toolkit.
4. Inicialize o provedor do Microsoft Teams.
5. Crie a página pop-up de autenticação.
6. Adicionar componentes.
7. Teste seu aplicativo.

## <a name="create-a-new-teams-application-with-a-custom-tab"></a>Criar um novo aplicativo do teams com uma guia personalizada

A maneira mais fácil de criar um novo aplicativo do teams é usar a [extensão do Microsoft Teams Toolkit](https://marketplace.visualstudio.com/items?itemName=TeamsDevApp.ms-teams-vscode-extension) para o Visual Studio Code. Siga as instruções para [configurar um novo projeto do teams](/microsoftteams/platform/toolkit/visual-studio-code-overview#set-up-a-new-teams-project). Quando você chegar à tela **Adicionar recursos** , selecione **Tab**e, em seguida, **guia pessoal**.

## <a name="set-up-ngrok-and-create-a-tunnel"></a>Configurar o ngrok e criar um túnel

Para testar seu aplicativo mais tarde, você precisará hospedar seu aplicativo por meio de uma URL voltada para o público usando HTTPS. Instale o [ngrok](https://ngrok.com/download) e crie um túnel da Internet para localhost: 3000 com o seguinte comando:

```bash
ngrok http 3000
```
No diretório do projeto, localize o `.publish\Development.env` arquivo e substitua o valor por pela `baseUrl0` URL do ngrok.

## <a name="add-the-microsoft-graph-toolkit"></a>Adicionar o Microsoft Graph Toolkit

Você pode usar o Microsoft Graph Toolkit em seu aplicativo referenciando o carregador diretamente (via unpkg) ou instalando o pacote NPM. Para usar o kit de ferramentas, você também precisará do [Microsoft Teams SDK](/javascript/api/overview/msteams-client?view=msteams-client-js-latest).

### <a name="use-via-mgt-loader"></a>Usar via gerenciamento-carregador
Para usar o kit de ferramentas e o SDK do teams por meio dos carregadores, adicione as seguintes referências a `public/index.html` :

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```

### <a name="use-via-npm-es6-modules"></a>Usar via NPM (módulos ES6)
O uso do kit de ferramentas por meio de módulos ES6 fornecerá controle total do processo de agrupamento e permitirá que você reúna apenas o código necessário para o aplicativo. Para usar os módulos do ES6, adicione os pacotes do NPM para o kit de ferramentas e o SDK do Microsoft Teams ao seu projeto:

```bash
npm install @microsoft/mgt @microsoft/teams-js
```

## <a name="initialize-the-teams-provider"></a>Inicializar o provedor de equipes

Os provedores do Microsoft Graph Toolkit permitem a autenticação e o acesso ao Microsoft Graph para os componentes. Para saber mais, consulte [usando os provedores](../providers.md). O [provedor de equipes](../providers/teams.md) lida com toda a lógica e as interações que precisam ser implementadas com o SDK do teams para autenticar o usuário.

Você pode optar por inicializar o provedor em seu código HTML ou JavaScript. 

### <a name="initialize-in-html"></a>Inicializar em HTML

No `public/index.html` , adicione o provedor de equipes como mostrado.

```html
<mgt-teams-provider
  client-id="<YOUR_CLIENT_ID>"
  auth-popup-url="https://<YOUR_NGROK_URL>/auth.html"
></mgt-teams-provider>
```

Substitua `<YOUR_CLIENT_ID>` pela ID do cliente para seu aplicativo e `<YOUR_NGROK_URL>` com a URL do ngrok que você criou.

### <a name="initialize-in-javascript"></a>Inicializar em JavaScript

Para inicializar o provedor no seu código JavaScript, localize o `src/components/App.js` arquivo no diretório do projeto. Importe o provedor de equipes e inicialize o provedor.

```js
import * as microsoftTeams from "@microsoft/teams-js/dist/MicrosoftTeams";
import { Providers, TeamsProvider } from '@microsoft/mgt';

TeamsProvider.microsoftTeamsLib = microsoftTeams;
Providers.globalProvider = new TeamsProvider ({
    clientId: '<YOUR_CLIENT_ID>',
    authPopupUrl: '/auth.html'
})
```
Substitua `<YOUR_CLIENT_ID>` pela ID do cliente para seu aplicativo.

### <a name="creating-an-appclient-id"></a>Criar uma ID de aplicativo/cliente
Para obter uma ID de cliente, você precisa [registrar seu aplicativo](../../auth-register-app-v2.md) no Azure AD. Certifique-se de adicionar a URL do ngrok com o caminho completo para a página pop-up de autenticação em seus URIs de redirecionamento (por exemplo, `https://<YOUR_NGROK_URL>/auth.html` ).
>**Observação**: o MSAL só dá suporte ao fluxo implícito do OAuth. Certifique-se de habilitar o fluxo implícito em seu aplicativo no portal do Azure (não está habilitado por padrão). Em **autenticação**, encontre a seção **concessão implícita** e marque as caixas de seleção para **tokens de acesso** e **tokens de ID**. 

## <a name="create-the-auth-popup-page"></a>Criar a página pop-up de autenticação

Para permitir que os usuários entrem, você precisa fornecer uma URL que o aplicativo Teams abrirá em um pop-up para acompanhar o fluxo de autenticação. A URL precisa estar em seu domínio, e toda esta página precisa ser chamada para o `TeamsProvider.handleAuth()` método.

Você pode fazer isso no HTML adicionando um novo `auth.html` arquivo na `public` pasta (que deve estar no mesmo nível que `index.html` ) e adicionando o seguinte código: 

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<script>
  mgt.TeamsProvider.handleAuth();
</script>
```

## <a name="add-components"></a>Adicionar componentes

Agora, você está pronto para adicionar qualquer um dos componentes do Microsoft Graph Toolkit à sua guia. 

Você pode adicionar componentes ao HTML normalmente. Por exemplo, para adicionar o componente de login, adicione o código a seguir ao corpo de `index.html` :

```html
<mgt-login></mgt-login>
```

Ou, você pode adicionar os componentes no JSX ao componente guia. Recomendamos usar a `mgt-react` biblioteca se você tiver criado o aplicativo Teams usando a extensão do kit de ferramentas do Microsoft Teams. Para saber mais, consulte [usando o Microsoft Graph Toolkit com reagir](./use-toolkit-with-react.md#using-mgt-react)

Primeiro, instale o `mgt-react` :

```bash
npm install @microsoft/mgt-react
```

Localize o `src/components/Tab.js` arquivo e importe os componentes que você deseja usar da `mgt-react` biblioteca. Por exemplo, para adicionar o `Login` uso do componente:

```js
import { Login } from "@microsoft/mgt-react"
```

Em seguida, adicione o componente à `return()` instrução do `render()` método de `Tab` :

```jsx
render() {
  return(
    <Login />
  );
}
```

## <a name="test-your-application"></a>Testar seu aplicativo

Crie e execute o aplicativo usando os seguintes comandos:
```bash
npm install
npm start
```

Para testar seu aplicativo, você precisa carregar seu aplicativo para o Microsoft Teams. Abra o cliente Microsoft Teams, selecione o **...** no menu à esquerda e vá para o **app Studio**. Clique na guia **Editor de manifesto** e selecione **importar um aplicativo existente**.

Localize o diretório do projeto e carregue o arquivo **Development.zip** dentro da pasta **. publish** .

Depois que o aplicativo for carregado, role para baixo no menu à esquerda e selecione **testar e distribuir**. Clique no botão **instalar** e, em seguida, clique em **Adicionar**. Você será redirecionado para a guia criada.

## <a name="next-steps"></a>Próximas etapas
- Confira este tutorial passo a passo sobre [a criação de uma guia do teams](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-10-microsoft-graph-toolkit-teams-provider/).
- Experimente os componentes no [playground](https://mgt.dev).
- Faça uma pergunta sobre o [estouro de pilha](https://aka.ms/mgt-question).
- Informe bugs ou deixe uma solicitação de recurso no [GitHub](https://aka.ms/mgt).