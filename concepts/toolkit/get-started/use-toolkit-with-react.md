---
title: Usar o Kit de Ferramentas do Microsoft Graph com o React
description: Começar a usar o Microsoft Graph Toolkit em um aplicativo React.
localization_priority: Normal
author: waldekmastykarz
ms.openlocfilehash: 1ed264233e24f542a3cc0e23d664f1977cbe318f
ms.sourcegitcommit: d02c438bcd58e8f64bfcd5fba0b40e436b46570e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/04/2021
ms.locfileid: "50101885"
---
# <a name="use-the-microsoft-graph-toolkit-with-react"></a>Usar o Kit de Ferramentas do Microsoft Graph com o React

O Microsoft Graph Toolkit é um conjunto de componentes da Web que simplificam a conexão com o Microsoft Graph e permitem que você se concentre no seu aplicativo. O Microsoft Graph Toolkit está disponível como um conjunto genérico de componentes web distribuídos por meio do `@microsoft/mgt` pacote npm.

Se você estiver criando aplicativos com [ `@microsoft/mgt-react` ](./mgt-react.md)o React, poderá usar o pacote, que envolve os componentes web do Microsoft Graph Toolkit em componentes do React e facilita a passagem de dados complexos.

Este artigo descreve o processo passo a passo de usar o Kit de Ferramentas do Microsoft Graph para criar um aplicativo React e conectá-lo ao Microsoft 365. Depois de concluir as etapas, você terá um aplicativo React que mostra os próximos compromissos do usuário atualmente assinado do Microsoft 365.

## <a name="prerequisites"></a>Pré-requisitos

Para seguir as etapas deste artigo, você precisará de um ambiente de desenvolvimento do Microsoft 365 e algumas ferramentas. Para obter detalhes, veja [como começar.](./overview.md)

## <a name="create-a-react-app"></a>Criar um aplicativo React

Crie um novo aplicativo React executando o seguinte comando. Isso criará um novo aplicativo React usando TypeScript, que ajudará você a escrever código mais robusto e evitar erros de tempo de execução.

```cmd
npx create-react-app my-m365-app --template typescript --use-npm
```

Altere o diretório de trabalho para o aplicativo recém-criado.

```cmd
cd my-m365-app
```

Em seguida, instale o `mgt-react` pacote npm, que contém os componentes do React do Kit de Ferramentas do Microsoft Graph.

```cmd
npm i @microsoft/mgt-react
```

Instale também `mgt-msal-provider` `mgt-element` o pacote npm, que contém o provedor de auth MSAL.

```cmd
npm i @microsoft/mgt-element @microsoft/mgt-msal-provider
```

Confirme se você pode executar o aplicativo.

```cmd
npm start
```

Você deve ser capaz de abrir seu aplicativo no navegador via `http://localhost:3000` .

[!INCLUDE [AAD with implicit flow app registration](../includes/aad-app-registration-spa.md)]

## <a name="connect-react-app-to-microsoft-365"></a>Conectar o aplicativo React ao Microsoft 365

Agora que você registrou seu aplicativo no Azure Active Directory (Azure AD), poderá conectar o aplicativo React ao Microsoft 365. Primeiro, permita que os usuários se inscrevam no aplicativo usando a conta da Microsoft.

### <a name="copy-the-azure-ad-application-registration-id"></a>Copiar a ID de registro do aplicativo Azure AD

1. No Portal do Azure, vá para o registro do seu aplicativo.
1. Verifique se você está na página **Visão** Geral.
1. Na seção **Essentials,** copie o valor da propriedade **de ID do aplicativo (cliente)**

### <a name="configure-the-microsoft-graph-toolkit-authentication-provider"></a>Configurar o provedor de autenticação do Microsoft Graph Toolkit

Em seguida, configure o provedor de autenticação que o Microsoft Graph Toolkit deve usar. Nesse caso, você usará a MSAL, que é um bom padrão para a criação de aplicativos autônomos. Se você usar qualquer um dos pontos de extensibilidade no Microsoft 365, como o Teams ou o SharePoint, você usará [outros provedores.](../providers/providers.md)

