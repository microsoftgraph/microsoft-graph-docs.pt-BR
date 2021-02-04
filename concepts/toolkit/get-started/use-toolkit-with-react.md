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
# <a name="use-the-microsoft-graph-toolkit-with-react"></a><span data-ttu-id="b086b-103">Usar o Kit de Ferramentas do Microsoft Graph com o React</span><span class="sxs-lookup"><span data-stu-id="b086b-103">Use the Microsoft Graph Toolkit with React</span></span>

<span data-ttu-id="b086b-104">O Microsoft Graph Toolkit é um conjunto de componentes da Web que simplificam a conexão com o Microsoft Graph e permitem que você se concentre no seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b086b-104">Microsoft Graph Toolkit is a set of web components that simplify connecting to Microsoft Graph and allow you to focus on your application instead.</span></span> <span data-ttu-id="b086b-105">O Microsoft Graph Toolkit está disponível como um conjunto genérico de componentes web distribuídos por meio do `@microsoft/mgt` pacote npm.</span><span class="sxs-lookup"><span data-stu-id="b086b-105">Microsoft Graph Toolkit is available as a generic set of web components distributed through the `@microsoft/mgt` npm package.</span></span>

<span data-ttu-id="b086b-106">Se você estiver criando aplicativos com [ `@microsoft/mgt-react` ](./mgt-react.md)o React, poderá usar o pacote, que envolve os componentes web do Microsoft Graph Toolkit em componentes do React e facilita a passagem de dados complexos.</span><span class="sxs-lookup"><span data-stu-id="b086b-106">If you're building apps with React, you can use the [`@microsoft/mgt-react` package](./mgt-react.md), which wraps Microsoft Graph Toolkit web components in React components and makes it easier to pass complex data.</span></span>

<span data-ttu-id="b086b-107">Este artigo descreve o processo passo a passo de usar o Kit de Ferramentas do Microsoft Graph para criar um aplicativo React e conectá-lo ao Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="b086b-107">This article describes the step-by-step process of using the Microsoft Graph Toolkit to create a React app and connect it to Microsoft 365.</span></span> <span data-ttu-id="b086b-108">Depois de concluir as etapas, você terá um aplicativo React que mostra os próximos compromissos do usuário atualmente assinado do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="b086b-108">After completing the steps, you'll have a React app that shows the upcoming appointments of the currently signed in user from Microsoft 365.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b086b-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b086b-109">Prerequisites</span></span>

<span data-ttu-id="b086b-110">Para seguir as etapas deste artigo, você precisará de um ambiente de desenvolvimento do Microsoft 365 e algumas ferramentas.</span><span class="sxs-lookup"><span data-stu-id="b086b-110">To follow the steps in this article, you'll need a Microsoft 365 development environment and a few tools.</span></span> <span data-ttu-id="b086b-111">Para obter detalhes, veja [como começar.](./overview.md)</span><span class="sxs-lookup"><span data-stu-id="b086b-111">For details, see [getting started](./overview.md).</span></span>

## <a name="create-a-react-app"></a><span data-ttu-id="b086b-112">Criar um aplicativo React</span><span class="sxs-lookup"><span data-stu-id="b086b-112">Create a React app</span></span>

<span data-ttu-id="b086b-113">Crie um novo aplicativo React executando o seguinte comando.</span><span class="sxs-lookup"><span data-stu-id="b086b-113">Create a new React app by running the following command.</span></span> <span data-ttu-id="b086b-114">Isso criará um novo aplicativo React usando TypeScript, que ajudará você a escrever código mais robusto e evitar erros de tempo de execução.</span><span class="sxs-lookup"><span data-stu-id="b086b-114">This will create a new React app using TypeScript, which will help you write more robust code and avoid runtime errors.</span></span>

```cmd
npx create-react-app my-m365-app --template typescript --use-npm
```

<span data-ttu-id="b086b-115">Altere o diretório de trabalho para o aplicativo recém-criado.</span><span class="sxs-lookup"><span data-stu-id="b086b-115">Change the working directory to the newly created app.</span></span>

```cmd
cd my-m365-app
```

<span data-ttu-id="b086b-116">Em seguida, instale o `mgt-react` pacote npm, que contém os componentes do React do Kit de Ferramentas do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b086b-116">Next, install the `mgt-react` npm package, which contains the Microsoft Graph Toolkit React components.</span></span>

