---
title: Criar uma guia do Microsoft Teams com o Microsoft Graph Toolkit
description: Começar a criar uma guia do Microsoft Teams usando o microsoft graph Toolkit.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 757c7eb8a94b0f6936a21f5ecb6f126cde36b6ad
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721562"
---
# <a name="build-a-microsoft-teams-tab-with-the-microsoft-graph-toolkit"></a>Criar uma guia do Microsoft Teams com o Microsoft Graph Toolkit

Este tópico aborda como começar a usar o microsoft graph Toolkit em uma solução do Microsoft Teams. Começar envolve as seguintes etapas:

1. Crie um novo aplicativo do Teams com uma guia personalizada.
2. Configurar ngrok e criar um túnel.
3. Adicione o microsoft graph Toolkit.
4. Inicializar o provedor do Microsoft Teams.
5. Crie a página pop-up de auth.
6. Adicione componentes.
7. Teste seu aplicativo.

## <a name="create-a-new-teams-application-with-a-custom-tab"></a>Criar um novo aplicativo do Teams com uma guia personalizada

A maneira mais fácil de criar um novo aplicativo do Teams é usar a extensão Toolkit [Microsoft Teams](https://marketplace.visualstudio.com/items?itemName=TeamsDevApp.ms-teams-vscode-extension) para Visual Studio Code. Siga as instruções para [configurar um novo projeto do Teams.](/microsoftteams/platform/toolkit/visual-studio-code-overview#set-up-a-new-teams-project) Quando você chegar à tela **Adicionar recursos,** selecione **Guia** e, em seguida, **guia Pessoal.**

## <a name="set-up-ngrok-and-create-a-tunnel"></a>Configurar ngrok e criar um túnel

Para testar seu aplicativo posteriormente, você precisará hospedar seu aplicativo em uma URL voltada para o público usando HTTPS. Instale [ngrok](https://ngrok.com/download) e crie um túnel da Internet para localhost:3000 com o seguinte comando:

```bash
ngrok http 3000
```
No diretório do projeto, localize o `.publish\Development.env` arquivo e substitua o valor por sua URL `baseUrl0` ngrok.

## <a name="add-the-microsoft-graph-toolkit"></a>Adicionar o microsoft graph Toolkit

Você pode usar o microsoft graph Toolkit em seu aplicativo fazendo referência ao carregador diretamente (por meio de unpkg) ou instalando o pacote npm. Para usar o Toolkit, você também precisará do [SDK do Microsoft Teams.](/javascript/api/overview/msteams-client?view=msteams-client-js-latest)

### <a name="use-via-mgt-loader"></a>Usar por meio do mgt-loader
Para usar o Toolkit e o SDK do Teams por meio dos carregadores, adicione as seguintes referências a `public/index.html` :

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```

### <a name="use-via-npm-es6-modules"></a>Usar por npm (módulos ES6)
Usar o Toolkit por meio de módulos ES6 dará a você controle total do processo de empacotamento e permitirá que você empacote apenas o código necessário para seu aplicativo. Para usar os módulos ES6, adicione os pacotes npm para o Toolkit e o SDK do Microsoft Teams ao seu projeto:

```bash
npm install @microsoft/mgt @microsoft/teams-js
```

## <a name="initialize-the-teams-provider"></a>Inicializar o provedor do Teams

Os provedores Toolkit Microsoft Graph permitem autenticação e acesso ao Microsoft Graph para os componentes. Para saber mais, confira [Usando os provedores](../providers/providers.md). O [provedor do Teams](../providers/teams.md) lida com toda a lógica e interações que precisam ser implementadas com o SDK do Teams para autenticar o usuário.

Você pode optar por inicializar o provedor em seu HTML ou no código JavaScript. 

### <a name="initialize-in-html"></a>Inicializar em HTML

Em `public/index.html` , adicione o provedor do Teams conforme mostrado.

```html
<mgt-teams-provider
  client-id="<YOUR_CLIENT_ID>"
  auth-popup-url="https://<YOUR_NGROK_URL>/auth.html"
></mgt-teams-provider>
```

Substitua `<YOUR_CLIENT_ID>` pela ID do cliente para seu aplicativo e `<YOUR_NGROK_URL>` pela URL de ngrok que você criou.

### <a name="initialize-in-javascript"></a>Inicializar em JavaScript

Para inicializar o provedor em seu código JavaScript, localize o `src/components/App.js` arquivo no diretório do projeto. Importe o Provedor do Teams e inicialize o provedor.

```js
import * as microsoftTeams from "@microsoft/teams-js";
import { Providers, TeamsProvider } from '@microsoft/mgt';

TeamsProvider.microsoftTeamsLib = microsoftTeams;
Providers.globalProvider = new TeamsProvider ({
    clientId: '<YOUR_CLIENT_ID>',
    authPopupUrl: '/auth.html'
})
```
Substitua `<YOUR_CLIENT_ID>` pela ID do cliente para seu aplicativo.

### <a name="creating-an-appclient-id"></a>Criando uma ID de aplicativo/cliente
Para obter uma ID do cliente, você precisa registrar [seu aplicativo](../../auth-register-app-v2.md) no Azure AD. Certifique-se de adicionar sua URL ngrok com o caminho completo para a página pop-up de autenticação para suas URIs de redirecionamento (por exemplo, `https://<YOUR_NGROK_URL>/auth.html` ).
>**Observação**: O MSAL só dá suporte ao Fluxo Implícito para OAuth. Certifique-se de habilitar o Fluxo Implícito em seu aplicativo no Portal do Azure (ele não está habilitado por padrão). Em **Autenticação**, encontre a seção **Concessão implícita** e selecione as caixas de seleção para **tokens de Acesso** e **tokens de ID**. 

## <a name="create-the-auth-popup-page"></a>Criar a página pop-up de auth

Para permitir que os usuários entre, você precisa fornecer uma URL que o aplicativo do Teams abrirá em um pop-up para seguir o fluxo de autenticação. A URL precisa estar em seu domínio, e tudo o que essa página precisa fazer é chamar o `TeamsProvider.handleAuth()` método.

Você pode fazer isso em seu HTML adicionando um novo arquivo na pasta (que deve estar no mesmo nível que ) e adicionando `auth.html` `public` o seguinte `index.html` código: 

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<script>
  mgt.TeamsProvider.handleAuth();
</script>
```

## <a name="add-components"></a>Adicionar componentes

Agora, você está pronto para adicionar qualquer um dos componentes do Microsoft Graph Toolkit à guia. 

Você pode adicionar componentes ao HTML como normalmente faria. Por exemplo, para adicionar o componente Logon, adicione o código abaixo ao corpo do `index.html` seu :

```html
<mgt-login></mgt-login>
```

Ou você pode adicionar os componentes no JSX ao componente Tab. Recomendamos o uso `mgt-react` da biblioteca se você criou seu aplicativo do Teams usando a extensão microsoft teams Toolkit extensão. Para saber mais, consulte [Using Microsoft Graph Toolkit with React](./use-toolkit-with-react.md)

Primeiro, instale `mgt-react` :

```bash
npm install @microsoft/mgt-react
```

Localize `src/components/Tab.js` o arquivo e importe os componentes que você deseja usar na `mgt-react` biblioteca. Por exemplo, para adicionar o `Login` uso do componente:

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

Crie e execute seu aplicativo usando os seguintes comandos:
```bash
npm install
npm start
```

Para testar seu aplicativo, você precisa carregar seu aplicativo no Teams. Abra o cliente do Microsoft Teams, selecione **o ...** no menu à esquerda e vá para **App Studio**. Clique na **guia Editor de Manifesto** e selecione Importar um aplicativo **existente.**

Localize o diretório do projeto e carregue **o arquivoDevelopment.zip** dentro da pasta **.publish.**

Depois que o aplicativo tiver sido carregado, role para baixo no menu esquerdo e selecione **Testar e Distribuir**. Clique no **botão Instalar** e clique em **Adicionar**. Você será redirecionado para a guia criada.

## <a name="next-steps"></a>Próximas etapas
- Confira este tutorial passo a passo sobre [como criar uma guia do Teams.](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-10-microsoft-graph-toolkit-teams-provider/)
- Experimente os componentes no [playground](https://mgt.dev).
- Faça uma pergunta sobre [Stack Overflow](https://aka.ms/mgt-question).
- Relatar bugs ou deixar uma solicitação de recurso [no GitHub](https://aka.ms/mgt).