1. No editor de código, abra **o src/index.** e na lista de importações, adicione:

    ```tsx
    import { Providers } from '@microsoft/mgt-element';
    import { MsalProvider } from '@microsoft/mgt-msal-provider';
    ```

1. Após a última `import` instrução, inicialize o Microsoft Graph Toolkit com o provedor MSAL.

    ```tsx
    Providers.globalProvider = new MsalProvider({
      clientId: 'REPLACE_WITH_CLIENTID'
    });
    ```

    Substitua o valor da `clientId` propriedade pelo valor da propriedade que você `Application (client) ID` copiou anteriormente no Portal do Azure.

Com essas alterações, o **arquivo src/index.tsx** terá a seguinte aparência.

  ```tsx
  import React from 'react';
  import ReactDOM from 'react-dom';
  import App from './App';
  import './index.css';
  import * as serviceWorker from './serviceWorker';

  import { Providers } from '@microsoft/mgt-element';
  import { MsalProvider } from '@microsoft/mgt-msal-provider';
  
  Providers.globalProvider = new MsalProvider({
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

Adicione o **componente React** do Kit de  Ferramentas do Microsoft Graph de logon, que exibirá o botão Entrar que as pessoas podem usar para entrar com a conta da Microsoft em seu aplicativo.

1. No editor de código, abra o **arquivo src/App.tsx** e adicione à lista de importações:

    ```tsx
    import { Login } from '@microsoft/mgt-react';
    ```

1. Na função, substitua o conteúdo da cláusula pela estrutura básica, incluindo o componente logon do Kit de Ferramentas `App` `return` do Microsoft Graph:

    ```tsx
    <div className="App">
      <header>
        <Login />
      </header>
    </div>
    ```

Com essas alterações, o **arquivo src/App.tsx** terá a seguinte aparência.
```tsx

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

### <a name="test-signing-in-to-your-application"></a>Testar a assinatura em seu aplicativo

Agora você poderá entrar em seu aplicativo com sua conta da Microsoft.

1. Volte para o navegador em que seu aplicativo React está sendo executado. Agora você deve ver um **botão Entrar.**
1. Ao clicar  no botão Entrar, você será solicitado a entrar com sua conta da Microsoft (você pode usar a mesma conta que a que acessou o Portal do Azure).
1. Como esta é a primeira vez que você está usando esse aplicativo Azure AD, precisa consentir seu uso em sua organização.
1. Depois de entrar, você será redirecionado para seu aplicativo React. Observe que o **botão** Entrar foi alterado para mostrar o nome do aplicativo React do usuário mostrando as informações do usuário recuperadas do ![ Microsoft 365 usando o Microsoft Graph ](../images/mgt-react-userinfo.png) Toolkit.

## <a name="load-data-from-microsoft-365"></a>Carregar dados do Microsoft 365

O Microsoft Graph Toolkit não apenas simplifica a autenticação para o Microsoft 365, mas também carrega seus dados. Neste exemplo, você mostrará o calendário da pessoa.

### <a name="specify-permissions-needed-for-your-application"></a>Especificar permissões necessárias para seu aplicativo

Antes de carregar dados do Microsoft 365, você precisa especificar a lista de escopos de permissão que seu aplicativo deve ter para acessar os dados do usuário. Esses escopos diferem dependendo do tipo de informação que você deseja mostrar. Nesse caso, você precisará de acesso ao calendário das pessoas, bem como acesso básico a informações sobre as pessoas que também são exibidas no calendário. Você pode encontrar os escopos exigidos por cada API na documentação da [API do Microsoft Graph.](/graph/api/overview)

1. No editor de código, abra o **arquivo src/index.tsx** e atualize o código de inicialização do provedor.

    ```tsx
    Providers.globalProvider = new MsalProvider({
      clientId: 'd7cb93c9-9097-4e38-8f06-7c0088ac3318',
      scopes: ['calendars.read', 'user.read', 'openid', 'profile', 'people.read', 'user.readbasic.all']
    });
    ```

