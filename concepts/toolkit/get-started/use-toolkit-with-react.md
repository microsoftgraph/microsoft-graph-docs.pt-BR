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
# <a name="use-the-microsoft-graph-toolkit-with-react"></a><span data-ttu-id="3ea8c-103">Use o kit de ferramentas do Microsoft Graph com reagir</span><span class="sxs-lookup"><span data-stu-id="3ea8c-103">Use the Microsoft Graph Toolkit with React</span></span>

<span data-ttu-id="3ea8c-104">O Microsoft Graph Toolkit é um conjunto de componentes Web que simplifica a conexão com o Microsoft Graph e permite que você se concentre em seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3ea8c-104">Microsoft Graph Toolkit is a set of web components that simplify connecting to Microsoft Graph and allow you to focus on your application instead.</span></span> <span data-ttu-id="3ea8c-105">O Microsoft Graph Toolkit está disponível como um conjunto genérico de componentes Web distribuídos por meio do pacote **@microsoft/MGT** NPM.</span><span class="sxs-lookup"><span data-stu-id="3ea8c-105">Microsoft Graph Toolkit is available as a generic set of web components distributed through the **@microsoft/mgt** npm package.</span></span>

<span data-ttu-id="3ea8c-106">Se você estiver criando aplicativos com reagir, poderá usar o pacote **@microsoft/MGT-React** , que encapsula o Microsoft Graph Toolkit Web Components em reagir componentes e torna mais fácil transmitir dados complexos.</span><span class="sxs-lookup"><span data-stu-id="3ea8c-106">If you're building apps with React, you can use the **@microsoft/mgt-react** package, which wraps Microsoft Graph Toolkit web components in React components and makes it easier to pass complex data.</span></span>

<span data-ttu-id="3ea8c-107">Este artigo descreve o processo passo a passo de usar o kit de ferramentas do Microsoft Graph para criar um aplicativo reagir e conectá-lo ao Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="3ea8c-107">This article describes the step-by-step process of using the Microsoft Graph Toolkit to create a React app and connect it to Microsoft 365.</span></span> <span data-ttu-id="3ea8c-108">Após concluir as etapas, você terá um aplicativo reagir que mostra os futuros compromissos do usuário conectado no momento da Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="3ea8c-108">After completing the steps, you'll have a React app that shows the upcoming appointments of the currently signed in user from Microsoft 365.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3ea8c-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3ea8c-109">Prerequisites</span></span>

<span data-ttu-id="3ea8c-110">Para seguir as etapas deste artigo, você precisará de um ambiente de desenvolvimento do Microsoft 365 e de algumas ferramentas.</span><span class="sxs-lookup"><span data-stu-id="3ea8c-110">To follow the steps in this article, you'll need a Microsoft 365 development environment and a few tools.</span></span> <span data-ttu-id="3ea8c-111">Para obter detalhes, consulte [introdução](./overview.md).</span><span class="sxs-lookup"><span data-stu-id="3ea8c-111">For details, see [getting started](./overview.md).</span></span>

## <a name="create-a-react-app"></a><span data-ttu-id="3ea8c-112">Criar um aplicativo reagir</span><span class="sxs-lookup"><span data-stu-id="3ea8c-112">Create a React app</span></span>

<span data-ttu-id="3ea8c-113">Crie um novo aplicativo reagir executando o seguinte comando.</span><span class="sxs-lookup"><span data-stu-id="3ea8c-113">Create a new React app by running the following command.</span></span> <span data-ttu-id="3ea8c-114">Isso criará um novo aplicativo reagir usando TypeScript, que o ajudará a escrever código mais robusto e evitar erros de tempo de execução.</span><span class="sxs-lookup"><span data-stu-id="3ea8c-114">This will create a new React app using TypeScript, which will help you write more robust code and avoid runtime errors.</span></span>

```cmd
npx create-react-app my-m365-app --template typescript
```

