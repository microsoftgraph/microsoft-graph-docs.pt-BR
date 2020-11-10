---
title: Use o kit de ferramentas do Microsoft Graph com reagir
description: Introdução ao uso do kit de ferramentas do Microsoft Graph em um aplicativo reagir.
localization_priority: Normal
author: waldekmastykarz
ms.openlocfilehash: 8f570caf2be4c123bd9a9a93e45a5508029efdee
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48967753"
---
# <a name="use-the-microsoft-graph-toolkit-with-react"></a>Use o kit de ferramentas do Microsoft Graph com reagir

O Microsoft Graph Toolkit é um conjunto de componentes Web que simplifica a conexão com o Microsoft Graph e permite que você se concentre em seu aplicativo. O Microsoft Graph Toolkit está disponível como um conjunto genérico de componentes Web distribuídos por meio do pacote **@microsoft/MGT** NPM.

Se você estiver criando aplicativos com reagir, poderá usar o pacote **@microsoft/MGT-React** , que encapsula o Microsoft Graph Toolkit Web Components em reagir componentes e torna mais fácil transmitir dados complexos.

Este artigo descreve o processo passo a passo de usar o kit de ferramentas do Microsoft Graph para criar um aplicativo reagir e conectá-lo ao Microsoft 365. Após concluir as etapas, você terá um aplicativo reagir que mostra os futuros compromissos do usuário conectado no momento da Microsoft 365.

## <a name="prerequisites"></a>Pré-requisitos

Para seguir as etapas deste artigo, você precisará de um ambiente de desenvolvimento do Microsoft 365 e de algumas ferramentas. Para obter detalhes, consulte [introdução](./overview.md).

## <a name="create-a-react-app"></a>Criar um aplicativo reagir

Crie um novo aplicativo reagir executando o seguinte comando. Isso criará um novo aplicativo reagir usando TypeScript, que o ajudará a escrever código mais robusto e evitar erros de tempo de execução.

```cmd
npx create-react-app my-m365-app --template typescript
```

Altere o diretório de trabalho para o aplicativo recém-criado.

```cmd
cd my-m365-app
```

Em seguida, instale o pacote NPM **-reajam** , que contém os componentes de reagir do Microsoft Graph Toolkit.

```cmd
npm i @microsoft/mgt-react
```

Confirme que você pode executar o aplicativo.

```cmd
HTTPS=true npm start
```

> [!IMPORTANT]
> Seu aplicativo precisa ser executado em HTTPS para poder autenticar-se no Microsoft 365. Para teste local, com os scripts de reagir, você pode configurar o servidor Web local para ser executado em HTTPS, definindo a `HTTPS` variável de ambiente como `true` . Você pode fazer isso sempre, prefixando o `npm start` comando com `HTTPS=true` (funciona apenas em bash) ou configurando a variável de ambiente globalmente no computador.

Você deve ser capaz de abrir seu aplicativo no navegador via `https://localhost:3000` .

[!INCLUDE [AAD with implicit flow app registration](../includes/aad-app-registration-spa.md)]

## <a name="connect-react-app-to-microsoft-365"></a>Conectar aplicativo reagir ao Microsoft 365

Agora que você registrou seu aplicativo com o Azure Active Directory (Azure AD), você pode conectar o aplicativo reagir ao Microsoft 365. Primeiro, permita que os usuários entrem no aplicativo usando sua conta da Microsoft.

### <a name="copy-the-azure-ad-application-registration-id"></a>Copiar a ID de registro do aplicativo do Azure AD

1. No portal do Azure, vá para o registro do aplicativo.
1. Verifique se você está na página de **visão geral** .
1. Na seção **Essentials** , copie o valor da propriedade **ID do aplicativo (cliente)**

### <a name="configure-the-microsoft-graph-toolkit-authentication-provider"></a>Configurar o provedor de autenticação do kit de ferramentas do Microsoft Graph

Em seguida, configure o provedor de autenticação que o Microsoft Graph Toolkit deve usar. Nesse caso, você usará o MSAL, que é um bom padrão para criar aplicativos autônomos. Se você usar qualquer um dos pontos de extensibilidade no Microsoft 365, como o Teams ou o SharePoint, você usará [outros provedores](../providers.md).