```cmd
npm i @microsoft/mgt-react
```

<span data-ttu-id="b086b-117">Instale também `mgt-msal-provider` `mgt-element` o pacote npm, que contém o provedor de auth MSAL.</span><span class="sxs-lookup"><span data-stu-id="b086b-117">Install the `mgt-msal-provider` and `mgt-element` npm package as well, which contains the MSAL auth provider.</span></span>

```cmd
npm i @microsoft/mgt-element @microsoft/mgt-msal-provider
```

<span data-ttu-id="b086b-118">Confirme se você pode executar o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b086b-118">Confirm that you can run the app.</span></span>

```cmd
npm start
```

<span data-ttu-id="b086b-119">Você deve ser capaz de abrir seu aplicativo no navegador via `http://localhost:3000` .</span><span class="sxs-lookup"><span data-stu-id="b086b-119">You should be able to open your app in the browser via `http://localhost:3000`.</span></span>

[!INCLUDE [AAD with implicit flow app registration](../includes/aad-app-registration-spa.md)]

## <a name="connect-react-app-to-microsoft-365"></a><span data-ttu-id="b086b-120">Conectar o aplicativo React ao Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="b086b-120">Connect React app to Microsoft 365</span></span>

<span data-ttu-id="b086b-121">Agora que você registrou seu aplicativo no Azure Active Directory (Azure AD), poderá conectar o aplicativo React ao Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="b086b-121">Now that you have registered your application with Azure Active Directory (Azure AD), you can connect the React app to Microsoft 365.</span></span> <span data-ttu-id="b086b-122">Primeiro, permita que os usuários se inscrevam no aplicativo usando a conta da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b086b-122">First, allow users to sign in to the app using their Microsoft account.</span></span>

### <a name="copy-the-azure-ad-application-registration-id"></a><span data-ttu-id="b086b-123">Copiar a ID de registro do aplicativo Azure AD</span><span class="sxs-lookup"><span data-stu-id="b086b-123">Copy the Azure AD application registration ID</span></span>

1. <span data-ttu-id="b086b-124">No Portal do Azure, vá para o registro do seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b086b-124">In the Azure Portal, go to your application registration.</span></span>
1. <span data-ttu-id="b086b-125">Verifique se você está na página **Visão** Geral.</span><span class="sxs-lookup"><span data-stu-id="b086b-125">Verify that you are on the **Overview** page.</span></span>
1. <span data-ttu-id="b086b-126">Na seção **Essentials,** copie o valor da propriedade **de ID do aplicativo (cliente)**</span><span class="sxs-lookup"><span data-stu-id="b086b-126">From the **Essentials** section, copy the value of the **Application (client) ID** property</span></span>

### <a name="configure-the-microsoft-graph-toolkit-authentication-provider"></a><span data-ttu-id="b086b-127">Configurar o provedor de autenticação do Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="b086b-127">Configure the Microsoft Graph Toolkit authentication provider</span></span>

<span data-ttu-id="b086b-128">Em seguida, configure o provedor de autenticação que o Microsoft Graph Toolkit deve usar.</span><span class="sxs-lookup"><span data-stu-id="b086b-128">Next, configure the authentication provider that the Microsoft Graph Toolkit should use.</span></span> <span data-ttu-id="b086b-129">Nesse caso, você usará a MSAL, que é um bom padrão para a criação de aplicativos autônomos.</span><span class="sxs-lookup"><span data-stu-id="b086b-129">In this case, you'll use MSAL, which is a good default for building standalone applications.</span></span> <span data-ttu-id="b086b-130">Se você usar qualquer um dos pontos de extensibilidade no Microsoft 365, como o Teams ou o SharePoint, você usará [outros provedores.](../providers/providers.md)</span><span class="sxs-lookup"><span data-stu-id="b086b-130">If you use any of the extensibility points in Microsoft 365, like Teams or SharePoint, you will use [other providers](../providers/providers.md).</span></span>

1. <span data-ttu-id="b086b-131">No editor de código, abra **o src/index.**</span><span class="sxs-lookup"><span data-stu-id="b086b-131">In the code editor, open the **src/index.**</span></span> <span data-ttu-id="b086b-132">e na lista de importações, adicione:</span><span class="sxs-lookup"><span data-stu-id="b086b-132">file, and to the list of imports, add:</span></span>

    ```tsx
    import { Providers } from '@microsoft/mgt-element';
    import { MsalProvider } from '@microsoft/mgt-msal-provider';
    ```