<span data-ttu-id="3ea8c-115">Altere o diretório de trabalho para o aplicativo recém-criado.</span><span class="sxs-lookup"><span data-stu-id="3ea8c-115">Change the working directory to the newly created app.</span></span>

```cmd
cd my-m365-app
```

<span data-ttu-id="3ea8c-116">Em seguida, instale o pacote NPM **-reajam** , que contém os componentes de reagir do Microsoft Graph Toolkit.</span><span class="sxs-lookup"><span data-stu-id="3ea8c-116">Next, install the **mgt-react** npm package, which contains the Microsoft Graph Toolkit React components.</span></span>

```cmd
npm i @microsoft/mgt-react
```

<span data-ttu-id="3ea8c-117">Confirme que você pode executar o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3ea8c-117">Confirm that you can run the app.</span></span>

```cmd
HTTPS=true npm start
```

> [!IMPORTANT]
> <span data-ttu-id="3ea8c-118">Seu aplicativo precisa ser executado em HTTPS para poder autenticar-se no Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="3ea8c-118">Your app need to run on HTTPS in order to be able to authenticate against Microsoft 365.</span></span> <span data-ttu-id="3ea8c-119">Para teste local, com os scripts de reagir, você pode configurar o servidor Web local para ser executado em HTTPS, definindo a `HTTPS` variável de ambiente como `true` .</span><span class="sxs-lookup"><span data-stu-id="3ea8c-119">For local testing, with the React scripts, you can configure the local web server to run on HTTPS by setting the `HTTPS` environment variable to `true`.</span></span> <span data-ttu-id="3ea8c-120">Você pode fazer isso sempre, prefixando o `npm start` comando com `HTTPS=true` (funciona apenas em bash) ou configurando a variável de ambiente globalmente no computador.</span><span class="sxs-lookup"><span data-stu-id="3ea8c-120">You can do this either each time, by prefixing the `npm start` command with `HTTPS=true` (works only in bash) or by setting the environment variable globally on your computer.</span></span>

<span data-ttu-id="3ea8c-121">Você deve ser capaz de abrir seu aplicativo no navegador via `https://localhost:3000` .</span><span class="sxs-lookup"><span data-stu-id="3ea8c-121">You should be able to open your app in the browser via `https://localhost:3000`.</span></span>

[!INCLUDE [AAD with implicit flow app registration](../includes/aad-app-registration-spa.md)]

## <a name="connect-react-app-to-microsoft-365"></a><span data-ttu-id="3ea8c-122">Conectar aplicativo reagir ao Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="3ea8c-122">Connect React app to Microsoft 365</span></span>

<span data-ttu-id="3ea8c-123">Agora que você registrou seu aplicativo com o Azure Active Directory (Azure AD), você pode conectar o aplicativo reagir ao Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="3ea8c-123">Now that you have registered your application with Azure Active Directory (Azure AD), you can connect the React app to Microsoft 365.</span></span> <span data-ttu-id="3ea8c-124">Primeiro, permita que os usuários entrem no aplicativo usando sua conta da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="3ea8c-124">First, allow users to sign in to the app using their Microsoft account.</span></span>

### <a name="copy-the-azure-ad-application-registration-id"></a><span data-ttu-id="3ea8c-125">Copiar a ID de registro do aplicativo do Azure AD</span><span class="sxs-lookup"><span data-stu-id="3ea8c-125">Copy the Azure AD application registration ID</span></span>

1. <span data-ttu-id="3ea8c-126">No portal do Azure, vá para o registro do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3ea8c-126">In the Azure Portal, go to your application registration.</span></span>
1. <span data-ttu-id="3ea8c-127">Verifique se você está na página de **visão geral** .</span><span class="sxs-lookup"><span data-stu-id="3ea8c-127">Verify that you are on the **Overview** page.</span></span>
1. <span data-ttu-id="3ea8c-128">Na seção **Essentials** , copie o valor da propriedade **ID do aplicativo (cliente)**</span><span class="sxs-lookup"><span data-stu-id="3ea8c-128">From the **Essentials** section, copy the value of the **Application (client) ID** property</span></span>

