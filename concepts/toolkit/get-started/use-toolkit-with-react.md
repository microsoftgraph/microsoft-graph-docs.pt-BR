---
title: Use o kit de ferramentas do Microsoft Graph com reagir
description: Introdução ao uso do kit de ferramentas do Microsoft Graph em um aplicativo reagir.
localization_priority: Normal
author: waldekmastykarz
ms.openlocfilehash: 57e9901c8b7ee1f8a5474f21ff4b09def053e7db
ms.sourcegitcommit: 7902607a1e5a030d46e907d08e16644a47a47006
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/12/2020
ms.locfileid: "49664132"
---
# <a name="use-the-microsoft-graph-toolkit-with-react"></a><span data-ttu-id="c6699-103">Use o kit de ferramentas do Microsoft Graph com reagir</span><span class="sxs-lookup"><span data-stu-id="c6699-103">Use the Microsoft Graph Toolkit with React</span></span>

<span data-ttu-id="c6699-104">O Microsoft Graph Toolkit é um conjunto de componentes Web que simplifica a conexão com o Microsoft Graph e permite que você se concentre em seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c6699-104">Microsoft Graph Toolkit is a set of web components that simplify connecting to Microsoft Graph and allow you to focus on your application instead.</span></span> <span data-ttu-id="c6699-105">O Microsoft Graph Toolkit está disponível como um conjunto genérico de componentes Web distribuídos por meio do `@microsoft/mgt` pacote do NPM.</span><span class="sxs-lookup"><span data-stu-id="c6699-105">Microsoft Graph Toolkit is available as a generic set of web components distributed through the `@microsoft/mgt` npm package.</span></span>

<span data-ttu-id="c6699-106">Se você estiver criando aplicativos com reagir, poderá usar o [ `@microsoft/mgt-react` pacote](./mgt-react.md), que encapsula o Microsoft Graph Toolkit Web Components em reagir componentes e facilita a passagem de dados complexos.</span><span class="sxs-lookup"><span data-stu-id="c6699-106">If you're building apps with React, you can use the [`@microsoft/mgt-react` package](./mgt-react.md), which wraps Microsoft Graph Toolkit web components in React components and makes it easier to pass complex data.</span></span>

<span data-ttu-id="c6699-107">Este artigo descreve o processo passo a passo de usar o kit de ferramentas do Microsoft Graph para criar um aplicativo reagir e conectá-lo ao Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="c6699-107">This article describes the step-by-step process of using the Microsoft Graph Toolkit to create a React app and connect it to Microsoft 365.</span></span> <span data-ttu-id="c6699-108">Após concluir as etapas, você terá um aplicativo reagir que mostra os futuros compromissos do usuário conectado no momento da Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="c6699-108">After completing the steps, you'll have a React app that shows the upcoming appointments of the currently signed in user from Microsoft 365.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c6699-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c6699-109">Prerequisites</span></span>

<span data-ttu-id="c6699-110">Para seguir as etapas deste artigo, você precisará de um ambiente de desenvolvimento do Microsoft 365 e de algumas ferramentas.</span><span class="sxs-lookup"><span data-stu-id="c6699-110">To follow the steps in this article, you'll need a Microsoft 365 development environment and a few tools.</span></span> <span data-ttu-id="c6699-111">Para obter detalhes, consulte [introdução](./overview.md).</span><span class="sxs-lookup"><span data-stu-id="c6699-111">For details, see [getting started](./overview.md).</span></span>

## <a name="create-a-react-app"></a><span data-ttu-id="c6699-112">Criar um aplicativo reagir</span><span class="sxs-lookup"><span data-stu-id="c6699-112">Create a React app</span></span>

<span data-ttu-id="c6699-113">Crie um novo aplicativo reagir executando o seguinte comando.</span><span class="sxs-lookup"><span data-stu-id="c6699-113">Create a new React app by running the following command.</span></span> <span data-ttu-id="c6699-114">Isso criará um novo aplicativo reagir usando TypeScript, que o ajudará a escrever código mais robusto e evitar erros de tempo de execução.</span><span class="sxs-lookup"><span data-stu-id="c6699-114">This will create a new React app using TypeScript, which will help you write more robust code and avoid runtime errors.</span></span>

```cmd
npx create-react-app my-m365-app --template typescript
```

<span data-ttu-id="c6699-115">Altere o diretório de trabalho para o aplicativo recém-criado.</span><span class="sxs-lookup"><span data-stu-id="c6699-115">Change the working directory to the newly created app.</span></span>

