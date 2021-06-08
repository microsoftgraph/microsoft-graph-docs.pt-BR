---
title: Crie uma Microsoft Teams com o microsoft Graph Toolkit
description: Começar a criar uma guia Microsoft Teams usando o microsoft Graph Toolkit.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 7bd9d989d30b7fc4286a6ca78445ffb01a772084
ms.sourcegitcommit: a2d81138de2a0404e611fbb535679199477ef3d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/08/2021
ms.locfileid: "52813164"
---
# <a name="build-a-microsoft-teams-tab-with-the-microsoft-graph-toolkit"></a>Crie uma Microsoft Teams com o microsoft Graph Toolkit

Este tópico aborda como começar a usar o microsoft Graph Toolkit em uma solução Microsoft Teams. Começar envolve as seguintes etapas:

1. Crie um novo Teams com uma guia personalizada.
2. Adicione o microsoft Graph Toolkit.
3. Inicializar o Microsoft Teams provedor.
4. Crie a página pop-up de auth.
5. Adicione componentes.
6. Teste seu aplicativo.

## <a name="create-a-new-teams-application-with-a-custom-tab"></a>Criar um novo aplicativo Teams com uma guia personalizada

A maneira mais fácil de criar um novo aplicativo Teams é usar a extensão [Microsoft Teams Toolkit para](https://marketplace.visualstudio.com/items?itemName=TeamsDevApp.ms-teams-vscode-extension) Visual Studio Code. Siga as instruções para [configurar um novo Teams projeto](/microsoftteams/platform/toolkit/visual-studio-code-overview#set-up-a-new-teams-project). Quando você chegar à tela **Adicionar recursos,** selecione **Guia** e, em seguida, **guia Pessoal.**

## <a name="add-the-microsoft-graph-toolkit"></a>Adicionar o microsoft Graph Toolkit

Você pode usar o microsoft Graph Toolkit em seu aplicativo fazendo referência ao carregador diretamente (via unpkg) ou instalando o pacote npm. Para usar o Toolkit, você também precisará do [Microsoft Teams SDK](/javascript/api/overview/msteams-client?view=msteams-client-js-latest).

### <a name="use-via-mgt-loader"></a>Usar por meio do mgt-loader
Para usar o Toolkit e Teams SDK por meio dos carregadores, adicione as seguintes referências dentro `<head>` do `public/index.html` arquivo:

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```

### <a name="use-via-npm-es6-modules"></a>Usar por npm (módulos ES6)
Usar o Toolkit por meio de módulos ES6 dará a você controle total do processo de empacotamento e permitirá que você empacote apenas o código necessário para seu aplicativo. Para usar os módulos ES6, adicione os pacotes npm para o Toolkit e o SDK Microsoft Teams ao seu projeto:

```bash
npm install @microsoft/mgt @microsoft/teams-js
```

## <a name="initialize-the-teams-provider"></a>Inicializar o provedor Teams

Os provedores Graph Toolkit Microsoft habilitam a autenticação e o acesso ao Microsoft Graph para os componentes. Para saber mais, confira [Usando os provedores](../providers/providers.md). O [Teams provedor](../providers/teams.md) lida com toda a lógica e interações que precisam ser implementadas com o SDK Teams para autenticar o usuário.

Você pode optar por inicializar o provedor em seu HTML ou no código JavaScript. 

### <a name="initialize-in-html"></a>Inicializar em HTML

In `public/index.html` , add the Teams provider into the , as `<body>` shown.

```html
<mgt-teams-provider
  client-id="<YOUR_CLIENT_ID>"
  auth-popup-url="/auth.html"
></mgt-teams-provider>
```

Substitua `<YOUR_CLIENT_ID>` pela ID do cliente para seu aplicativo. 

### <a name="initialize-in-javascript"></a>Inicializar em JavaScript

Para inicializar o provedor em seu código JavaScript, localize o `src/components/App.js` arquivo no diretório do projeto. Importe o Teams Provedor e inicialize o provedor.

```JavaScript
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

Para obter uma ID do cliente, você precisa registrar um aplicativo Azure Active Directory cliente. Siga as etapas no [artigo Criar um Azure Active Directory app.](./add-aad-app-registration.md)

Certifique-se de definir o **URI de** redirecionamento no registro do aplicativo para apontar para sua `auth.html` página. Por exemplo, se você estiver executando seu aplicativo `localhost:3000` em , de definir o URI de redirecionamento como `https://localhost:3000/auth.html` .

>**Observação**: O MSAL só dá suporte ao Flow implícito para OAuth. Certifique-se de habilitar o Flow implícito em seu aplicativo no Portal do Azure (ele não está habilitado por padrão). Em **Autenticação**, encontre a seção **Concessão implícita** e selecione as caixas de seleção para **tokens de Acesso** e **tokens de ID**. 

## <a name="create-the-auth-popup-page"></a>Criar a página pop-up de auth

Para permitir que os usuários entre, você precisa fornecer uma URL que o aplicativo Teams abrirá em um pop-up para seguir o fluxo de autenticação. A URL precisa estar em seu domínio, e tudo o que essa página precisa fazer é chamar o `TeamsProvider.handleAuth()` método.

Você pode fazer isso adicionando um novo arquivo na pasta (que deve estar no mesmo nível que ) e adicionando `auth.html` `public` o seguinte `index.html` código: 

```html
<!DOCTYPE html>
<html>
  <head>
    <script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
    <script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
  </head>

  <body>
    <script>
      mgt.TeamsProvider.handleAuth();
    </script>
  </body>
</html>
```

## <a name="add-components"></a>Adicionar componentes

Agora, você está pronto para adicionar qualquer um dos componentes do Microsoft Graph Toolkit à sua guia. 

Você pode adicionar componentes ao HTML como normalmente faria. Por exemplo, para adicionar o componente Logon, adicione o código abaixo ao corpo do `index.html` seu :

```HTML
<mgt-login></mgt-login>
```

Ou você pode adicionar os componentes no JSX ao componente Tab. Recomendamos usar a `mgt-react` biblioteca se você criou seu aplicativo Teams usando a extensão Microsoft Teams Toolkit de usuário. Para saber mais, consulte [Using Microsoft Graph Toolkit with React](./use-toolkit-with-react.md)

Primeiro, instale `mgt-react` :

```Command Line
npm install @microsoft/mgt-react
```

Localize `src/components/Tab.js` o arquivo e importe os componentes que você deseja usar na `mgt-react` biblioteca. Por exemplo, para adicionar o `Login` uso do componente:

```JavaScript
import { Login } from "@microsoft/mgt-react"
```

Em seguida, adicione o componente à `return()` instrução do `render()` método de `Tab` :

```JavaScript
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

Para testar seu aplicativo, você pode instalar seu aplicativo para Teams por meio do Teams Toolkit Extension. Abra o Teams Toolkit Extension e clique **em Abrir Microsoft Teams Toolkit**. Clique **em App Studio** no menu esquerdo, role para baixo e selecione Testar e **Distribuir**, em **seguida, Instalar**. Teams abrirá no navegador e você será redirecionado para a guia criada. Você deve ser capaz de ver o componente de Logon e usá-lo para entrar no seu aplicativo.

## <a name="next-steps"></a>Próximas etapas
- Confira este tutorial passo a passo sobre [como criar uma Teams guia](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-10-microsoft-graph-toolkit-teams-provider/).
- Experimente os componentes no [playground](https://mgt.dev).
- Faça uma pergunta sobre [Stack Overflow](https://aka.ms/mgt-question).
- Relatar bugs ou deixar uma solicitação de recurso [GitHub](https://aka.ms/mgt).