### <a name="configure-the-microsoft-graph-toolkit-authentication-provider"></a><span data-ttu-id="3ea8c-129">Configurar o provedor de autenticação do kit de ferramentas do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="3ea8c-129">Configure the Microsoft Graph Toolkit authentication provider</span></span>

<span data-ttu-id="3ea8c-130">Em seguida, configure o provedor de autenticação que o Microsoft Graph Toolkit deve usar.</span><span class="sxs-lookup"><span data-stu-id="3ea8c-130">Next, configure the authentication provider that the Microsoft Graph Toolkit should use.</span></span> <span data-ttu-id="3ea8c-131">Nesse caso, você usará o MSAL, que é um bom padrão para criar aplicativos autônomos.</span><span class="sxs-lookup"><span data-stu-id="3ea8c-131">In this case, you'll use MSAL, which is a good default for building standalone applications.</span></span> <span data-ttu-id="3ea8c-132">Se você usar qualquer um dos pontos de extensibilidade no Microsoft 365, como o Teams ou o SharePoint, você usará [outros provedores](../providers.md).</span><span class="sxs-lookup"><span data-stu-id="3ea8c-132">If you use any of the extensibility points in Microsoft 365, like Teams or SharePoint, you will use [other providers](../providers.md).</span></span>

1. <span data-ttu-id="3ea8c-133">No editor de código, abra **src/index.**</span><span class="sxs-lookup"><span data-stu-id="3ea8c-133">In the code editor, open the **src/index.**</span></span> <span data-ttu-id="3ea8c-134">e, na lista de importações, adicione:</span><span class="sxs-lookup"><span data-stu-id="3ea8c-134">file, and to the list of imports, add:</span></span>

    ```tsx
    import { MsalProvider, Providers } from '@microsoft/mgt';
    ```

1. <span data-ttu-id="3ea8c-135">Após a última `import` instrução, inicialize o Microsoft Graph Toolkit com o provedor MSAL.</span><span class="sxs-lookup"><span data-stu-id="3ea8c-135">After the last `import` statement, initialize the Microsoft Graph Toolkit with MSAL provider.</span></span>

    ```tsx
    Providers.globalProvider = new MsalProvider({
      clientId: 'REPLACE_WITH_CLIENTID'
    });
    ```

    <span data-ttu-id="3ea8c-136">Substitua o valor da `clientId` propriedade com o valor da `Application (client) ID` propriedade que você copiou anteriormente no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="3ea8c-136">Replace the value of the `clientId` property with the value of the `Application (client) ID` property you copied previously in the Azure Portal.</span></span>

<span data-ttu-id="3ea8c-137">Com essas alterações, o arquivo **src/index. TSX** será semelhante ao seguinte.</span><span class="sxs-lookup"><span data-stu-id="3ea8c-137">With these changes, the **src/index.tsx** file will look like the following.</span></span>

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

### <a name="add-the-sign-in-button"></a><span data-ttu-id="3ea8c-138">Adicionar o botão entrar</span><span class="sxs-lookup"><span data-stu-id="3ea8c-138">Add the Sign in button</span></span>

<span data-ttu-id="3ea8c-139">Adicione o componente de **logon** do Microsoft Graph Toolkit para reagir, que exibirá o botão de **entrada** que as pessoas podem usar para entrar com sua conta da Microsoft em seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3ea8c-139">Add the **Login** Microsoft Graph Toolkit React component, which will display the **Sign in** button people can use to sign in with their Microsoft account to your app.</span></span>

1. <span data-ttu-id="3ea8c-140">No editor de códigos, abra o arquivo **src/app. TSX** e, na lista de importações, adicione:</span><span class="sxs-lookup"><span data-stu-id="3ea8c-140">In the code editor, open the **src/App.tsx** file, and to the list of imports add:</span></span>

    ```tsx
    import { Login } from '@microsoft/mgt-react';
    ```