```cmd
cd my-m365-app
```

<span data-ttu-id="c6699-116">Em seguida, instale o `mgt-react` pacote NPM, que contém os componentes de reagir do Microsoft Graph Toolkit.</span><span class="sxs-lookup"><span data-stu-id="c6699-116">Next, install the `mgt-react` npm package, which contains the Microsoft Graph Toolkit React components.</span></span>

```cmd
npm i @microsoft/mgt-react
```

<span data-ttu-id="c6699-117">Instale o `mgt-msal-provider` pacote e o `mgt-element` NPM também, que contém o provedor de autenticação do MSAL.</span><span class="sxs-lookup"><span data-stu-id="c6699-117">Install the `mgt-msal-provider` and `mgt-element` npm package as well, which contains the MSAL auth provider.</span></span>

```cmd
npm i @microsoft/mgt-element @microsoft/mgt-msal-provider
```

<span data-ttu-id="c6699-118">Confirme que você pode executar o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c6699-118">Confirm that you can run the app.</span></span>

```cmd
npm start
```

<span data-ttu-id="c6699-119">Você deve ser capaz de abrir seu aplicativo no navegador via `http://localhost:3000` .</span><span class="sxs-lookup"><span data-stu-id="c6699-119">You should be able to open your app in the browser via `http://localhost:3000`.</span></span>

[!INCLUDE [AAD with implicit flow app registration](../includes/aad-app-registration-spa.md)]

## <a name="connect-react-app-to-microsoft-365"></a><span data-ttu-id="c6699-120">Conectar aplicativo reagir ao Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="c6699-120">Connect React app to Microsoft 365</span></span>

<span data-ttu-id="c6699-121">Agora que você registrou seu aplicativo com o Azure Active Directory (Azure AD), você pode conectar o aplicativo reagir ao Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="c6699-121">Now that you have registered your application with Azure Active Directory (Azure AD), you can connect the React app to Microsoft 365.</span></span> <span data-ttu-id="c6699-122">Primeiro, permita que os usuários entrem no aplicativo usando sua conta da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c6699-122">First, allow users to sign in to the app using their Microsoft account.</span></span>

### <a name="copy-the-azure-ad-application-registration-id"></a><span data-ttu-id="c6699-123">Copiar a ID de registro do aplicativo do Azure AD</span><span class="sxs-lookup"><span data-stu-id="c6699-123">Copy the Azure AD application registration ID</span></span>

1. <span data-ttu-id="c6699-124">No portal do Azure, vá para o registro do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c6699-124">In the Azure Portal, go to your application registration.</span></span>
1. <span data-ttu-id="c6699-125">Verifique se você está na página de **visão geral** .</span><span class="sxs-lookup"><span data-stu-id="c6699-125">Verify that you are on the **Overview** page.</span></span>
1. <span data-ttu-id="c6699-126">Na seção **Essentials** , copie o valor da propriedade **ID do aplicativo (cliente)**</span><span class="sxs-lookup"><span data-stu-id="c6699-126">From the **Essentials** section, copy the value of the **Application (client) ID** property</span></span>

### <a name="configure-the-microsoft-graph-toolkit-authentication-provider"></a><span data-ttu-id="c6699-127">Configurar o provedor de autenticação do kit de ferramentas do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="c6699-127">Configure the Microsoft Graph Toolkit authentication provider</span></span>

<span data-ttu-id="c6699-128">Em seguida, configure o provedor de autenticação que o Microsoft Graph Toolkit deve usar.</span><span class="sxs-lookup"><span data-stu-id="c6699-128">Next, configure the authentication provider that the Microsoft Graph Toolkit should use.</span></span> <span data-ttu-id="c6699-129">Nesse caso, você usará o MSAL, que é um bom padrão para criar aplicativos autônomos.</span><span class="sxs-lookup"><span data-stu-id="c6699-129">In this case, you'll use MSAL, which is a good default for building standalone applications.</span></span> <span data-ttu-id="c6699-130">Se você usar qualquer um dos pontos de extensibilidade no Microsoft 365, como o Teams ou o SharePoint, você usará [outros provedores](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="c6699-130">If you use any of the extensibility points in Microsoft 365, like Teams or SharePoint, you will use [other providers](../providers/providers.md).</span></span>