1. <span data-ttu-id="b086b-133">Após a última `import` instrução, inicialize o Microsoft Graph Toolkit com o provedor MSAL.</span><span class="sxs-lookup"><span data-stu-id="b086b-133">After the last `import` statement, initialize the Microsoft Graph Toolkit with MSAL provider.</span></span>

    ```tsx
    Providers.globalProvider = new MsalProvider({
      clientId: 'REPLACE_WITH_CLIENTID'
    });
    ```

    <span data-ttu-id="b086b-134">Substitua o valor da `clientId` propriedade pelo valor da propriedade que você `Application (client) ID` copiou anteriormente no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="b086b-134">Replace the value of the `clientId` property with the value of the `Application (client) ID` property you copied previously in the Azure Portal.</span></span>

<span data-ttu-id="b086b-135">Com essas alterações, o **arquivo src/index.tsx** terá a seguinte aparência.</span><span class="sxs-lookup"><span data-stu-id="b086b-135">With these changes, the **src/index.tsx** file will look like the following.</span></span>

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

### <a name="add-the-sign-in-button"></a><span data-ttu-id="b086b-136">Adicionar o botão Entrar</span><span class="sxs-lookup"><span data-stu-id="b086b-136">Add the Sign in button</span></span>

<span data-ttu-id="b086b-137">Adicione o **componente React** do Kit de  Ferramentas do Microsoft Graph de logon, que exibirá o botão Entrar que as pessoas podem usar para entrar com a conta da Microsoft em seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b086b-137">Add the **Login** Microsoft Graph Toolkit React component, which will display the **Sign in** button people can use to sign in with their Microsoft account to your app.</span></span>

1. <span data-ttu-id="b086b-138">No editor de código, abra o **arquivo src/App.tsx** e adicione à lista de importações:</span><span class="sxs-lookup"><span data-stu-id="b086b-138">In the code editor, open the **src/App.tsx** file, and to the list of imports add:</span></span>

    ```tsx
    import { Login } from '@microsoft/mgt-react';
    ```

1. <span data-ttu-id="b086b-139">Na função, substitua o conteúdo da cláusula pela estrutura básica, incluindo o componente logon do Kit de Ferramentas `App` `return` do Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="b086b-139">In the `App` function, replace the contents of the `return` clause with the basic structure including the Microsoft Graph Toolkit Login component:</span></span>

    ```tsx
    <div className="App">
      <header>
        <Login />
      </header>
    </div>
    ```

<span data-ttu-id="b086b-140">Com essas alterações, o **arquivo src/App.tsx** terá a seguinte aparência.</span><span class="sxs-lookup"><span data-stu-id="b086b-140">With these changes, the **src/App.tsx** file will look like the following.</span></span>
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

### <a name="test-signing-in-to-your-application"></a><span data-ttu-id="b086b-141">Testar a assinatura em seu aplicativo</span><span class="sxs-lookup"><span data-stu-id="b086b-141">Test signing in to your application</span></span>

<span data-ttu-id="b086b-142">Agora você poderá entrar em seu aplicativo com sua conta da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b086b-142">You should now be able to sign in to your application with your Microsoft account.</span></span>

1. <span data-ttu-id="b086b-143">Volte para o navegador em que seu aplicativo React está sendo executado.</span><span class="sxs-lookup"><span data-stu-id="b086b-143">Go back to the browser where your React app is running.</span></span> <span data-ttu-id="b086b-144">Agora você deve ver um **botão Entrar.**</span><span class="sxs-lookup"><span data-stu-id="b086b-144">You should now see a **Sign in** button.</span></span>
1. <span data-ttu-id="b086b-145">Ao clicar  no botão Entrar, você será solicitado a entrar com sua conta da Microsoft (você pode usar a mesma conta que a que acessou o Portal do Azure).</span><span class="sxs-lookup"><span data-stu-id="b086b-145">When you click the **Sign in** button, you will be prompted to sign in with your Microsoft account (you can use the same account as the one you accessed the Azure Portal with).</span></span>
1. <span data-ttu-id="b086b-146">Como esta é a primeira vez que você está usando esse aplicativo Azure AD, precisa consentir seu uso em sua organização.</span><span class="sxs-lookup"><span data-stu-id="b086b-146">Because this is the first time you're using this Azure AD application, you need to consent its use in your organization.</span></span>
1. <span data-ttu-id="b086b-147">Depois de entrar, você será redirecionado para seu aplicativo React.</span><span class="sxs-lookup"><span data-stu-id="b086b-147">After signing in, you will be redirected to your React app.</span></span> <span data-ttu-id="b086b-148">Observe que o **botão** Entrar foi alterado para mostrar o nome do aplicativo React do usuário mostrando as informações do usuário recuperadas do ![ Microsoft 365 usando o Microsoft Graph ](../images/mgt-react-userinfo.png) Toolkit.</span><span class="sxs-lookup"><span data-stu-id="b086b-148">Notice that the **Sign in** button changed to show your user's name ![React app showing user info retrieved from Microsoft 365 using Microsoft Graph Toolkit](../images/mgt-react-userinfo.png).</span></span>