1. <span data-ttu-id="3ea8c-141">Na `App` função, substitua o conteúdo da `return` cláusula pela estrutura básica, incluindo o componente de logon do Microsoft Graph Toolkit:</span><span class="sxs-lookup"><span data-stu-id="3ea8c-141">In the `App` function, replace the contents of the `return` clause with the basic structure including the Microsoft Graph Toolkit Login component:</span></span>

    ```tsx
    <div className="App">
      <header>
        <Login />
      </header>
    </div>
    ```

<span data-ttu-id="3ea8c-142">Com essas alterações, o arquivo **src/app. TSX** será semelhante ao seguinte.</span><span class="sxs-lookup"><span data-stu-id="3ea8c-142">With these changes, the **src/App.tsx** file will look like the following.</span></span>
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

### <a name="test-signing-in-to-your-application"></a><span data-ttu-id="3ea8c-143">Testar sessão no seu aplicativo</span><span class="sxs-lookup"><span data-stu-id="3ea8c-143">Test signing in to your application</span></span>

<span data-ttu-id="3ea8c-144">Agora você poderá entrar no seu aplicativo com sua conta da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="3ea8c-144">You should now be able to sign in to your application with your Microsoft account.</span></span>

1. <span data-ttu-id="3ea8c-145">Volte para o navegador onde seu aplicativo reagir está em execução.</span><span class="sxs-lookup"><span data-stu-id="3ea8c-145">Go back to the browser where your React app is running.</span></span> <span data-ttu-id="3ea8c-146">Agora você deve ver um botão **entrar** .</span><span class="sxs-lookup"><span data-stu-id="3ea8c-146">You should now see a **Sign in** button.</span></span>
1. <span data-ttu-id="3ea8c-147">Ao clicar no botão **entrar** , você será solicitado a entrar com sua conta da Microsoft (você pode usar a mesma conta que você acessou o portal do Azure).</span><span class="sxs-lookup"><span data-stu-id="3ea8c-147">When you click the **Sign in** button, you will be prompted to sign in with your Microsoft account (you can use the same account as the one you accessed the Azure Portal with).</span></span>
1. <span data-ttu-id="3ea8c-148">Como esta é a primeira vez que você está usando esse aplicativo do Azure AD, você precisa consentir seu uso na sua organização.</span><span class="sxs-lookup"><span data-stu-id="3ea8c-148">Because this is the first time you're using this Azure AD application, you need to consent its use in your organization.</span></span>
1. <span data-ttu-id="3ea8c-149">Após entrar, você será redirecionado para seu aplicativo reagir.</span><span class="sxs-lookup"><span data-stu-id="3ea8c-149">After signing in, you will be redirected to your React app.</span></span> <span data-ttu-id="3ea8c-150">Observe que o botão **entrar** foi alterado para mostrar o nome do seu usuário ![ aplicativo reagir mostrando as informações do usuário recuperadas do Microsoft 365 usando o Microsoft Graph Toolkit ](../images/mgt-react-userinfo.png) .</span><span class="sxs-lookup"><span data-stu-id="3ea8c-150">Notice that the **Sign in** button changed to show your user's name ![React app showing user info retrieved from Microsoft 365 using Microsoft Graph Toolkit](../images/mgt-react-userinfo.png).</span></span>

## <a name="load-data-from-microsoft-365"></a><span data-ttu-id="3ea8c-151">Carregar dados do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="3ea8c-151">Load data from Microsoft 365</span></span>

<span data-ttu-id="3ea8c-152">O Microsoft Graph Toolkit não apenas simplifica a autenticação para o Microsoft 365, mas também o carregamento dos dados.</span><span class="sxs-lookup"><span data-stu-id="3ea8c-152">Microsoft Graph Toolkit not only simplifies authentication to Microsoft 365, but also loading its data.</span></span> <span data-ttu-id="3ea8c-153">Neste exemplo, você mostrará o calendário do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="3ea8c-153">In this example, you'll show the signed in person's calendar.</span></span>