1. <span data-ttu-id="c6699-131">No editor de código, abra **src/index.**</span><span class="sxs-lookup"><span data-stu-id="c6699-131">In the code editor, open the **src/index.**</span></span> <span data-ttu-id="c6699-132">e, na lista de importações, adicione:</span><span class="sxs-lookup"><span data-stu-id="c6699-132">file, and to the list of imports, add:</span></span>

    ```tsx
    import { Providers } from '@microsoft/mgt-element';
    import { MsalProvider } from '@microsoft/mgt-msal-provider';
    ```

1. <span data-ttu-id="c6699-133">Após a última `import` instrução, inicialize o Microsoft Graph Toolkit com o provedor MSAL.</span><span class="sxs-lookup"><span data-stu-id="c6699-133">After the last `import` statement, initialize the Microsoft Graph Toolkit with MSAL provider.</span></span>

    ```tsx
    Providers.globalProvider = new MsalProvider({
      clientId: 'REPLACE_WITH_CLIENTID'
    });
    ```

    <span data-ttu-id="c6699-134">Substitua o valor da `clientId` propriedade com o valor da `Application (client) ID` propriedade que você copiou anteriormente no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="c6699-134">Replace the value of the `clientId` property with the value of the `Application (client) ID` property you copied previously in the Azure Portal.</span></span>

<span data-ttu-id="c6699-135">Com essas alterações, o arquivo **src/index. TSX** será semelhante ao seguinte.</span><span class="sxs-lookup"><span data-stu-id="c6699-135">With these changes, the **src/index.tsx** file will look like the following.</span></span>

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

### <a name="add-the-sign-in-button"></a><span data-ttu-id="c6699-136">Adicionar o botão entrar</span><span class="sxs-lookup"><span data-stu-id="c6699-136">Add the Sign in button</span></span>

<span data-ttu-id="c6699-137">Adicione o componente de **logon** do Microsoft Graph Toolkit para reagir, que exibirá o botão de **entrada** que as pessoas podem usar para entrar com sua conta da Microsoft em seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c6699-137">Add the **Login** Microsoft Graph Toolkit React component, which will display the **Sign in** button people can use to sign in with their Microsoft account to your app.</span></span>

1. <span data-ttu-id="c6699-138">No editor de códigos, abra o arquivo **src/app. TSX** e, na lista de importações, adicione:</span><span class="sxs-lookup"><span data-stu-id="c6699-138">In the code editor, open the **src/App.tsx** file, and to the list of imports add:</span></span>

    ```tsx
    import { Login } from '@microsoft/mgt-react';
    ```

1. <span data-ttu-id="c6699-139">Na `App` função, substitua o conteúdo da `return` cláusula pela estrutura básica, incluindo o componente de logon do Microsoft Graph Toolkit:</span><span class="sxs-lookup"><span data-stu-id="c6699-139">In the `App` function, replace the contents of the `return` clause with the basic structure including the Microsoft Graph Toolkit Login component:</span></span>

    ```tsx
    <div className="App">
      <header>
        <Login />
      </header>
    </div>
    ```

<span data-ttu-id="c6699-140">Com essas alterações, o arquivo **src/app. TSX** será semelhante ao seguinte.</span><span class="sxs-lookup"><span data-stu-id="c6699-140">With these changes, the **src/App.tsx** file will look like the following.</span></span>
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

### <a name="test-signing-in-to-your-application"></a><span data-ttu-id="c6699-141">Testar sessão no seu aplicativo</span><span class="sxs-lookup"><span data-stu-id="c6699-141">Test signing in to your application</span></span>

<span data-ttu-id="c6699-142">Agora você poderá entrar no seu aplicativo com sua conta da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c6699-142">You should now be able to sign in to your application with your Microsoft account.</span></span>