1. No editor de código, abra **src/index.** e, na lista de importações, adicione:

    ```tsx
    import { MsalProvider, Providers } from '@microsoft/mgt';
    ```

1. Após a última `import` instrução, inicialize o Microsoft Graph Toolkit com o provedor MSAL.

    ```tsx
    Providers.globalProvider = new MsalProvider({
      clientId: 'REPLACE_WITH_CLIENTID'
    });
    ```

    Substitua o valor da `clientId` propriedade com o valor da `Application (client) ID` propriedade que você copiou anteriormente no portal do Azure.

Com essas alterações, o arquivo **src/index. TSX** será semelhante ao seguinte.

  ```tsx
  import { MsalProvider, Providers } from '@microsoft/mgt';
  import React from 'react';
  import ReactDOM from 'react-dom';
  import App from './App';
  import './index.css';
  import * as serviceWorker from './serviceWorker';
  
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

### <a name="add-the-sign-in-button"></a>Adicionar o botão entrar

Adicione o componente de **logon** do Microsoft Graph Toolkit para reagir, que exibirá o botão de **entrada** que as pessoas podem usar para entrar com sua conta da Microsoft em seu aplicativo.

1. No editor de códigos, abra o arquivo **src/app. TSX** e, na lista de importações, adicione:

    ```tsx
    import { Login } from '@microsoft/mgt-react';
    ```

1. Na `App` função, substitua o conteúdo da `return` cláusula pela estrutura básica, incluindo o componente de logon do Microsoft Graph Toolkit:

    ```tsx
    <div className="App">
      <header>
        <Login />
      </header>
    </div>
    ```

Com essas alterações, o arquivo **src/app. TSX** será semelhante ao seguinte.
```tsx
import { MsalProvider, Providers } from '@microsoft/mgt';
import { Login } from '@microsoft/mgt-react';
import React from 'react';
import './App.css';

