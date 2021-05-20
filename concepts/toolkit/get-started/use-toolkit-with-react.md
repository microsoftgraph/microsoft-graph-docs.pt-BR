---
title: Use o microsoft Graph Toolkit com React
description: Começar a usar o microsoft Graph Toolkit em um React aplicativo.
localization_priority: Normal
author: waldekmastykarz
ms.openlocfilehash: a1eaf17b4d4b12e04c11941ab25c5e2bdfd6d57a
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579771"
---
# <a name="use-the-microsoft-graph-toolkit-with-react"></a><span data-ttu-id="1fdf6-103">Use o microsoft Graph Toolkit com React</span><span class="sxs-lookup"><span data-stu-id="1fdf6-103">Use the Microsoft Graph Toolkit with React</span></span>

<span data-ttu-id="1fdf6-104">O Microsoft Graph Toolkit é um conjunto de componentes da Web que simplificam a conexão com o Microsoft Graph e permitem que você se concentre em seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1fdf6-104">Microsoft Graph Toolkit is a set of web components that simplify connecting to Microsoft Graph and allow you to focus on your application instead.</span></span> <span data-ttu-id="1fdf6-105">O Microsoft Graph Toolkit está disponível como um conjunto genérico de componentes web distribuídos por meio do `@microsoft/mgt` pacote npm.</span><span class="sxs-lookup"><span data-stu-id="1fdf6-105">Microsoft Graph Toolkit is available as a generic set of web components distributed through the `@microsoft/mgt` npm package.</span></span>

<span data-ttu-id="1fdf6-106">Se você estiver criando aplicativos com React, poderá usar o pacote [ `@microsoft/mgt-react` ,](./mgt-react.md)que envolve os componentes da Web do Microsoft Graph Toolkit em componentes React e facilita a passagem de dados complexos.</span><span class="sxs-lookup"><span data-stu-id="1fdf6-106">If you're building apps with React, you can use the [`@microsoft/mgt-react` package](./mgt-react.md), which wraps Microsoft Graph Toolkit web components in React components and makes it easier to pass complex data.</span></span>

<span data-ttu-id="1fdf6-107">Este artigo descreve o processo passo a passo de usar o microsoft Graph Toolkit para criar um aplicativo React e conectá-lo ao Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="1fdf6-107">This article describes the step-by-step process of using the Microsoft Graph Toolkit to create a React app and connect it to Microsoft 365.</span></span> <span data-ttu-id="1fdf6-108">Depois de concluir as etapas, você terá um aplicativo React que mostra os próximos compromissos do usuário atualmente Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="1fdf6-108">After completing the steps, you'll have a React app that shows the upcoming appointments of the currently signed in user from Microsoft 365.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1fdf6-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1fdf6-109">Prerequisites</span></span>

<span data-ttu-id="1fdf6-110">Para seguir as etapas deste artigo, você precisará de um ambiente Microsoft 365 desenvolvimento e algumas ferramentas.</span><span class="sxs-lookup"><span data-stu-id="1fdf6-110">To follow the steps in this article, you'll need a Microsoft 365 development environment and a few tools.</span></span> <span data-ttu-id="1fdf6-111">Para obter detalhes, consulte [getting started](./overview.md).</span><span class="sxs-lookup"><span data-stu-id="1fdf6-111">For details, see [getting started](./overview.md).</span></span>

## <a name="create-a-react-app"></a><span data-ttu-id="1fdf6-112">Criar um React aplicativo</span><span class="sxs-lookup"><span data-stu-id="1fdf6-112">Create a React app</span></span>

<span data-ttu-id="1fdf6-113">Crie um novo React aplicativo executando o seguinte comando.</span><span class="sxs-lookup"><span data-stu-id="1fdf6-113">Create a new React app by running the following command.</span></span> <span data-ttu-id="1fdf6-114">Isso criará um novo aplicativo React usando TypeScript, o que ajudará você a escrever um código mais robusto e evitar erros de tempo de execução.</span><span class="sxs-lookup"><span data-stu-id="1fdf6-114">This will create a new React app using TypeScript, which will help you write more robust code and avoid runtime errors.</span></span>

