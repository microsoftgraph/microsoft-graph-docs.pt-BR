---
title: Use o microsoft Graph Toolkit com React
description: Começar a usar o microsoft Graph Toolkit em um React aplicativo.
localization_priority: Normal
author: waldekmastykarz
ms.openlocfilehash: 0c06566824c6da06490f83693aedd7ef40ae282b
ms.sourcegitcommit: a2d81138de2a0404e611fbb535679199477ef3d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/08/2021
ms.locfileid: "52813069"
---
# <a name="use-the-microsoft-graph-toolkit-with-react"></a>Use o microsoft Graph Toolkit com React

O Microsoft Graph Toolkit é um conjunto de componentes da Web que simplificam a conexão com o Microsoft Graph e permitem que você se concentre em seu aplicativo. O Microsoft Graph Toolkit está disponível como um conjunto genérico de componentes web distribuídos por meio do `@microsoft/mgt` pacote npm.

Se você estiver criando aplicativos com React, poderá usar o pacote [ `@microsoft/mgt-react` ,](./mgt-react.md)que envolve os componentes da Web do Microsoft Graph Toolkit em componentes React e facilita a passagem de dados complexos.

Este artigo descreve o processo passo a passo de usar o microsoft Graph Toolkit para criar um aplicativo React e conectá-lo ao Microsoft 365. Depois de concluir as etapas, você terá um aplicativo React que mostra os próximos compromissos do usuário atualmente Microsoft 365.

## <a name="prerequisites"></a>Pré-requisitos

Para seguir as etapas deste artigo, você precisará de um ambiente Microsoft 365 desenvolvimento e algumas ferramentas. Para obter detalhes, consulte [getting started](./overview.md).

## <a name="create-a-react-app"></a>Criar um React aplicativo

Crie um novo React aplicativo executando o seguinte comando. Isso criará um novo aplicativo React usando TypeScript, o que ajudará você a escrever um código mais robusto e evitar erros de tempo de execução.

```Command Line
npx create-react-app my-m365-app --template typescript --use-npm
```

Altere o diretório de trabalho para o aplicativo recém-criado.

```Command Line
cd my-m365-app
```

Em seguida, instale o `mgt-react` pacote npm, que contém os componentes Graph Toolkit React Microsoft.

```Command Line
npm i @microsoft/mgt-react
```

Instale o `mgt-msal2-provider` `mgt-element` pacote e npm também, que contém o provedor de auth MSAL 2.0.

```Command Line
npm i @microsoft/mgt-element @microsoft/mgt-msal2-provider
```

Confirme se você pode executar o aplicativo.

```Command Line
npm start
```

Você deve ser capaz de abrir seu aplicativo no navegador por `http://localhost:3000` meio de .

[!INCLUDE [AAD with implicit flow app registration](../includes/aad-app-registration-spa.md)]

## <a name="connect-react-app-to-microsoft-365"></a>Conexão React aplicativo para Microsoft 365

Agora que você registrou seu aplicativo com o Azure Active Directory (Azure AD), você pode conectar o aplicativo React ao Microsoft 365. Primeiro, permita que os usuários entre no aplicativo usando sua conta da Microsoft.

### <a name="copy-the-azure-ad-application-registration-id"></a>Copiar a ID de registro do aplicativo do Azure AD

1. No Portal do Azure, acesse o registro do aplicativo.
1. Verifique se você está na página **Visão** Geral.
1. Na seção **Essentials,** copie o valor da propriedade **Application (client) ID**

### <a name="configure-the-microsoft-graph-toolkit-authentication-provider"></a>Configurar o provedor de autenticação Graph Toolkit Microsoft

Em seguida, configure o provedor de autenticação que o microsoft Graph Toolkit deve usar. Nesse caso, você usará o MSAL, que é um bom padrão para a criação de aplicativos autônomos. Se você usar qualquer um dos pontos de extensibilidade no Microsoft 365, como Teams ou SharePoint, você usará [outros provedores](../providers/providers.md).