## <a name="load-data-from-microsoft-365"></a><span data-ttu-id="b086b-149">Carregar dados do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="b086b-149">Load data from Microsoft 365</span></span>

<span data-ttu-id="b086b-150">O Microsoft Graph Toolkit não apenas simplifica a autenticação para o Microsoft 365, mas também carrega seus dados.</span><span class="sxs-lookup"><span data-stu-id="b086b-150">Microsoft Graph Toolkit not only simplifies authentication to Microsoft 365, but also loading its data.</span></span> <span data-ttu-id="b086b-151">Neste exemplo, você mostrará o calendário da pessoa.</span><span class="sxs-lookup"><span data-stu-id="b086b-151">In this example, you'll show the signed in person's calendar.</span></span>

### <a name="specify-permissions-needed-for-your-application"></a><span data-ttu-id="b086b-152">Especificar permissões necessárias para seu aplicativo</span><span class="sxs-lookup"><span data-stu-id="b086b-152">Specify permissions needed for your application</span></span>

<span data-ttu-id="b086b-153">Antes de carregar dados do Microsoft 365, você precisa especificar a lista de escopos de permissão que seu aplicativo deve ter para acessar os dados do usuário.</span><span class="sxs-lookup"><span data-stu-id="b086b-153">Before you can load data from Microsoft 365, you need to specify the list of permission scopes your application must be granted to access user's data.</span></span> <span data-ttu-id="b086b-154">Esses escopos diferem dependendo do tipo de informação que você deseja mostrar.</span><span class="sxs-lookup"><span data-stu-id="b086b-154">These scopes differ depending on what kind of information you want to show.</span></span> <span data-ttu-id="b086b-155">Nesse caso, você precisará de acesso ao calendário das pessoas, bem como acesso básico a informações sobre as pessoas que também são exibidas no calendário.</span><span class="sxs-lookup"><span data-stu-id="b086b-155">In this case, you will need access to people's calendar as well as basic access to information about people that is also displayed in the calendar.</span></span> <span data-ttu-id="b086b-156">Você pode encontrar os escopos exigidos por cada API na documentação da [API do Microsoft Graph.](/graph/api/overview)</span><span class="sxs-lookup"><span data-stu-id="b086b-156">You can find the scopes required by each API in the [Microsoft Graph API documentation](/graph/api/overview).</span></span>

1. <span data-ttu-id="b086b-157">No editor de código, abra o **arquivo src/index.tsx** e atualize o código de inicialização do provedor.</span><span class="sxs-lookup"><span data-stu-id="b086b-157">In the code editor, open the **src/index.tsx** file, and update the provider initialization code.</span></span>

    ```tsx
    Providers.globalProvider = new MsalProvider({
      clientId: 'd7cb93c9-9097-4e38-8f06-7c0088ac3318',
      scopes: ['calendars.read', 'user.read', 'openid', 'profile', 'people.read', 'user.readbasic.all']
    });
    ```

### <a name="show-users-data-after-signing-in"></a><span data-ttu-id="b086b-158">Mostrar dados do usuário após entrar</span><span class="sxs-lookup"><span data-stu-id="b086b-158">Show user's data after signing in</span></span>