1. <span data-ttu-id="c6699-143">Volte para o navegador onde seu aplicativo reagir está em execução.</span><span class="sxs-lookup"><span data-stu-id="c6699-143">Go back to the browser where your React app is running.</span></span> <span data-ttu-id="c6699-144">Agora você deve ver um botão **entrar** .</span><span class="sxs-lookup"><span data-stu-id="c6699-144">You should now see a **Sign in** button.</span></span>
1. <span data-ttu-id="c6699-145">Ao clicar no botão **entrar** , você será solicitado a entrar com sua conta da Microsoft (você pode usar a mesma conta que você acessou o portal do Azure).</span><span class="sxs-lookup"><span data-stu-id="c6699-145">When you click the **Sign in** button, you will be prompted to sign in with your Microsoft account (you can use the same account as the one you accessed the Azure Portal with).</span></span>
1. <span data-ttu-id="c6699-146">Como esta é a primeira vez que você está usando esse aplicativo do Azure AD, você precisa consentir seu uso na sua organização.</span><span class="sxs-lookup"><span data-stu-id="c6699-146">Because this is the first time you're using this Azure AD application, you need to consent its use in your organization.</span></span>
1. <span data-ttu-id="c6699-147">Após entrar, você será redirecionado para seu aplicativo reagir.</span><span class="sxs-lookup"><span data-stu-id="c6699-147">After signing in, you will be redirected to your React app.</span></span> <span data-ttu-id="c6699-148">Observe que o botão **entrar** foi alterado para mostrar o nome do seu usuário ![ aplicativo reagir mostrando as informações do usuário recuperadas do Microsoft 365 usando o Microsoft Graph Toolkit ](../images/mgt-react-userinfo.png) .</span><span class="sxs-lookup"><span data-stu-id="c6699-148">Notice that the **Sign in** button changed to show your user's name ![React app showing user info retrieved from Microsoft 365 using Microsoft Graph Toolkit](../images/mgt-react-userinfo.png).</span></span>

## <a name="load-data-from-microsoft-365"></a><span data-ttu-id="c6699-149">Carregar dados do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="c6699-149">Load data from Microsoft 365</span></span>

<span data-ttu-id="c6699-150">O Microsoft Graph Toolkit não apenas simplifica a autenticação para o Microsoft 365, mas também o carregamento dos dados.</span><span class="sxs-lookup"><span data-stu-id="c6699-150">Microsoft Graph Toolkit not only simplifies authentication to Microsoft 365, but also loading its data.</span></span> <span data-ttu-id="c6699-151">Neste exemplo, você mostrará o calendário do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="c6699-151">In this example, you'll show the signed in person's calendar.</span></span>

### <a name="specify-permissions-needed-for-your-application"></a><span data-ttu-id="c6699-152">Especificar permissões necessárias para seu aplicativo</span><span class="sxs-lookup"><span data-stu-id="c6699-152">Specify permissions needed for your application</span></span>

<span data-ttu-id="c6699-153">Antes de poder carregar dados do Microsoft 365, você precisa especificar a lista de escopos de permissão que seu aplicativo deve ser concedido para acessar os dados do usuário.</span><span class="sxs-lookup"><span data-stu-id="c6699-153">Before you can load data from Microsoft 365, you need to specify the list of permission scopes your application must be granted to access user's data.</span></span> <span data-ttu-id="c6699-154">Esses escopos diferem, dependendo do tipo de informação que você deseja exibir.</span><span class="sxs-lookup"><span data-stu-id="c6699-154">These scopes differ depending on what kind of information you want to show.</span></span> <span data-ttu-id="c6699-155">Nesse caso, você precisará acessar o calendário de pessoas e o acesso básico às informações sobre as pessoas que também são exibidas no calendário.</span><span class="sxs-lookup"><span data-stu-id="c6699-155">In this case, you will need access to people's calendar as well as basic access to information about people that is also displayed in the calendar.</span></span> <span data-ttu-id="c6699-156">Você pode encontrar os escopos exigidos por cada API na [documentação da API do Microsoft Graph](/graph/api/overview).</span><span class="sxs-lookup"><span data-stu-id="c6699-156">You can find the scopes required by each API in the [Microsoft Graph API documentation](/graph/api/overview).</span></span>

1. <span data-ttu-id="c6699-157">No editor de códigos, abra o arquivo **src/index. TSX** e atualize o código de inicialização do provedor.</span><span class="sxs-lookup"><span data-stu-id="c6699-157">In the code editor, open the **src/index.tsx** file, and update the provider initialization code.</span></span>

    ```tsx
    Providers.globalProvider = new MsalProvider({
      clientId: 'd7cb93c9-9097-4e38-8f06-7c0088ac3318',
      scopes: ['calendars.read', 'user.read', 'openid', 'profile', 'people.read', 'user.readbasic.all']
    });
    ```

### <a name="show-users-data-after-signing-in"></a><span data-ttu-id="c6699-158">Mostrar dados do usuário após entrar</span><span class="sxs-lookup"><span data-stu-id="c6699-158">Show user's data after signing in</span></span>