>[!NOTE] 
>Se você estiver usando o Provedor MSAL no momento e quiser atualizar para o Provedor MSAL 2, siga as etapas no artigo do provedor [MSAL 2.](../providers/msal2.md#migrating-from-msal-provider-to-msal-2-provider)

1. No editor de código, abra **o src/index.** e à lista de importações, adicione:

    ```TypeScript
    import { Providers } from '@microsoft/mgt-element';
    import { Msal2Provider } from '@microsoft/mgt-msal2-provider';
    ```

1. Após a última `import` instrução, inicialize o microsoft Graph Toolkit com o provedor MSAL.

    ```TypeScript
    Providers.globalProvider = new Msal2Provider({
      clientId: 'REPLACE_WITH_CLIENTID'
    });
    ```

    Substitua o valor da propriedade pelo valor da propriedade copiada `clientId` `Application (client) ID` anteriormente no Portal do Azure.

Com essas alterações, o **arquivo src/index.tsx** terá a seguinte aparência.

  ```tsx
  import React from 'react';
  import ReactDOM from 'react-dom';
  import App from './App';
  import './index.css';
  import * as serviceWorker from './serviceWorker';

  import { Providers } from '@microsoft/mgt-element';
  import { Msal2Provider } from '@microsoft/mgt-msal2-provider';
  
  Providers.globalProvider = new Msal2Provider({
    clientId: 'REPLACE_WITH_CLIENTID'
  });
  
  ReactDOM.render(
    <React.StrictMode>
      <App />
    </React.StrictMode>,
    document.getElementById('root')
  );
  
  // If you want your app to work offline and load faster, you can change
  // unregister() to register() below. Note this comes with some pitfalls.
  // Learn more about service workers: https://bit.ly/CRA-PWA
  serviceWorker.unregister();
  ```

### <a name="add-the-sign-in-button"></a>Adicionar o botão Entrar

Adicione o **componente Logon** do Microsoft Graph Toolkit React, que exibirá o botão Entrar que as pessoas podem usar para entrar com sua conta da Microsoft em seu aplicativo. 

1. No editor de código, abra o **arquivo src/App.tsx** e, na lista de importações, adicione:

    ```TypeScript
    import { Login } from '@microsoft/mgt-react';
    ```

1. Na `App` função, substitua o conteúdo da cláusula pela estrutura básica, incluindo o componente Graph Toolkit `return` Logon da Microsoft:

    ```TypeScript
    <div className="App">
      <header>
        <Login />
      </header>
    </div>
    ```

Com essas alterações, o **arquivo src/App.tsx** terá a seguinte aparência.
```TypeScript

import { Login } from '@microsoft/mgt-react';
import React from 'react';
import './App.css';

function App() {
  return (
    <div className="App">
      <header>
        <Login />
      </header>
    </div>
  );
}

export default App;
```

### <a name="test-signing-in-to-your-application"></a>Testar o registro no aplicativo

Agora você deve poder entrar no aplicativo com sua conta da Microsoft.

1. Volte para o navegador onde seu aplicativo React está sendo executado. Agora você deve ver um **botão Entrar.**
1. Ao clicar  no botão Entrar, você será solicitado a entrar com sua conta da Microsoft (você pode usar a mesma conta com a qual você acessou o Portal do Azure).
1. Como esta é a primeira vez que você está usando esse aplicativo do Azure AD, você precisa consentir seu uso em sua organização.
1. Depois de entrar, você será redirecionado para seu React app. Observe que o **botão** Entrar foi alterado para mostrar o nome do usuário React aplicativo mostrando informações do usuário recuperadas do Microsoft 365 usando o ![ Microsoft Graph Toolkit ](../images/mgt-react-userinfo.png) .

## <a name="load-data-from-microsoft-365"></a>Carregar dados de Microsoft 365

A Microsoft Graph Toolkit simplifica a autenticação para Microsoft 365, mas também carrega seus dados. Neste exemplo, você mostrará o calendário da pessoa assinada.

### <a name="specify-permissions-needed-for-your-application"></a>Especificar permissões necessárias para seu aplicativo

Antes de carregar dados Microsoft 365, você precisa especificar a lista de escopos de permissão que seu aplicativo deve ter para acessar os dados do usuário. Esses escopos diferem dependendo do tipo de informação que você deseja mostrar. Nesse caso, você precisará de acesso ao calendário das pessoas, bem como acesso básico a informações sobre pessoas que também são exibidas no calendário. Você pode encontrar os escopos exigidos por cada API na documentação da [API Graph Microsoft.](/graph/api/overview)

1. No editor de código, abra o **arquivo src/index.tsx** e atualize o código de inicialização do provedor.

    ```TypeScript
    Providers.globalProvider = new Msal2Provider({
      clientId: 'REPLACE_WITH_CLIENTID',
      scopes: ['calendars.read', 'user.read', 'openid', 'profile', 'people.read', 'user.readbasic.all']
    });
    ```

### <a name="show-users-data-after-signing-in"></a>Mostrar dados do usuário após entrar

Em seguida, estenda o aplicativo para mostrar dados do calendário do usuário. Você só pode acessar essas informações depois que o usuário entrar. Para fazer isso, você precisará rastrear o estado de login do usuário e mostrar os dados do calendário depois que o usuário tiver se assinado com sua conta da Microsoft.

#### <a name="track-users-sign-in-state"></a>Controlar o estado de login do usuário

Para rastrear o estado de login do usuário em seu aplicativo, você usará o React e os ganchos em combinação com manipuladores de eventos `useState` `useEffect` do provedor.

1. No editor de código, abra o **arquivo src/App.tsx** e estenda a instrução React `import` existente.

    ```TypeScript
    import React, { useState, useEffect } from 'react';
    ```

1. Importe os `Provider` tipos e de , `ProviderState` `mgt-element` adicionando a importações.

    ```TypeScript
    import { Providers, ProviderState } from '@microsoft/mgt-element';
    ```

1. Adicione uma função personalizada chamada que permite controlar o estado de login do `useIsSignedIn` usuário em seu aplicativo.

    ```TypeScript
    function useIsSignedIn(): [boolean] {
      const [isSignedIn, setIsSignedIn] = useState(false);
    
      useEffect(() => {
        const updateState = () => {
          const provider = Providers.globalProvider;
          setIsSignedIn(provider && provider.state === ProviderState.SignedIn);
        };
    
        Providers.onProviderUpdated(updateState);
        updateState();
    
        return () => {
          Providers.removeProviderUpdatedListener(updateState);
        }
      }, []);
    
      return [isSignedIn];
    }
    ```

Essa função faz duas coisas. Primeiro, usando o `useState` React, ele habilita o estado de controle dentro do componente. Sempre que o estado mudar, React renderizará seu componente. Em segundo lugar, usando o React, ele estende o ciclo de vida do componente rastreando as alterações no provedor Graph Toolkit Microsoft e atualizando o componente, se `useEffect` necessário.

#### <a name="load-users-calendar-if-user-is-signed-in"></a>Carregar o calendário do usuário se o usuário estiver assinado

Agora que você rastreia o estado de login do usuário em seu aplicativo, você pode mostrar seu calendário depois de entrar.

1. No editor de código, abra o **arquivo src/App.tsx** e, dentro da função **App,** adicione:

    ```TypeScript
    const [isSignedIn] = useIsSignedIn();
    ```

    Isso define uma constante Boolean, que você pode usar para determinar se o usuário está atualmente `isSignedIn` dentro do aplicativo.

1. Estenda o conteúdo da cláusula com um componente de Agenda Graph Toolkit `return` `div` Microsoft.

    ```TypeScript
    <div>
      {isSignedIn &&
        <Agenda />}
    </div>
    ```

Com essas alterações, o **arquivo src/App.tsx** deve ter a seguinte aparência.

```TypeScript
import { Providers, ProviderState } from '@microsoft/mgt';
import { Agenda, Login } from '@microsoft/mgt-react';
import React, { useState, useEffect } from 'react';
import './App.css';

function useIsSignedIn(): [boolean] {
  const [isSignedIn, setIsSignedIn] = useState(false);

  useEffect(() => {
    const updateState = () => {
      const provider = Providers.globalProvider;
      setIsSignedIn(provider && provider.state === ProviderState.SignedIn);
    };

    Providers.onProviderUpdated(updateState);
    updateState();

    return () => {
      Providers.removeProviderUpdatedListener(updateState);
    }
  }, []);

  return [isSignedIn];
}

function App() {
  const [isSignedIn] = useIsSignedIn();

  return (
    <div className="App">
      <header>
        <Login />
      </header>
      <div>
        {isSignedIn &&
          <Agenda />}
      </div>
    </div>
  );
}

export default App;
```

### <a name="test-showing-users-calendar-after-they-signed-in"></a>Testar mostrando o calendário do usuário depois que ele se inscreveu

Com essas alterações, depois de entrar no aplicativo com sua conta da Microsoft, você deverá ver seu calendário.

1. Para ver as alterações, feche o navegador e abra-o novamente e vá para `http://localhost:3000` . Faça isso porque alterou o valor da propriedade, o que afeta o token de acesso solicitado `scopes` pelo Azure AD.
1. Escolha o **botão Entrar** e entre usando sua conta da Microsoft. Observe as adições à lista de permissões solicitadas no prompt de consentimento. Isso porque você incluiu permissões adicionais na `scope` propriedade.
1. Depois de concordar com o uso do aplicativo, você deverá ver informações sobre o usuário atual e seu calendário.

![Aplicativo concluído](../images/mgt-finished-app.png)

## <a name="next-steps"></a>Próximas etapas

- Veja [o que está no microsoft Graph Toolkit](../overview.md).
- Experimente os componentes no [playground](https://mgt.dev).
- Faça uma pergunta sobre [Stack Overflow](https://aka.ms/mgt-question).
- Relatar bugs ou deixar uma solicitação de recurso [GitHub](https://aka.ms/mgt).