<span data-ttu-id="b086b-159">Em seguida, estenda o aplicativo para mostrar dados do calendário do usuário.</span><span class="sxs-lookup"><span data-stu-id="b086b-159">Next, extend the application to show data from the user's calendar.</span></span> <span data-ttu-id="b086b-160">Você só poderá acessar essas informações depois que o usuário entrar.</span><span class="sxs-lookup"><span data-stu-id="b086b-160">You can access this information only after the user has signed in.</span></span> <span data-ttu-id="b086b-161">Para fazer isso, você precisará controlar o estado de login do usuário e mostrar os dados do calendário depois que o usuário entrar com a conta da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b086b-161">To do this, you will need to track the  user's sign in state and show the calendar data after the user has signed in with their Microsoft account.</span></span>

#### <a name="track-users-sign-in-state"></a><span data-ttu-id="b086b-162">Acompanhar o estado de login do usuário</span><span class="sxs-lookup"><span data-stu-id="b086b-162">Track user's sign in state</span></span>

<span data-ttu-id="b086b-163">Para controlar o estado de login do usuário em seu aplicativo, você usará o React e os ganchos em combinação com manipuladores de `useState` `useEffect` eventos do provedor.</span><span class="sxs-lookup"><span data-stu-id="b086b-163">To track the user's sign in state in your application, you will use the React `useState` and `useEffect` hooks in combination with provider event handlers.</span></span>

1. <span data-ttu-id="b086b-164">No editor de código, abra o **arquivo src/App.tsx** e estenda a instrução React `import` existente.</span><span class="sxs-lookup"><span data-stu-id="b086b-164">In the code editor, open the **src/App.tsx** file and extend the existing React `import` statement.</span></span>

    ```tsx
    import React, { useState, useEffect } from 'react';
    ```

1. <span data-ttu-id="b086b-165">Importe o `Provider` e os tipos de , `ProviderState` `mgt-element` adicionando às importações.</span><span class="sxs-lookup"><span data-stu-id="b086b-165">Import the `Provider` and `ProviderState` types from `mgt-element`, by adding to imports.</span></span>

    ```tsx
    import { Providers, ProviderState } from '@microsoft/mgt-element';
    ```

1. <span data-ttu-id="b086b-166">Adicione uma função personalizada chamada que permite rastrear o estado de login do `useIsSignedIn` usuário em seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b086b-166">Add a custom function named `useIsSignedIn` that enables tracking the user's sign in state in your application.</span></span>

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

<span data-ttu-id="b086b-167">Esta função faz duas coisas.</span><span class="sxs-lookup"><span data-stu-id="b086b-167">This function does two things.</span></span> <span data-ttu-id="b086b-168">Primeiro, usando o `useState` gancho do React, ele habilita o estado de rastreamento dentro do componente.</span><span class="sxs-lookup"><span data-stu-id="b086b-168">First, using the React `useState` hook, it enables tracking state inside your component.</span></span> <span data-ttu-id="b086b-169">Sempre que o estado mudar, o React renderizará o componente.</span><span class="sxs-lookup"><span data-stu-id="b086b-169">Whenever the state changes, React will re-render your component.</span></span> <span data-ttu-id="b086b-170">Em segundo lugar, usando o gancho react, ele estende o ciclo de vida do componente rastreando as alterações no provedor do Microsoft Graph Toolkit e atualizando o `useEffect` componente, se necessário.</span><span class="sxs-lookup"><span data-stu-id="b086b-170">Second, using the React `useEffect` hook, it extends the component's lifecycle by tracking changes in the Microsoft Graph Toolkit provider and updating the component if necessary.</span></span>

#### <a name="load-users-calendar-if-user-is-signed-in"></a><span data-ttu-id="b086b-171">Carregar o calendário do usuário se o usuário estiver se inscreveu</span><span class="sxs-lookup"><span data-stu-id="b086b-171">Load user's calendar if user is signed in</span></span>

<span data-ttu-id="b086b-172">Agora que você rastreia o estado de login do usuário em seu aplicativo, pode mostrar o calendário depois de entrar.</span><span class="sxs-lookup"><span data-stu-id="b086b-172">Now that you track the user's sign in state in your application, you can show their calendar after they signed in.</span></span>

1. <span data-ttu-id="b086b-173">No editor de código, abra o **arquivo src/App.tsx** e, dentro da função **App,** adicione:</span><span class="sxs-lookup"><span data-stu-id="b086b-173">In the code editor, open the **src/App.tsx** file, and inside the **App** function, add:</span></span>

    ```tsx
    const [isSignedIn] = useIsSignedIn();
    ```

    <span data-ttu-id="b086b-174">Isso define uma constante Boolean, que você pode usar para determinar se o usuário está `isSignedIn` atualmente londo em seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b086b-174">This defines a Boolean `isSignedIn` constant, which you can use to determine whether the user is currently signed in to your application.</span></span>