<span data-ttu-id="c6699-159">Em seguida, estenda o aplicativo para mostrar os dados do calendário do usuário.</span><span class="sxs-lookup"><span data-stu-id="c6699-159">Next, extend the application to show data from the user's calendar.</span></span> <span data-ttu-id="c6699-160">Você pode acessar essas informações somente depois que o usuário entrar.</span><span class="sxs-lookup"><span data-stu-id="c6699-160">You can access this information only after the user has signed in.</span></span> <span data-ttu-id="c6699-161">Para fazer isso, você precisará controlar o estado de entrada do usuário e mostrar os dados do calendário depois que o usuário entrar com a conta da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c6699-161">To do this, you will need to track the  user's sign in state and show the calendar data after the user has signed in with their Microsoft account.</span></span>

#### <a name="track-users-sign-in-state"></a><span data-ttu-id="c6699-162">Rastrear o estado de entrada do usuário</span><span class="sxs-lookup"><span data-stu-id="c6699-162">Track user's sign in state</span></span>

<span data-ttu-id="c6699-163">Para acompanhar o estado de entrada do usuário em seu aplicativo, você usará a combinação de reagir `useState` e `useEffect` conexões com os manipuladores de eventos do provedor.</span><span class="sxs-lookup"><span data-stu-id="c6699-163">To track the user's sign in state in your application, you will use the React `useState` and `useEffect` hooks in combination with provider event handlers.</span></span>

1. <span data-ttu-id="c6699-164">No editor de códigos, abra o arquivo **src/app. TSX** e estenda a instrução de reagir existente `import` .</span><span class="sxs-lookup"><span data-stu-id="c6699-164">In the code editor, open the **src/App.tsx** file and extend the existing React `import` statement.</span></span>

    ```tsx
    import React, { useState, useEffect } from 'react';
    ```

1. <span data-ttu-id="c6699-165">Importar os `Provider` `ProviderState` tipos e de `mgt-element` , adicionando às importações.</span><span class="sxs-lookup"><span data-stu-id="c6699-165">Import the `Provider` and `ProviderState` types from `mgt-element`, by adding to imports.</span></span>

    ```tsx
    import { Providers, ProviderState } from '@microsoft/mgt-element';
    ```

1. <span data-ttu-id="c6699-166">Adicione uma função personalizada nomeada `useIsSignedIn` que permite o acompanhamento do estado de entrada do usuário em seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c6699-166">Add a custom function named `useIsSignedIn` that enables tracking the user's sign in state in your application.</span></span>

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

<span data-ttu-id="c6699-167">Essa função faz duas coisas.</span><span class="sxs-lookup"><span data-stu-id="c6699-167">This function does two things.</span></span> <span data-ttu-id="c6699-168">Primeiro, usando o gancho de reagir `useState` , ele habilita o estado de controle dentro de seu componente.</span><span class="sxs-lookup"><span data-stu-id="c6699-168">First, using the React `useState` hook, it enables tracking state inside your component.</span></span> <span data-ttu-id="c6699-169">Sempre que o estado for alterado, reagir reprocessará seu componente.</span><span class="sxs-lookup"><span data-stu-id="c6699-169">Whenever the state changes, React will re-render your component.</span></span> <span data-ttu-id="c6699-170">Em segundo lugar, usando o gancho de reagir `useEffect` , ele estende o ciclo de vida do componente ao controlar as alterações no provedor do Microsoft Graph Toolkit e atualizar o componente, se necessário.</span><span class="sxs-lookup"><span data-stu-id="c6699-170">Second, using the React `useEffect` hook, it extends the component's lifecycle by tracking changes in the Microsoft Graph Toolkit provider and updating the component if necessary.</span></span>

#### <a name="load-users-calendar-if-user-is-signed-in"></a><span data-ttu-id="c6699-171">Carregar calendário do usuário se o usuário estiver conectado</span><span class="sxs-lookup"><span data-stu-id="c6699-171">Load user's calendar if user is signed in</span></span>

<span data-ttu-id="c6699-172">Agora que você acompanha o estado de entrada do usuário em seu aplicativo, você pode mostrar seu calendário após ele entrar.</span><span class="sxs-lookup"><span data-stu-id="c6699-172">Now that you track the user's sign in state in your application, you can show their calendar after they signed in.</span></span>