function App() {
  Providers.globalProvider = new MsalProvider({
    clientId: 'REPLACE_WITH_CLIENTID'
  });

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

### <a name="test-signing-in-to-your-application"></a>Testar sessão no seu aplicativo

Agora você poderá entrar no seu aplicativo com sua conta da Microsoft.

1. Volte para o navegador onde seu aplicativo reagir está em execução. Agora você deve ver um botão **entrar** .
1. Ao clicar no botão **entrar** , você será solicitado a entrar com sua conta da Microsoft (você pode usar a mesma conta que você acessou o portal do Azure).
1. Como esta é a primeira vez que você está usando esse aplicativo do Azure AD, você precisa consentir seu uso na sua organização.
1. Após entrar, você será redirecionado para seu aplicativo reagir. Observe que o botão **entrar** foi alterado para mostrar o nome do seu usuário ![ aplicativo reagir mostrando as informações do usuário recuperadas do Microsoft 365 usando o Microsoft Graph Toolkit ](../images/mgt-react-userinfo.png) .

## <a name="load-data-from-microsoft-365"></a>Carregar dados do Microsoft 365

O Microsoft Graph Toolkit não apenas simplifica a autenticação para o Microsoft 365, mas também o carregamento dos dados. Neste exemplo, você mostrará o calendário do usuário conectado.

### <a name="specify-permissions-needed-for-your-application"></a>Especificar permissões necessárias para seu aplicativo

Antes de poder carregar dados do Microsoft 365, você precisa especificar a lista de escopos de permissão que seu aplicativo deve ser concedido para acessar os dados do usuário. Esses escopos diferem, dependendo do tipo de informação que você deseja exibir. Nesse caso, você precisará acessar o calendário de pessoas e o acesso básico às informações sobre as pessoas que também são exibidas no calendário. Você pode encontrar os escopos exigidos por cada API na [documentação da API do Microsoft Graph](/graph/api/overview?toc=.%2Fref%2Ftoc.json&view=graph-rest-1.0).

1. No editor de códigos, abra o arquivo **src/index. TSX** e atualize o código de inicialização do provedor.

    ```tsx
    Providers.globalProvider = new MsalProvider({
      clientId: 'd7cb93c9-9097-4e38-8f06-7c0088ac3318',
      scopes: ['calendars.read', 'user.read', 'openid', 'profile', 'people.read', 'user.readbasic.all']
    });
    ```

### <a name="show-users-data-after-signing-in"></a>Mostrar dados do usuário após entrar

Em seguida, estenda o aplicativo para mostrar os dados do calendário do usuário. Você pode acessar essas informações somente depois que o usuário entrar. Para fazer isso, você precisará controlar o estado de entrada do usuário e mostrar os dados do calendário depois que o usuário entrar com a conta da Microsoft.

#### <a name="track-users-sign-in-state"></a>Rastrear o estado de entrada do usuário

Para acompanhar o estado de entrada do usuário em seu aplicativo, você usará a combinação de reagir `useState` e `useEffect` conexões com os manipuladores de eventos do provedor.

1. No editor de códigos, abra o arquivo **src/app. TSX** e estenda a instrução de reagir existente `import` .

    ```tsx
    import React, { useState, useEffect } from 'react';
    ```

1. Importe os `Provider` `ProviderState` tipos e do Microsoft Graph Toolkit adicionando às importações.

    ```tsx
    import { Providers, ProviderState } from '@microsoft/mgt';
    ```

1. Adicione uma função personalizada nomeada `useIsSignedIn` que permite o acompanhamento do estado de entrada do usuário em seu aplicativo.

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

Essa função faz duas coisas. Primeiro, usando o gancho de reagir `useState` , ele habilita o estado de controle dentro de seu componente. Sempre que o estado for alterado, reagir reprocessará seu componente. Em segundo lugar, usando o gancho de reagir `useEffect` , ele estende o ciclo de vida do componente ao controlar as alterações no provedor do Microsoft Graph Toolkit e atualizar o componente, se necessário.

#### <a name="load-users-calendar-if-user-is-signed-in"></a>Carregar calendário do usuário se o usuário estiver conectado

Agora que você acompanha o estado de entrada do usuário em seu aplicativo, você pode mostrar seu calendário após ele entrar.

1. No editor de códigos, abra o arquivo **src/app. TSX** e, dentro da função **app** , adicione:

    ```tsx
    const [isSignedIn] = useIsSignedIn();
    ```

    Isso define uma constante booleana `isSignedIn` , que você pode usar para determinar se o usuário está atualmente conectado ao seu aplicativo.

1. Estenda o conteúdo da `return` cláusula com um componente de `div` programação adicional e o Microsoft Graph Toolkit.

    ```tsx
    <div>
      {isSignedIn &&
        <Agenda />}
    </div>
    ```

Com essas alterações, o arquivo **src/app. TSX** deve ser semelhante ao seguinte.

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

### <a name="test-showing-users-calendar-after-they-signed-in"></a>Teste mostrando o calendário do usuário depois que ele entrou

Com essas alterações, após entrar em seu aplicativo com sua conta da Microsoft, você deve ver seu calendário.

1. Para ver as alterações, feche o navegador e abra-o novamente e vá para `https://localhost:3000` . Isso é feito porque você alterou o valor da `scopes` propriedade, que afeta o token de acesso solicitado pelo Azure AD.
1. Escolha o botão **entrar** e entre usando sua conta da Microsoft. Observe as adições à lista de permissões solicitadas no prompt de consentimento. Isso ocorre porque você incluiu permissões adicionais na `scope` propriedade.
1. Após a reenvio ao uso do aplicativo, você deve ver informações sobre o usuário atual e seu calendário.

![Aplicativo concluído](../images/mgt-finished-app.png)

## <a name="next-steps"></a>Próximas etapas

- Veja [o que há no Microsoft Graph Toolkit](../overview.md).
- Experimente os componentes no [playground](https://mgt.dev).
- Faça uma pergunta sobre o [estouro de pilha](https://aka.ms/mgt-question).
- Informe bugs ou deixe uma solicitação de recurso no [GitHub](https://aka.ms/mgt).