1. <span data-ttu-id="b086b-175">Estenda o conteúdo da cláusula com um componente adicional e o componente agenda do Kit de Ferramentas `return` `div` do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b086b-175">Extend the contents of the `return` clause with an additional `div` and the Microsoft Graph Toolkit Agenda component.</span></span>

    ```tsx
    <div>
      {isSignedIn &&
        <Agenda />}
    </div>
    ```

<span data-ttu-id="b086b-176">Com essas alterações, o **arquivo src/App.tsx** deve se parecer com o seguinte.</span><span class="sxs-lookup"><span data-stu-id="b086b-176">With these changes, the **src/App.tsx** file should look like the following.</span></span>

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

### <a name="test-showing-users-calendar-after-they-signed-in"></a><span data-ttu-id="b086b-177">Teste mostrando o calendário do usuário depois que ele se inscreveu</span><span class="sxs-lookup"><span data-stu-id="b086b-177">Test showing user's calendar after they signed in</span></span>

<span data-ttu-id="b086b-178">Com essas alterações, depois de entrar em seu aplicativo com sua conta da Microsoft, você deverá ver seu calendário.</span><span class="sxs-lookup"><span data-stu-id="b086b-178">With these changes, after signing in to your application with your Microsoft account, you should see your calendar.</span></span>

1. <span data-ttu-id="b086b-179">Para ver as alterações, feche o navegador e abra-o novamente e vá para `http://localhost:3000` .</span><span class="sxs-lookup"><span data-stu-id="b086b-179">To see the changes, close the browser and open it again, and go to `http://localhost:3000`.</span></span> <span data-ttu-id="b086b-180">Você faz isso porque alterou o valor da propriedade, o que afeta o token de acesso que você `scopes` solicita do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b086b-180">You do this because you changed the value of the `scopes` property, which affects the access token that you request from Azure AD.</span></span>
1. <span data-ttu-id="b086b-181">Escolha o **botão Entrar** e entre usando sua conta da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b086b-181">Choose the **Sign In** button and sign in using your Microsoft account.</span></span> <span data-ttu-id="b086b-182">Observe as adições à lista de permissões solicitadas na solicitação de consentimento.</span><span class="sxs-lookup"><span data-stu-id="b086b-182">Notice the additions to the list of permissions requested in the consent prompt.</span></span> <span data-ttu-id="b086b-183">Isso porque você incluiu permissões adicionais na `scope` propriedade.</span><span class="sxs-lookup"><span data-stu-id="b086b-183">This is because you included additional permissions in the `scope` property.</span></span>
1. <span data-ttu-id="b086b-184">Depois de consentir o uso do aplicativo, você deverá ver informações sobre o usuário atual e seu calendário.</span><span class="sxs-lookup"><span data-stu-id="b086b-184">After consenting to the use of the application, you should see information about the current user and their calendar.</span></span>

![Aplicativo concluído](../images/mgt-finished-app.png)

## <a name="next-steps"></a><span data-ttu-id="b086b-186">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="b086b-186">Next steps</span></span>

- <span data-ttu-id="b086b-187">Veja [o que há no Kit de Ferramentas do Microsoft Graph.](../overview.md)</span><span class="sxs-lookup"><span data-stu-id="b086b-187">See [what's in the Microsoft Graph Toolkit](../overview.md).</span></span>
- <span data-ttu-id="b086b-188">Experimente os componentes no [playground.](https://mgt.dev)</span><span class="sxs-lookup"><span data-stu-id="b086b-188">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="b086b-189">Faça uma pergunta no [Stack Overflow](https://aka.ms/mgt-question).</span><span class="sxs-lookup"><span data-stu-id="b086b-189">Ask a question on [Stack Overflow](https://aka.ms/mgt-question).</span></span>
- <span data-ttu-id="b086b-190">Relatar bugs ou deixar uma solicitação de recurso [no GitHub.](https://aka.ms/mgt)</span><span class="sxs-lookup"><span data-stu-id="b086b-190">Report bugs or leave a feature request on [GitHub](https://aka.ms/mgt).</span></span>