1. <span data-ttu-id="c6699-173">No editor de códigos, abra o arquivo **src/app. TSX** e, dentro da função **app** , adicione:</span><span class="sxs-lookup"><span data-stu-id="c6699-173">In the code editor, open the **src/App.tsx** file, and inside the **App** function, add:</span></span>

    ```tsx
    const [isSignedIn] = useIsSignedIn();
    ```

    <span data-ttu-id="c6699-174">Isso define uma constante booleana `isSignedIn` , que você pode usar para determinar se o usuário está atualmente conectado ao seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c6699-174">This defines a Boolean `isSignedIn` constant, which you can use to determine whether the user is currently signed in to your application.</span></span>

1. <span data-ttu-id="c6699-175">Estenda o conteúdo da `return` cláusula com um componente de `div` programação adicional e o Microsoft Graph Toolkit.</span><span class="sxs-lookup"><span data-stu-id="c6699-175">Extend the contents of the `return` clause with an additional `div` and the Microsoft Graph Toolkit Agenda component.</span></span>

    ```tsx
    <div>
      {isSignedIn &&
        <Agenda />}
    </div>
    ```

<span data-ttu-id="c6699-176">Com essas alterações, o arquivo **src/app. TSX** deve ser semelhante ao seguinte.</span><span class="sxs-lookup"><span data-stu-id="c6699-176">With these changes, the **src/App.tsx** file should look like the following.</span></span>

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

### <a name="test-showing-users-calendar-after-they-signed-in"></a><span data-ttu-id="c6699-177">Teste mostrando o calendário do usuário depois que ele entrou</span><span class="sxs-lookup"><span data-stu-id="c6699-177">Test showing user's calendar after they signed in</span></span>

<span data-ttu-id="c6699-178">Com essas alterações, após entrar em seu aplicativo com sua conta da Microsoft, você deve ver seu calendário.</span><span class="sxs-lookup"><span data-stu-id="c6699-178">With these changes, after signing in to your application with your Microsoft account, you should see your calendar.</span></span>

1. <span data-ttu-id="c6699-179">Para ver as alterações, feche o navegador e abra-o novamente e vá para `http://localhost:3000` .</span><span class="sxs-lookup"><span data-stu-id="c6699-179">To see the changes, close the browser and open it again, and go to `http://localhost:3000`.</span></span> <span data-ttu-id="c6699-180">Isso é feito porque você alterou o valor da `scopes` propriedade, que afeta o token de acesso solicitado pelo Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c6699-180">You do this because you changed the value of the `scopes` property, which affects the access token that you request from Azure AD.</span></span>
1. <span data-ttu-id="c6699-181">Escolha o botão **entrar** e entre usando sua conta da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c6699-181">Choose the **Sign In** button and sign in using your Microsoft account.</span></span> <span data-ttu-id="c6699-182">Observe as adições à lista de permissões solicitadas no prompt de consentimento.</span><span class="sxs-lookup"><span data-stu-id="c6699-182">Notice the additions to the list of permissions requested in the consent prompt.</span></span> <span data-ttu-id="c6699-183">Isso ocorre porque você incluiu permissões adicionais na `scope` propriedade.</span><span class="sxs-lookup"><span data-stu-id="c6699-183">This is because you included additional permissions in the `scope` property.</span></span>
1. <span data-ttu-id="c6699-184">Após a reenvio ao uso do aplicativo, você deve ver informações sobre o usuário atual e seu calendário.</span><span class="sxs-lookup"><span data-stu-id="c6699-184">After consenting to the use of the application, you should see information about the current user and their calendar.</span></span>

![Aplicativo concluído](../images/mgt-finished-app.png)

## <a name="next-steps"></a><span data-ttu-id="c6699-186">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="c6699-186">Next steps</span></span>

- <span data-ttu-id="c6699-187">Veja [o que há no Microsoft Graph Toolkit](../overview.md).</span><span class="sxs-lookup"><span data-stu-id="c6699-187">See [what's in the Microsoft Graph Toolkit](../overview.md).</span></span>
- <span data-ttu-id="c6699-188">Experimente os componentes no [playground](https://mgt.dev).</span><span class="sxs-lookup"><span data-stu-id="c6699-188">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="c6699-189">Faça uma pergunta sobre o [estouro de pilha](https://aka.ms/mgt-question).</span><span class="sxs-lookup"><span data-stu-id="c6699-189">Ask a question on [Stack Overflow](https://aka.ms/mgt-question).</span></span>
- <span data-ttu-id="c6699-190">Informe bugs ou deixe uma solicitação de recurso no [GitHub](https://aka.ms/mgt).</span><span class="sxs-lookup"><span data-stu-id="c6699-190">Report bugs or leave a feature request on [GitHub](https://aka.ms/mgt).</span></span>