### <a name="specify-permissions-needed-for-your-application"></a><span data-ttu-id="3ea8c-154">Especificar permissões necessárias para seu aplicativo</span><span class="sxs-lookup"><span data-stu-id="3ea8c-154">Specify permissions needed for your application</span></span>

<span data-ttu-id="3ea8c-155">Antes de poder carregar dados do Microsoft 365, você precisa especificar a lista de escopos de permissão que seu aplicativo deve ser concedido para acessar os dados do usuário.</span><span class="sxs-lookup"><span data-stu-id="3ea8c-155">Before you can load data from Microsoft 365, you need to specify the list of permission scopes your application must be granted to access user's data.</span></span> <span data-ttu-id="3ea8c-156">Esses escopos diferem, dependendo do tipo de informação que você deseja exibir.</span><span class="sxs-lookup"><span data-stu-id="3ea8c-156">These scopes differ depending on what kind of information you want to show.</span></span> <span data-ttu-id="3ea8c-157">Nesse caso, você precisará acessar o calendário de pessoas e o acesso básico às informações sobre as pessoas que também são exibidas no calendário.</span><span class="sxs-lookup"><span data-stu-id="3ea8c-157">In this case, you will need access to people's calendar as well as basic access to information about people that is also displayed in the calendar.</span></span> <span data-ttu-id="3ea8c-158">Você pode encontrar os escopos exigidos por cada API na [documentação da API do Microsoft Graph](/graph/api/overview?toc=.%2Fref%2Ftoc.json&view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="3ea8c-158">You can find the scopes required by each API in the [Microsoft Graph API documentation](/graph/api/overview?toc=.%2Fref%2Ftoc.json&view=graph-rest-1.0).</span></span>

1. <span data-ttu-id="3ea8c-159">No editor de códigos, abra o arquivo **src/index. TSX** e atualize o código de inicialização do provedor.</span><span class="sxs-lookup"><span data-stu-id="3ea8c-159">In the code editor, open the **src/index.tsx** file, and update the provider initialization code.</span></span>

    ```tsx
    Providers.globalProvider = new MsalProvider({
      clientId: 'd7cb93c9-9097-4e38-8f06-7c0088ac3318',
      scopes: ['calendars.read', 'user.read', 'openid', 'profile', 'people.read', 'user.readbasic.all']
    });
    ```

### <a name="show-users-data-after-signing-in"></a><span data-ttu-id="3ea8c-160">Mostrar dados do usuário após entrar</span><span class="sxs-lookup"><span data-stu-id="3ea8c-160">Show user's data after signing in</span></span>

<span data-ttu-id="3ea8c-161">Em seguida, estenda o aplicativo para mostrar os dados do calendário do usuário.</span><span class="sxs-lookup"><span data-stu-id="3ea8c-161">Next, extend the application to show data from the user's calendar.</span></span> <span data-ttu-id="3ea8c-162">Você pode acessar essas informações somente depois que o usuário entrar.</span><span class="sxs-lookup"><span data-stu-id="3ea8c-162">You can access this information only after the user has signed in.</span></span> <span data-ttu-id="3ea8c-163">Para fazer isso, você precisará controlar o estado de entrada do usuário e mostrar os dados do calendário depois que o usuário entrar com a conta da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="3ea8c-163">To do this, you will need to track the  user's sign in state and show the calendar data after the user has signed in with their Microsoft account.</span></span>

#### <a name="track-users-sign-in-state"></a><span data-ttu-id="3ea8c-164">Rastrear o estado de entrada do usuário</span><span class="sxs-lookup"><span data-stu-id="3ea8c-164">Track user's sign in state</span></span>

<span data-ttu-id="3ea8c-165">Para acompanhar o estado de entrada do usuário em seu aplicativo, você usará a combinação de reagir `useState` e `useEffect` conexões com os manipuladores de eventos do provedor.</span><span class="sxs-lookup"><span data-stu-id="3ea8c-165">To track the user's sign in state in your application, you will use the React `useState` and `useEffect` hooks in combination with provider event handlers.</span></span>

1. <span data-ttu-id="3ea8c-166">No editor de códigos, abra o arquivo **src/app. TSX** e estenda a instrução de reagir existente `import` .</span><span class="sxs-lookup"><span data-stu-id="3ea8c-166">In the code editor, open the **src/App.tsx** file and extend the existing React `import` statement.</span></span>

    ```tsx
    import React, { useState, useEffect } from 'react';
    ```

1. <span data-ttu-id="3ea8c-167">Importe os `Provider` `ProviderState` tipos e do Microsoft Graph Toolkit adicionando às importações.</span><span class="sxs-lookup"><span data-stu-id="3ea8c-167">Import the `Provider` and `ProviderState` types from Microsoft Graph Toolkit, by adding to imports.</span></span>

    ```tsx
    import { Providers, ProviderState } from '@microsoft/mgt';
    ```

1. <span data-ttu-id="3ea8c-168">Adicione uma função personalizada nomeada `useIsSignedIn` que permite o acompanhamento do estado de entrada do usuário em seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3ea8c-168">Add a custom function named `useIsSignedIn` that enables tracking the user's sign in state in your application.</span></span>

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

<span data-ttu-id="3ea8c-169">Essa função faz duas coisas.</span><span class="sxs-lookup"><span data-stu-id="3ea8c-169">This function does two things.</span></span> <span data-ttu-id="3ea8c-170">Primeiro, usando o gancho de reagir `useState` , ele habilita o estado de controle dentro de seu componente.</span><span class="sxs-lookup"><span data-stu-id="3ea8c-170">First, using the React `useState` hook, it enables tracking state inside your component.</span></span> <span data-ttu-id="3ea8c-171">Sempre que o estado for alterado, reagir reprocessará seu componente.</span><span class="sxs-lookup"><span data-stu-id="3ea8c-171">Whenever the state changes, React will re-render your component.</span></span> <span data-ttu-id="3ea8c-172">Em segundo lugar, usando o gancho de reagir `useEffect` , ele estende o ciclo de vida do componente ao controlar as alterações no provedor do Microsoft Graph Toolkit e atualizar o componente, se necessário.</span><span class="sxs-lookup"><span data-stu-id="3ea8c-172">Second, using the React `useEffect` hook, it extends the component's lifecycle by tracking changes in the Microsoft Graph Toolkit provider and updating the component if necessary.</span></span>

#### <a name="load-users-calendar-if-user-is-signed-in"></a><span data-ttu-id="3ea8c-173">Carregar calendário do usuário se o usuário estiver conectado</span><span class="sxs-lookup"><span data-stu-id="3ea8c-173">Load user's calendar if user is signed in</span></span>

<span data-ttu-id="3ea8c-174">Agora que você acompanha o estado de entrada do usuário em seu aplicativo, você pode mostrar seu calendário após ele entrar.</span><span class="sxs-lookup"><span data-stu-id="3ea8c-174">Now that you track the user's sign in state in your application, you can show their calendar after they signed in.</span></span>

1. <span data-ttu-id="3ea8c-175">No editor de códigos, abra o arquivo **src/app. TSX** e, dentro da função **app** , adicione:</span><span class="sxs-lookup"><span data-stu-id="3ea8c-175">In the code editor, open the **src/App.tsx** file, and inside the **App** function, add:</span></span>

    ```tsx
    const [isSignedIn] = useIsSignedIn();
    ```

    <span data-ttu-id="3ea8c-176">Isso define uma constante booleana `isSignedIn` , que você pode usar para determinar se o usuário está atualmente conectado ao seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3ea8c-176">This defines a Boolean `isSignedIn` constant, which you can use to determine whether the user is currently signed in to your application.</span></span>

1. <span data-ttu-id="3ea8c-177">Estenda o conteúdo da `return` cláusula com um componente de `div` programação adicional e o Microsoft Graph Toolkit.</span><span class="sxs-lookup"><span data-stu-id="3ea8c-177">Extend the contents of the `return` clause with an additional `div` and the Microsoft Graph Toolkit Agenda component.</span></span>

    ```tsx
    <div>
      {isSignedIn &&
        <Agenda />}
    </div>
    ```

<span data-ttu-id="3ea8c-178">Com essas alterações, o arquivo **src/app. TSX** deve ser semelhante ao seguinte.</span><span class="sxs-lookup"><span data-stu-id="3ea8c-178">With these changes, the **src/App.tsx** file should look like the following.</span></span>

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

### <a name="test-showing-users-calendar-after-they-signed-in"></a><span data-ttu-id="3ea8c-179">Teste mostrando o calendário do usuário depois que ele entrou</span><span class="sxs-lookup"><span data-stu-id="3ea8c-179">Test showing user's calendar after they signed in</span></span>

<span data-ttu-id="3ea8c-180">Com essas alterações, após entrar em seu aplicativo com sua conta da Microsoft, você deve ver seu calendário.</span><span class="sxs-lookup"><span data-stu-id="3ea8c-180">With these changes, after signing in to your application with your Microsoft account, you should see your calendar.</span></span>

1. <span data-ttu-id="3ea8c-181">Para ver as alterações, feche o navegador e abra-o novamente e vá para `https://localhost:3000` .</span><span class="sxs-lookup"><span data-stu-id="3ea8c-181">To see the changes, close the browser and open it again, and go to `https://localhost:3000`.</span></span> <span data-ttu-id="3ea8c-182">Isso é feito porque você alterou o valor da `scopes` propriedade, que afeta o token de acesso solicitado pelo Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3ea8c-182">You do this because you changed the value of the `scopes` property, which affects the access token that you request from Azure AD.</span></span>
1. <span data-ttu-id="3ea8c-183">Escolha o botão **entrar** e entre usando sua conta da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="3ea8c-183">Choose the **Sign In** button and sign in using your Microsoft account.</span></span> <span data-ttu-id="3ea8c-184">Observe as adições à lista de permissões solicitadas no prompt de consentimento.</span><span class="sxs-lookup"><span data-stu-id="3ea8c-184">Notice the additions to the list of permissions requested in the consent prompt.</span></span> <span data-ttu-id="3ea8c-185">Isso ocorre porque você incluiu permissões adicionais na `scope` propriedade.</span><span class="sxs-lookup"><span data-stu-id="3ea8c-185">This is because you included additional permissions in the `scope` property.</span></span>
1. <span data-ttu-id="3ea8c-186">Após a reenvio ao uso do aplicativo, você deve ver informações sobre o usuário atual e seu calendário.</span><span class="sxs-lookup"><span data-stu-id="3ea8c-186">After consenting to the use of the application, you should see information about the current user and their calendar.</span></span>

![Aplicativo concluído](../images/mgt-finished-app.png)

## <a name="next-steps"></a><span data-ttu-id="3ea8c-188">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="3ea8c-188">Next steps</span></span>

- <span data-ttu-id="3ea8c-189">Veja [o que há no Microsoft Graph Toolkit](../overview.md).</span><span class="sxs-lookup"><span data-stu-id="3ea8c-189">See [what's in the Microsoft Graph Toolkit](../overview.md).</span></span>
- <span data-ttu-id="3ea8c-190">Experimente os componentes no [playground](https://mgt.dev).</span><span class="sxs-lookup"><span data-stu-id="3ea8c-190">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="3ea8c-191">Faça uma pergunta sobre o [estouro de pilha](https://aka.ms/mgt-question).</span><span class="sxs-lookup"><span data-stu-id="3ea8c-191">Ask a question on [Stack Overflow](https://aka.ms/mgt-question).</span></span>
- <span data-ttu-id="3ea8c-192">Informe bugs ou deixe uma solicitação de recurso no [GitHub](https://aka.ms/mgt).</span><span class="sxs-lookup"><span data-stu-id="3ea8c-192">Report bugs or leave a feature request on [GitHub](https://aka.ms/mgt).</span></span>