```cmd
npx create-react-app my-m365-app --template typescript --use-npm
```

<span data-ttu-id="1fdf6-115">Altere o diretório de trabalho para o aplicativo recém-criado.</span><span class="sxs-lookup"><span data-stu-id="1fdf6-115">Change the working directory to the newly created app.</span></span>

```cmd
cd my-m365-app
```

<span data-ttu-id="1fdf6-116">Em seguida, instale o `mgt-react` pacote npm, que contém os componentes Graph Toolkit React Microsoft.</span><span class="sxs-lookup"><span data-stu-id="1fdf6-116">Next, install the `mgt-react` npm package, which contains the Microsoft Graph Toolkit React components.</span></span>

```cmd
npm i @microsoft/mgt-react
```

<span data-ttu-id="1fdf6-117">Instale o `mgt-msal2-provider` `mgt-element` pacote e npm também, que contém o provedor de auth MSAL 2.0.</span><span class="sxs-lookup"><span data-stu-id="1fdf6-117">Install the `mgt-msal2-provider` and `mgt-element` npm package as well, which contains the MSAL 2.0 auth provider.</span></span>

```cmd
npm i @microsoft/mgt-element @microsoft/mgt-msal2-provider
```

<span data-ttu-id="1fdf6-118">Confirme se você pode executar o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1fdf6-118">Confirm that you can run the app.</span></span>

```cmd
npm start
```

<span data-ttu-id="1fdf6-119">Você deve ser capaz de abrir seu aplicativo no navegador por `http://localhost:3000` meio de .</span><span class="sxs-lookup"><span data-stu-id="1fdf6-119">You should be able to open your app in the browser via `http://localhost:3000`.</span></span>

[!INCLUDE [AAD with implicit flow app registration](../includes/aad-app-registration-spa.md)]

## <a name="connect-react-app-to-microsoft-365"></a><span data-ttu-id="1fdf6-120">Conexão React aplicativo para Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="1fdf6-120">Connect React app to Microsoft 365</span></span>

<span data-ttu-id="1fdf6-121">Agora que você registrou seu aplicativo com o Azure Active Directory (Azure AD), você pode conectar o aplicativo React ao Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="1fdf6-121">Now that you have registered your application with Azure Active Directory (Azure AD), you can connect the React app to Microsoft 365.</span></span> <span data-ttu-id="1fdf6-122">Primeiro, permita que os usuários entre no aplicativo usando sua conta da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="1fdf6-122">First, allow users to sign in to the app using their Microsoft account.</span></span>

### <a name="copy-the-azure-ad-application-registration-id"></a><span data-ttu-id="1fdf6-123">Copiar a ID de registro do aplicativo do Azure AD</span><span class="sxs-lookup"><span data-stu-id="1fdf6-123">Copy the Azure AD application registration ID</span></span>

1. <span data-ttu-id="1fdf6-124">No Portal do Azure, acesse o registro do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1fdf6-124">In the Azure Portal, go to your application registration.</span></span>
1. <span data-ttu-id="1fdf6-125">Verifique se você está na página **Visão** Geral.</span><span class="sxs-lookup"><span data-stu-id="1fdf6-125">Verify that you are on the **Overview** page.</span></span>
1. <span data-ttu-id="1fdf6-126">Na seção **Essentials,** copie o valor da propriedade **Application (client) ID**</span><span class="sxs-lookup"><span data-stu-id="1fdf6-126">From the **Essentials** section, copy the value of the **Application (client) ID** property</span></span>

### <a name="configure-the-microsoft-graph-toolkit-authentication-provider"></a><span data-ttu-id="1fdf6-127">Configurar o provedor de autenticação Graph Toolkit Microsoft</span><span class="sxs-lookup"><span data-stu-id="1fdf6-127">Configure the Microsoft Graph Toolkit authentication provider</span></span>