### <a name="show-users-data-after-signing-in"></a>Mostrar dados do usuário após entrar

Em seguida, estenda o aplicativo para mostrar dados do calendário do usuário. Você só poderá acessar essas informações depois que o usuário entrar. Para fazer isso, você precisará controlar o estado de login do usuário e mostrar os dados do calendário depois que o usuário entrar com a conta da Microsoft.

#### <a name="track-users-sign-in-state"></a>Acompanhar o estado de login do usuário

Para controlar o estado de login do usuário em seu aplicativo, você usará o React e os ganchos em combinação com manipuladores de `useState` `useEffect` eventos do provedor.

1. No editor de código, abra o **arquivo src/App.tsx** e estenda a instrução React `import` existente.

    ```tsx
    import React, { useState, useEffect } from 'react';
    ```

1. Importe o `Provider` e os tipos de , `ProviderState` `mgt-element` adicionando às importações.

    ```tsx
    import { Providers, ProviderState } from '@microsoft/mgt-element';
    ```

1. Adicione uma função personalizada chamada que permite rastrear o estado de login do `useIsSignedIn` usuário em seu aplicativo.

    ```tsx
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

Esta função faz duas coisas. Primeiro, usando o `useState` gancho do React, ele habilita o estado de rastreamento dentro do componente. Sempre que o estado mudar, o React renderizará o componente. Em segundo lugar, usando o gancho react, ele estende o ciclo de vida do componente rastreando as alterações no provedor do Microsoft Graph Toolkit e atualizando o `useEffect` componente, se necessário.

#### <a name="load-users-calendar-if-user-is-signed-in"></a>Carregar o calendário do usuário se o usuário estiver se inscreveu

Agora que você rastreia o estado de login do usuário em seu aplicativo, pode mostrar o calendário depois de entrar.

1. No editor de código, abra o **arquivo src/App.tsx** e, dentro da função **App,** adicione:

    ```tsx
    const [isSignedIn] = useIsSignedIn();
    ```

    Isso define uma constante Boolean, que você pode usar para determinar se o usuário está `isSignedIn` atualmente londo em seu aplicativo.

1. Estenda o conteúdo da cláusula com um componente adicional e o componente agenda do Kit de Ferramentas `return` `div` do Microsoft Graph.

    ```tsx
    <div>
      {isSignedIn &&
        <Agenda />}
    </div>
    ```

Com essas alterações, o **arquivo src/App.tsx** deve se parecer com o seguinte.

```tsx
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

### <a name="test-showing-users-calendar-after-they-signed-in"></a>Teste mostrando o calendário do usuário depois que ele se inscreveu

Com essas alterações, depois de entrar em seu aplicativo com sua conta da Microsoft, você deverá ver seu calendário.

1. Para ver as alterações, feche o navegador e abra-o novamente e vá para `http://localhost:3000` . Você faz isso porque alterou o valor da propriedade, o que afeta o token de acesso que você `scopes` solicita do Azure AD.
1. Escolha o **botão Entrar** e entre usando sua conta da Microsoft. Observe as adições à lista de permissões solicitadas na solicitação de consentimento. Isso porque você incluiu permissões adicionais na `scope` propriedade.
1. Depois de consentir o uso do aplicativo, você deverá ver informações sobre o usuário atual e seu calendário.

![Aplicativo concluído](../images/mgt-finished-app.png)

## <a name="next-steps"></a>Próximas etapas

- Veja [o que há no Kit de Ferramentas do Microsoft Graph.](../overview.md)
- Experimente os componentes no [playground.](https://mgt.dev)
- Faça uma pergunta no [Stack Overflow](https://aka.ms/mgt-question).
- Relatar bugs ou deixar uma solicitação de recurso [no GitHub.](https://aka.ms/mgt)
