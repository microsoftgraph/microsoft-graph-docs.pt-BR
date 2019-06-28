---
title: Use o Postman com a API do Microsoft Graph
description: Use a coleção do Microsoft Graph Postman para começar a usar as APIs do Microsoft Graph em questão minutos.
author: jthake-msft
localization_priority: Priority
ms.openlocfilehash: 0a26b444249a6ee85f875b3a88222f4404aaa238
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2019
ms.locfileid: "35242928"
---
# <a name="use-postman-with-the-microsoft-graph-api"></a><span data-ttu-id="a97de-103">Use o Postman com a API do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="a97de-103">Use the Microsoft Graph API</span></span>

<span data-ttu-id="a97de-104">Você pode usar a coleção do Microsoft Graph Postman para começar a usar as APIs do Microsoft Graph em questão minutos.</span><span class="sxs-lookup"><span data-stu-id="a97de-104">You can use the Microsoft Graph Postman collection to get started with Microsoft Graph APIs in minutes.</span></span>

![Imagem do Postman](https://github.com/microsoftgraph/microsoftgraph-postman-collections/blob/master/images/postman.png?raw=true)

<span data-ttu-id="a97de-106">Este artigo explica como começar a usar o Postman e o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="a97de-106">This article explains how to get up and running with Postman and Microsoft Graph.</span></span> <span data-ttu-id="a97de-107">Você também pode explorar as APIs do Microsoft Graph diretamente em seu navegador da Web usando o [Explorador do Graph](https://developer.microsoft.com/pt-BR/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="a97de-107">You can also explore Microsoft Graph APIs directly in your web browser by using [Graph Explorer](https://developer.microsoft.com/en-us/graph/graph-explorer).</span></span>

## <a name="accessing-the-collection"></a><span data-ttu-id="a97de-108">Acessando a coleção</span><span class="sxs-lookup"><span data-stu-id="a97de-108">Accessing the collection</span></span>
<span data-ttu-id="a97de-109">Você pode acessar a coleção no Postman de duas maneiras: adquirindo-o ou contribuindo para ele.</span><span class="sxs-lookup"><span data-stu-id="a97de-109">You can access the collection in Postman in two ways: by consuming it or by contributing to it.</span></span> <span data-ttu-id="a97de-110">Primeiro, o [Postman](https://www.getpostman.com/) precisará estar em execução no seu computador.</span><span class="sxs-lookup"><span data-stu-id="a97de-110">You will need to have [Postman](https://www.getpostman.com/) running on your computer first.</span></span>

### <a name="consume-the-collection"></a><span data-ttu-id="a97de-111">Adquirir a coleção</span><span class="sxs-lookup"><span data-stu-id="a97de-111">Consume the collection</span></span>
<span data-ttu-id="a97de-112">Adquirir a coleção é a maneira mais fácil de começar a usar as APIs do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="a97de-112">Consuming the collection is the easiest way to get started with Microsoft Graph APIs.</span></span> <span data-ttu-id="a97de-113">O [link de compartilhamento do Postman](https://www.getpostman.com/collections/d89a737b5f0c0825898a) iniciará o Postman.</span><span class="sxs-lookup"><span data-stu-id="a97de-113">The [Postman sharing link](https://www.getpostman.com/collections/d89a737b5f0c0825898a) will launch Postman.</span></span>

<span data-ttu-id="a97de-114">A vantagem de usar a coleção compartilhada é que novas solicitações serão exibidas automaticamente, sem a necessidade de etapas adicionais.</span><span class="sxs-lookup"><span data-stu-id="a97de-114">The advantage to using the shared collection is that new requests will automatically show for you without any additional steps.</span></span>

<span data-ttu-id="a97de-115">Após obter a coleção, você precisará configurar as variáveis do ambiente:</span><span class="sxs-lookup"><span data-stu-id="a97de-115">After you have the collection, you'll need to set up the environment variables:</span></span>

1. <span data-ttu-id="a97de-116">Selecione **Arquivo | Importar ...**.</span><span class="sxs-lookup"><span data-stu-id="a97de-116">Choose **File | Import ...**.</span></span>
2. <span data-ttu-id="a97de-117">Selecione **Importar do link**.</span><span class="sxs-lookup"><span data-stu-id="a97de-117">Select **Import From Link**.</span></span>
3. <span data-ttu-id="a97de-118">Copie e cole o seguinte URL e selecione **Importar**.</span><span class="sxs-lookup"><span data-stu-id="a97de-118">Copy and paste the following URL and choose **Import**.</span></span>
 
    ```
    https://raw.githubusercontent.com/microsoftgraph/microsoftgraph-postman-collections/master/Microsoft%20Graph%20v1.0.postman_environment.json
    ```

<span data-ttu-id="a97de-119">Você deverá ver o **ambiente do Microsoft Graph** na lista suspensa do ambiente na parte superior direita, próximo ao ícone de olho.</span><span class="sxs-lookup"><span data-stu-id="a97de-119">You should now see the **Microsoft Graph environment** in the top right environment drop down by the eye icon.</span></span> <span data-ttu-id="a97de-120">Agora, você precisará [configurar o seu ambiente](#using-the-collection).</span><span class="sxs-lookup"><span data-stu-id="a97de-120">Now you need to  [set up your environment](#using-the-collection).</span></span>

### <a name="contribute-to-the-collection"></a><span data-ttu-id="a97de-121">Contribua para a coleção</span><span class="sxs-lookup"><span data-stu-id="a97de-121">Contribute to the collection</span></span>
<span data-ttu-id="a97de-122">Se você desejar contribuir com suas próprias solicitações, você precisará bifurcar o repositório github das [coleções do Microsoft Graph Postman](https://github.com/microsoftgraph/microsoftgraph-postman-collections).</span><span class="sxs-lookup"><span data-stu-id="a97de-122">If you want to contribute your own requests, you will need to fork the [Microsoft Graph Postman collections](https://github.com/microsoftgraph/microsoftgraph-postman-collections) github repo.</span></span> 

<span data-ttu-id="a97de-123">Para detalhes sobre como fazer isso, assista ao vídeo a seguir.</span><span class="sxs-lookup"><span data-stu-id="a97de-123">For details about how to do this, watch the following video.</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/4tg-OBdv_8o]

<span data-ttu-id="a97de-124">Para importar as coleções do Postman:</span><span class="sxs-lookup"><span data-stu-id="a97de-124">To import the Postman collections:</span></span>

1. <span data-ttu-id="a97de-125">Baixe e registre-se no [Postman](https://www.getpostman.com/).</span><span class="sxs-lookup"><span data-stu-id="a97de-125">Download and register for [Postman](https://www.getpostman.com/).</span></span>
2. <span data-ttu-id="a97de-126">Selecione **Arquivo | Importar ...**.</span><span class="sxs-lookup"><span data-stu-id="a97de-126">Choose **File | Import ...**.</span></span>
3. <span data-ttu-id="a97de-127">Selecione **Importar do link**.</span><span class="sxs-lookup"><span data-stu-id="a97de-127">Select **Import From Link**.</span></span>
4. <span data-ttu-id="a97de-128">Cole os dois URLs a seguir e selecione **Importar** após cada um.</span><span class="sxs-lookup"><span data-stu-id="a97de-128">Paste the following two URLs and choose **Import** after each.</span></span>

    ```
      https://raw.githubusercontent.com/microsoftgraph/microsoftgraph-postman-collections/master/Microsoft%20Graph%20v1.0.postman_collection.json
      
    ```
    ```
      https://raw.githubusercontent.com/microsoftgraph/microsoftgraph-postman-collections/master/Microsoft%20Graph%20v1.0.postman_environment.json

    ```

<span data-ttu-id="a97de-129">Você deverá ver a coleção do **Microsoft Graph v1.0** no painel **Coleções**.</span><span class="sxs-lookup"><span data-stu-id="a97de-129">You should now see the **Microsoft Graph v1.0** collection on the **Collections** pane.</span></span>

## <a name="using-the-collection"></a><span data-ttu-id="a97de-130">Usando a coleção</span><span class="sxs-lookup"><span data-stu-id="a97de-130">Using the collection</span></span>
<span data-ttu-id="a97de-131">Após obter a coleção do **Microsoft Graph v1.0** e o **ambiente do Microsoft Graph** no Postman, siga estas etapas.</span><span class="sxs-lookup"><span data-stu-id="a97de-131">After you have the **Microsoft Graph v1.0** collection and the **Microsoftr Graph environment** in Postman, follow these steps.</span></span>

### <a name="set-up-application-api-calls"></a><span data-ttu-id="a97de-132">Configure as chamadas de API do aplicativo</span><span class="sxs-lookup"><span data-stu-id="a97de-132">Set up application API calls</span></span>

1. <span data-ttu-id="a97de-133">Escolha a opção **Sem ambiente** na lista suspensa na parte superior direita.</span><span class="sxs-lookup"><span data-stu-id="a97de-133">Choose the **No environment** drop down in top right corner.</span></span>
2. <span data-ttu-id="a97de-134">Selecione **ambiente do Microsoft Graph**.</span><span class="sxs-lookup"><span data-stu-id="a97de-134">Select **Microsoft Graph environment**.</span></span>
3. <span data-ttu-id="a97de-135">Selecione o ícone de **olho** à direita e, em seguida, **Editar**.</span><span class="sxs-lookup"><span data-stu-id="a97de-135">Choose the **eye** icon to the right and then choose **Edit**.</span></span>
4. <span data-ttu-id="a97de-136">Insira o seu aplicativo da plataforma de identidade da Microsoft nas variáveis **atuais** (e não **iniciais**): **ClientID**, **ClientSecret** e **TenantID**.</span><span class="sxs-lookup"><span data-stu-id="a97de-136">Enter your Microsoft Identity Application in the **current** (not **initial**) variables: **ClientID**, **ClientSecret** and **TenantID**.</span></span> 
 <span data-ttu-id="a97de-137">Para obter mais informações sobre como criar um aplicativo e autorizar o fluxo único do aplicativo, confira a postagem do blog [Usar o Postman para fazer chamadas do Microsoft Graph](https://developer.microsoft.com/en-us/graph/blogs/30daysmsgraph-day-13-postman-to-make-microsoft-graph-calls/).</span><span class="sxs-lookup"><span data-stu-id="a97de-137">For more information about how to create an application and to admin consent the app-only flow, see the [Use Postman to make Microsoft Graph calls](https://developer.microsoft.com/en-us/graph/blogs/30daysmsgraph-day-13-postman-to-make-microsoft-graph-calls/) blog post.</span></span>

5. <span data-ttu-id="a97de-138">Selecione **Atualizar**.</span><span class="sxs-lookup"><span data-stu-id="a97de-138">Select **Update**.</span></span> <span data-ttu-id="a97de-139">Feche a caixa de diálogo **Gerenciar Ambientes**.</span><span class="sxs-lookup"><span data-stu-id="a97de-139">Close the **Manage Environments** dialog box.</span></span> <span data-ttu-id="a97de-140">Na coleção do **Microsoft Graph v1.0 | Aplicativo** no lado esquerdo, selecione **Obter Token de Acesso Único do Aplicativo**.</span><span class="sxs-lookup"><span data-stu-id="a97de-140">In the **MicrosoftGraph v1.0 | Application** collection on left side, choose **Get App-only Access Token**.</span></span> <span data-ttu-id="a97de-141">Em seguida, no lado direito, selecione **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="a97de-141">Then choose **Send** on the right.</span></span>
6. <span data-ttu-id="a97de-142">Expanda a pasta **Aplicativo | Usuários** e selecione **Obter Usuários**.</span><span class="sxs-lookup"><span data-stu-id="a97de-142">Expand the **Application | Users** folder and choose **Get Users**.</span></span> <span data-ttu-id="a97de-143">Em seguida, clique em **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="a97de-143">Then choose **Send**.</span></span>

<span data-ttu-id="a97de-144">Agora você está pronto para usar as coleções do Microsoft Graph v1.0.</span><span class="sxs-lookup"><span data-stu-id="a97de-144">You are now up and running with the Microsoft Graph v1.0 collections.</span></span>

><span data-ttu-id="a97de-145">**Observação:** se você deseja executar outras APIs na coleção, você precisará concordar com as permissões necessárias do seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a97de-145">**Note:** If you want to run other APIs in the collection, you will need to consent the required permissions for your application.</span></span>

### <a name="set-up-on-behalf-of-api-calls"></a><span data-ttu-id="a97de-146">Configurar as chamadas de API em nome de</span><span class="sxs-lookup"><span data-stu-id="a97de-146">Set up on-behalf-of API calls</span></span>
<span data-ttu-id="a97de-147">A maneira mais simples de configurar chamadas de APIs em nome de é fornecer um **UserName** e **UserPassword** nas configurações de ambiente e usar o **Em Nome de um Usuário | Obter Token de Acesso do Usuário**.</span><span class="sxs-lookup"><span data-stu-id="a97de-147">The simplest way to set up on-behalf-of API calls is to provide a **UserName** and **UserPassword** in the environment settings and use the **On Behalf of a User | Get User Access Token**.</span></span> 

><span data-ttu-id="a97de-148">**Importante:** não recomendamos o uso de contas de usuário de produção, pois essas informações são armazenadas diretamente no Postman.</span><span class="sxs-lookup"><span data-stu-id="a97de-148">**Important:** We don't recommend using production user accounts because this information is stored directly in Postman.</span></span> <span data-ttu-id="a97de-149">Também não recomendamos o uso deste método para obter tokens de acesso na produção.</span><span class="sxs-lookup"><span data-stu-id="a97de-149">We also don't  recommend using this approach to obtain access tokens in production.</span></span> <span data-ttu-id="a97de-150">Use-o apenas para fins de teste.</span><span class="sxs-lookup"><span data-stu-id="a97de-150">Use it only for testing purposes.</span></span>

<span data-ttu-id="a97de-151">Se você não deseja armazenar nomes de usuário e senhas em variáveis de ambiente que sincronizam com a sua conta de nuvem do Postman, é possível usar a função **Obter Novo Token de Acesso** para obter um token sem sair do Postman.</span><span class="sxs-lookup"><span data-stu-id="a97de-151">If you don't want to store user names and passwords in environment variables that sync to your Postman cloud account, you can use the  **Get New Access Token** capability to get a token without leaving Postman.</span></span>

1. <span data-ttu-id="a97de-152">Selecione **Em nome de um Usuário | Obter Token de Acesso usando o Postman**.</span><span class="sxs-lookup"><span data-stu-id="a97de-152">Select **On behalf of a User | Get Access Token using Postman**.</span></span>
2. <span data-ttu-id="a97de-153">Selecione a guia **Autorização**.</span><span class="sxs-lookup"><span data-stu-id="a97de-153">Choose the Authorization tab in the Request Editor.</span></span>
3. <span data-ttu-id="a97de-154">Selecione o botão **obter token de acesso**.</span><span class="sxs-lookup"><span data-stu-id="a97de-154">Choose the **get access token** button.</span></span>
4. <span data-ttu-id="a97de-155">Preencha os campos a seguir com os seus valores reais de locatário e aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a97de-155">Fill out the following boxes with your real tenant and application values.</span></span> <span data-ttu-id="a97de-156">Note que aqui você não poderá usar as variáveis de ambiente; você terá que usar os valores reais.</span><span class="sxs-lookup"><span data-stu-id="a97de-156">Note that you cannot use the environment variables here; you have to use the actual values.</span></span> <span data-ttu-id="a97de-157">Eles podem ser encontrados selecionando **EndPoints** na lâmina do aplicativo em portal.azure.com.</span><span class="sxs-lookup"><span data-stu-id="a97de-157">You can find them by selecting **EndPoints** in the application blade in portal.azure.com.</span></span>

    - <span data-ttu-id="a97de-158">URL de retorno de chamada: https://app.getpostman.com/oauth2/callback</span><span class="sxs-lookup"><span data-stu-id="a97de-158">Callback URL: https://app.getpostman.com/oauth2/callback</span></span>
    - <span data-ttu-id="a97de-159">URL de Autenticação: https://login.microsoftonline.com/**TENANTID**/oauth2/v2.0/authorize</span><span class="sxs-lookup"><span data-stu-id="a97de-159">Auth URL: https://login.microsoftonline.com/**TENANTID**/oauth2/v2.0/authorize</span></span>
    - <span data-ttu-id="a97de-160">URL do Token de Acesso: https://login.microsoftonline.com/**TENANTID**/oauth2/v2.0/token</span><span class="sxs-lookup"><span data-stu-id="a97de-160">Access Token URL: https://login.microsoftonline.com/**TENANTID**/oauth2/v2.0/token</span></span>
    - <span data-ttu-id="a97de-161">ID do Cliente: **CLIENTID**</span><span class="sxs-lookup"><span data-stu-id="a97de-161">Client ID: **CLIENTID**</span></span>
    - <span data-ttu-id="a97de-162">Segredo do Cliente: **CLIENTSECRET**</span><span class="sxs-lookup"><span data-stu-id="a97de-162">Client Secret: **CLIENTSECRET**</span></span>
    - <span data-ttu-id="a97de-163">Escopo: https://graph.microsoft.com/.default</span><span class="sxs-lookup"><span data-stu-id="a97de-163">https://graph.microsoft.com/.default</span></span>
    - <span data-ttu-id="a97de-164">Estado: **RANDOMSTRING**</span><span class="sxs-lookup"><span data-stu-id="a97de-164">State: **RANDOMSTRING**</span></span>
 
5. <span data-ttu-id="a97de-165">Selecione **Solicitar Token**.</span><span class="sxs-lookup"><span data-stu-id="a97de-165">Choose **Request Token**.</span></span> <span data-ttu-id="a97de-166">Você deverá ver um prompt de interface de usuário para entrar e autorizar permissões.</span><span class="sxs-lookup"><span data-stu-id="a97de-166">You should see a UI prompt to sign in and consent permissions.</span></span>
6. <span data-ttu-id="a97de-167">Copie o token de acesso, abra as suas variáveis de ambiente e cole-o no campo **UserAccessToken**.</span><span class="sxs-lookup"><span data-stu-id="a97de-167">Copy the access token, open your environment variables, and paste it into the **UserAccessToken** field.</span></span>

<span data-ttu-id="a97de-168">Agora todas as suas solicitações irão funcionar.</span><span class="sxs-lookup"><span data-stu-id="a97de-168">Now all your requests will work.</span></span>