<span data-ttu-id="1fdf6-128">Em seguida, configure o provedor de autenticação que o microsoft Graph Toolkit deve usar.</span><span class="sxs-lookup"><span data-stu-id="1fdf6-128">Next, configure the authentication provider that the Microsoft Graph Toolkit should use.</span></span> <span data-ttu-id="1fdf6-129">Nesse caso, você usará o MSAL, que é um bom padrão para a criação de aplicativos autônomos.</span><span class="sxs-lookup"><span data-stu-id="1fdf6-129">In this case, you'll use MSAL, which is a good default for building standalone applications.</span></span> <span data-ttu-id="1fdf6-130">Se você usar qualquer um dos pontos de extensibilidade no Microsoft 365, como Teams ou SharePoint, você usará [outros provedores](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="1fdf6-130">If you use any of the extensibility points in Microsoft 365, like Teams or SharePoint, you will use [other providers](../providers/providers.md).</span></span>

>[!NOTE] 
><span data-ttu-id="1fdf6-131">Se você estiver usando o Provedor MSAL no momento e quiser atualizar para o Provedor MSAL 2, siga as etapas no artigo do provedor [MSAL 2.](../providers/msal2.md#migrating-from-msal-provider-to-msal-2-provider)</span><span class="sxs-lookup"><span data-stu-id="1fdf6-131">If you are currently using MSAL Provider and would like to update to the MSAL 2 Provider, follow the steps in the [MSAL 2 provider](../providers/msal2.md#migrating-from-msal-provider-to-msal-2-provider) article.</span></span>

1. <span data-ttu-id="1fdf6-132">No editor de código, abra **o src/index.**</span><span class="sxs-lookup"><span data-stu-id="1fdf6-132">In the code editor, open the **src/index.**</span></span> <span data-ttu-id="1fdf6-133">e à lista de importações, adicione:</span><span class="sxs-lookup"><span data-stu-id="1fdf6-133">file, and to the list of imports, add:</span></span>

    ```tsx
    import { Providers } from '@microsoft/mgt-element';
    import { Msal2Provider } from '@microsoft/mgt-msal2-provider';
    ```

1. <span data-ttu-id="1fdf6-134">Após a última `import` instrução, inicialize o microsoft Graph Toolkit com o provedor MSAL.</span><span class="sxs-lookup"><span data-stu-id="1fdf6-134">After the last `import` statement, initialize the Microsoft Graph Toolkit with MSAL provider.</span></span>

    ```tsx
    Providers.globalProvider = new Msal2Provider({
      clientId: 'REPLACE_WITH_CLIENTID'
    });
    ```

    <span data-ttu-id="1fdf6-135">Substitua o valor da propriedade pelo valor da propriedade copiada `clientId` `Application (client) ID` anteriormente no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="1fdf6-135">Replace the value of the `clientId` property with the value of the `Application (client) ID` property you copied previously in the Azure Portal.</span></span>

<span data-ttu-id="1fdf6-136">Com essas alterações, o **arquivo src/index.tsx** terá a seguinte aparência.</span><span class="sxs-lookup"><span data-stu-id="1fdf6-136">With these changes, the **src/index.tsx** file will look like the following.</span></span>

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

### <a name="add-the-sign-in-button"></a><span data-ttu-id="1fdf6-137">Adicionar o botão Entrar</span><span class="sxs-lookup"><span data-stu-id="1fdf6-137">Add the Sign in button</span></span>

<span data-ttu-id="1fdf6-138">Adicione o **componente Logon** do Microsoft Graph Toolkit React, que exibirá o botão Entrar que as pessoas podem usar para entrar com sua conta da Microsoft em seu aplicativo. </span><span class="sxs-lookup"><span data-stu-id="1fdf6-138">Add the **Login** Microsoft Graph Toolkit React component, which will display the **Sign in** button people can use to sign in with their Microsoft account to your app.</span></span>

1. <span data-ttu-id="1fdf6-139">No editor de código, abra o **arquivo src/App.tsx** e, na lista de importações, adicione:</span><span class="sxs-lookup"><span data-stu-id="1fdf6-139">In the code editor, open the **src/App.tsx** file, and to the list of imports add:</span></span>

    ```tsx
    import { Login } from '@microsoft/mgt-react';
    ```

1. <span data-ttu-id="1fdf6-140">Na `App` função, substitua o conteúdo da cláusula pela estrutura básica, incluindo o componente Graph Toolkit `return` Logon da Microsoft:</span><span class="sxs-lookup"><span data-stu-id="1fdf6-140">In the `App` function, replace the contents of the `return` clause with the basic structure including the Microsoft Graph Toolkit Login component:</span></span>

    ```tsx
    <div className="App">
      <header>
        <Login />
      </header>
    </div>
    ```

<span data-ttu-id="1fdf6-141">Com essas alterações, o **arquivo src/App.tsx** terá a seguinte aparência.</span><span class="sxs-lookup"><span data-stu-id="1fdf6-141">With these changes, the **src/App.tsx** file will look like the following.</span></span>
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

### <a name="test-signing-in-to-your-application"></a><span data-ttu-id="1fdf6-142">Testar o registro no aplicativo</span><span class="sxs-lookup"><span data-stu-id="1fdf6-142">Test signing in to your application</span></span>

<span data-ttu-id="1fdf6-143">Agora você deve poder entrar no aplicativo com sua conta da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="1fdf6-143">You should now be able to sign in to your application with your Microsoft account.</span></span>

1. <span data-ttu-id="1fdf6-144">Volte para o navegador onde seu aplicativo React está sendo executado.</span><span class="sxs-lookup"><span data-stu-id="1fdf6-144">Go back to the browser where your React app is running.</span></span> <span data-ttu-id="1fdf6-145">Agora você deve ver um **botão Entrar.**</span><span class="sxs-lookup"><span data-stu-id="1fdf6-145">You should now see a **Sign in** button.</span></span>
1. <span data-ttu-id="1fdf6-146">Ao clicar  no botão Entrar, você será solicitado a entrar com sua conta da Microsoft (você pode usar a mesma conta com a qual você acessou o Portal do Azure).</span><span class="sxs-lookup"><span data-stu-id="1fdf6-146">When you click the **Sign in** button, you will be prompted to sign in with your Microsoft account (you can use the same account as the one you accessed the Azure Portal with).</span></span>
1. <span data-ttu-id="1fdf6-147">Como esta é a primeira vez que você está usando esse aplicativo do Azure AD, você precisa consentir seu uso em sua organização.</span><span class="sxs-lookup"><span data-stu-id="1fdf6-147">Because this is the first time you're using this Azure AD application, you need to consent its use in your organization.</span></span>
1. <span data-ttu-id="1fdf6-148">Depois de entrar, você será redirecionado para seu React app.</span><span class="sxs-lookup"><span data-stu-id="1fdf6-148">After signing in, you will be redirected to your React app.</span></span> <span data-ttu-id="1fdf6-149">Observe que o **botão** Entrar foi alterado para mostrar o nome do usuário React aplicativo mostrando informações do usuário recuperadas do Microsoft 365 usando o ![ Microsoft Graph Toolkit ](../images/mgt-react-userinfo.png) .</span><span class="sxs-lookup"><span data-stu-id="1fdf6-149">Notice that the **Sign in** button changed to show your user's name ![React app showing user info retrieved from Microsoft 365 using Microsoft Graph Toolkit](../images/mgt-react-userinfo.png).</span></span>

## <a name="load-data-from-microsoft-365"></a><span data-ttu-id="1fdf6-150">Carregar dados de Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="1fdf6-150">Load data from Microsoft 365</span></span>

<span data-ttu-id="1fdf6-151">A Microsoft Graph Toolkit simplifica a autenticação para Microsoft 365, mas também carrega seus dados.</span><span class="sxs-lookup"><span data-stu-id="1fdf6-151">Microsoft Graph Toolkit not only simplifies authentication to Microsoft 365, but also loading its data.</span></span> <span data-ttu-id="1fdf6-152">Neste exemplo, você mostrará o calendário da pessoa assinada.</span><span class="sxs-lookup"><span data-stu-id="1fdf6-152">In this example, you'll show the signed in person's calendar.</span></span>

### <a name="specify-permissions-needed-for-your-application"></a><span data-ttu-id="1fdf6-153">Especificar permissões necessárias para seu aplicativo</span><span class="sxs-lookup"><span data-stu-id="1fdf6-153">Specify permissions needed for your application</span></span>

<span data-ttu-id="1fdf6-154">Antes de carregar dados Microsoft 365, você precisa especificar a lista de escopos de permissão que seu aplicativo deve ter para acessar os dados do usuário.</span><span class="sxs-lookup"><span data-stu-id="1fdf6-154">Before you can load data from Microsoft 365, you need to specify the list of permission scopes your application must be granted to access user's data.</span></span> <span data-ttu-id="1fdf6-155">Esses escopos diferem dependendo do tipo de informação que você deseja mostrar.</span><span class="sxs-lookup"><span data-stu-id="1fdf6-155">These scopes differ depending on what kind of information you want to show.</span></span> <span data-ttu-id="1fdf6-156">Nesse caso, você precisará de acesso ao calendário das pessoas, bem como acesso básico a informações sobre pessoas que também são exibidas no calendário.</span><span class="sxs-lookup"><span data-stu-id="1fdf6-156">In this case, you will need access to people's calendar as well as basic access to information about people that is also displayed in the calendar.</span></span> <span data-ttu-id="1fdf6-157">Você pode encontrar os escopos exigidos por cada API na documentação da [API Graph Microsoft.](/graph/api/overview)</span><span class="sxs-lookup"><span data-stu-id="1fdf6-157">You can find the scopes required by each API in the [Microsoft Graph API documentation](/graph/api/overview).</span></span>

1. <span data-ttu-id="1fdf6-158">No editor de código, abra o **arquivo src/index.tsx** e atualize o código de inicialização do provedor.</span><span class="sxs-lookup"><span data-stu-id="1fdf6-158">In the code editor, open the **src/index.tsx** file, and update the provider initialization code.</span></span>

    ```tsx
    Providers.globalProvider = new Msal2Provider({
      clientId: 'REPLACE_WITH_CLIENTID',
      scopes: ['calendars.read', 'user.read', 'openid', 'profile', 'people.read', 'user.readbasic.all']
    });
    ```

### <a name="show-users-data-after-signing-in"></a><span data-ttu-id="1fdf6-159">Mostrar dados do usuário após entrar</span><span class="sxs-lookup"><span data-stu-id="1fdf6-159">Show user's data after signing in</span></span>

<span data-ttu-id="1fdf6-160">Em seguida, estenda o aplicativo para mostrar dados do calendário do usuário.</span><span class="sxs-lookup"><span data-stu-id="1fdf6-160">Next, extend the application to show data from the user's calendar.</span></span> <span data-ttu-id="1fdf6-161">Você só pode acessar essas informações depois que o usuário entrar.</span><span class="sxs-lookup"><span data-stu-id="1fdf6-161">You can access this information only after the user has signed in.</span></span> <span data-ttu-id="1fdf6-162">Para fazer isso, você precisará rastrear o estado de login do usuário e mostrar os dados do calendário depois que o usuário tiver se assinado com sua conta da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="1fdf6-162">To do this, you will need to track the  user's sign in state and show the calendar data after the user has signed in with their Microsoft account.</span></span>

#### <a name="track-users-sign-in-state"></a><span data-ttu-id="1fdf6-163">Controlar o estado de login do usuário</span><span class="sxs-lookup"><span data-stu-id="1fdf6-163">Track user's sign in state</span></span>

<span data-ttu-id="1fdf6-164">Para rastrear o estado de login do usuário em seu aplicativo, você usará o React e os ganchos em combinação com manipuladores de eventos `useState` `useEffect` do provedor.</span><span class="sxs-lookup"><span data-stu-id="1fdf6-164">To track the user's sign in state in your application, you will use the React `useState` and `useEffect` hooks in combination with provider event handlers.</span></span>

1. <span data-ttu-id="1fdf6-165">No editor de código, abra o **arquivo src/App.tsx** e estenda a instrução React `import` existente.</span><span class="sxs-lookup"><span data-stu-id="1fdf6-165">In the code editor, open the **src/App.tsx** file and extend the existing React `import` statement.</span></span>

    ```tsx
    import React, { useState, useEffect } from 'react';
    ```

1. <span data-ttu-id="1fdf6-166">Importe os `Provider` tipos e de , `ProviderState` `mgt-element` adicionando a importações.</span><span class="sxs-lookup"><span data-stu-id="1fdf6-166">Import the `Provider` and `ProviderState` types from `mgt-element`, by adding to imports.</span></span>

    ```tsx
    import { Providers, ProviderState } from '@microsoft/mgt-element';
    ```

1. <span data-ttu-id="1fdf6-167">Adicione uma função personalizada chamada que permite controlar o estado de login do `useIsSignedIn` usuário em seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1fdf6-167">Add a custom function named `useIsSignedIn` that enables tracking the user's sign in state in your application.</span></span>

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

<span data-ttu-id="1fdf6-168">Essa função faz duas coisas.</span><span class="sxs-lookup"><span data-stu-id="1fdf6-168">This function does two things.</span></span> <span data-ttu-id="1fdf6-169">Primeiro, usando o `useState` React, ele habilita o estado de controle dentro do componente.</span><span class="sxs-lookup"><span data-stu-id="1fdf6-169">First, using the React `useState` hook, it enables tracking state inside your component.</span></span> <span data-ttu-id="1fdf6-170">Sempre que o estado mudar, React renderizará seu componente.</span><span class="sxs-lookup"><span data-stu-id="1fdf6-170">Whenever the state changes, React will re-render your component.</span></span> <span data-ttu-id="1fdf6-171">Em segundo lugar, usando o React, ele estende o ciclo de vida do componente rastreando as alterações no provedor Graph Toolkit Microsoft e atualizando o componente, se `useEffect` necessário.</span><span class="sxs-lookup"><span data-stu-id="1fdf6-171">Second, using the React `useEffect` hook, it extends the component's lifecycle by tracking changes in the Microsoft Graph Toolkit provider and updating the component if necessary.</span></span>

#### <a name="load-users-calendar-if-user-is-signed-in"></a><span data-ttu-id="1fdf6-172">Carregar o calendário do usuário se o usuário estiver assinado</span><span class="sxs-lookup"><span data-stu-id="1fdf6-172">Load user's calendar if user is signed in</span></span>

<span data-ttu-id="1fdf6-173">Agora que você rastreia o estado de login do usuário em seu aplicativo, você pode mostrar seu calendário depois de entrar.</span><span class="sxs-lookup"><span data-stu-id="1fdf6-173">Now that you track the user's sign in state in your application, you can show their calendar after they signed in.</span></span>

1. <span data-ttu-id="1fdf6-174">No editor de código, abra o **arquivo src/App.tsx** e, dentro da função **App,** adicione:</span><span class="sxs-lookup"><span data-stu-id="1fdf6-174">In the code editor, open the **src/App.tsx** file, and inside the **App** function, add:</span></span>

    ```tsx
    const [isSignedIn] = useIsSignedIn();
    ```

    <span data-ttu-id="1fdf6-175">Isso define uma constante Boolean, que você pode usar para determinar se o usuário está atualmente `isSignedIn` dentro do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1fdf6-175">This defines a Boolean `isSignedIn` constant, which you can use to determine whether the user is currently signed in to your application.</span></span>

1. <span data-ttu-id="1fdf6-176">Estenda o conteúdo da cláusula com um componente de Agenda Graph Toolkit `return` `div` Microsoft.</span><span class="sxs-lookup"><span data-stu-id="1fdf6-176">Extend the contents of the `return` clause with an additional `div` and the Microsoft Graph Toolkit Agenda component.</span></span>

    ```tsx
    <div>
      {isSignedIn &&
        <Agenda />}
    </div>
    ```

<span data-ttu-id="1fdf6-177">Com essas alterações, o **arquivo src/App.tsx** deve ter a seguinte aparência.</span><span class="sxs-lookup"><span data-stu-id="1fdf6-177">With these changes, the **src/App.tsx** file should look like the following.</span></span>

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

### <a name="test-showing-users-calendar-after-they-signed-in"></a><span data-ttu-id="1fdf6-178">Testar mostrando o calendário do usuário depois que ele se inscreveu</span><span class="sxs-lookup"><span data-stu-id="1fdf6-178">Test showing user's calendar after they signed in</span></span>

<span data-ttu-id="1fdf6-179">Com essas alterações, depois de entrar no aplicativo com sua conta da Microsoft, você deverá ver seu calendário.</span><span class="sxs-lookup"><span data-stu-id="1fdf6-179">With these changes, after signing in to your application with your Microsoft account, you should see your calendar.</span></span>

1. <span data-ttu-id="1fdf6-180">Para ver as alterações, feche o navegador e abra-o novamente e vá para `http://localhost:3000` .</span><span class="sxs-lookup"><span data-stu-id="1fdf6-180">To see the changes, close the browser and open it again, and go to `http://localhost:3000`.</span></span> <span data-ttu-id="1fdf6-181">Faça isso porque alterou o valor da propriedade, o que afeta o token de acesso solicitado `scopes` pelo Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1fdf6-181">You do this because you changed the value of the `scopes` property, which affects the access token that you request from Azure AD.</span></span>
1. <span data-ttu-id="1fdf6-182">Escolha o **botão Entrar** e entre usando sua conta da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="1fdf6-182">Choose the **Sign In** button and sign in using your Microsoft account.</span></span> <span data-ttu-id="1fdf6-183">Observe as adições à lista de permissões solicitadas no prompt de consentimento.</span><span class="sxs-lookup"><span data-stu-id="1fdf6-183">Notice the additions to the list of permissions requested in the consent prompt.</span></span> <span data-ttu-id="1fdf6-184">Isso porque você incluiu permissões adicionais na `scope` propriedade.</span><span class="sxs-lookup"><span data-stu-id="1fdf6-184">This is because you included additional permissions in the `scope` property.</span></span>
1. <span data-ttu-id="1fdf6-185">Depois de concordar com o uso do aplicativo, você deverá ver informações sobre o usuário atual e seu calendário.</span><span class="sxs-lookup"><span data-stu-id="1fdf6-185">After consenting to the use of the application, you should see information about the current user and their calendar.</span></span>

![Aplicativo concluído](../images/mgt-finished-app.png)

## <a name="next-steps"></a><span data-ttu-id="1fdf6-187">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="1fdf6-187">Next steps</span></span>

- <span data-ttu-id="1fdf6-188">Veja [o que está no microsoft Graph Toolkit](../overview.md).</span><span class="sxs-lookup"><span data-stu-id="1fdf6-188">See [what's in the Microsoft Graph Toolkit](../overview.md).</span></span>
- <span data-ttu-id="1fdf6-189">Experimente os componentes no [playground](https://mgt.dev).</span><span class="sxs-lookup"><span data-stu-id="1fdf6-189">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="1fdf6-190">Faça uma pergunta sobre [Stack Overflow](https://aka.ms/mgt-question).</span><span class="sxs-lookup"><span data-stu-id="1fdf6-190">Ask a question on [Stack Overflow](https://aka.ms/mgt-question).</span></span>
- <span data-ttu-id="1fdf6-191">Relatar bugs ou deixar uma solicitação de recurso [GitHub](https://aka.ms/mgt).</span><span class="sxs-lookup"><span data-stu-id="1fdf6-191">Report bugs or leave a feature request on [GitHub](https://aka.ms/mgt).</span></span>
