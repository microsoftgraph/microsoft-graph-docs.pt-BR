---
title: Use o Postman com a API do Microsoft Graph
description: Use a coleção do Microsoft Graph Postman para começar a usar as APIs do Microsoft Graph em questão minutos.
author: jthake-msft
localization_priority: Priority
ms.openlocfilehash: c7029a68314c0a093e0943bcdad46be27155ca25
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556212"
---
# <a name="use-postman-with-the-microsoft-graph-api"></a><span data-ttu-id="23dff-103">Use o Postman com a API do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="23dff-103">Use Postman with the Microsoft Graph API</span></span>

<span data-ttu-id="23dff-104">Você pode usar a coleção do Microsoft Graph Postman para começar a usar as APIs do Microsoft Graph em questão minutos.</span><span class="sxs-lookup"><span data-stu-id="23dff-104">You can use the Microsoft Graph Postman collection to get started with Microsoft Graph APIs in minutes.</span></span>

![Imagem do Postman](https://github.com/microsoftgraph/microsoftgraph-postman-collections/blob/master/images/postman.png?raw=true)

<span data-ttu-id="23dff-106">Este artigo explica como começar a usar o Postman e o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="23dff-106">This article explains how to get up and running with Postman and Microsoft Graph.</span></span> <span data-ttu-id="23dff-107">Você também pode explorar as APIs do Microsoft Graph diretamente em seu navegador da Web usando o [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="23dff-107">You can also explore Microsoft Graph APIs directly in your web browser by using [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>

## <a name="accessing-the-collection"></a><span data-ttu-id="23dff-108">Acessando a coleção</span><span class="sxs-lookup"><span data-stu-id="23dff-108">Accessing the collection</span></span>
<span data-ttu-id="23dff-109">Você pode acessar a coleção no Postman de duas maneiras: adquirindo-o ou contribuindo para ele.</span><span class="sxs-lookup"><span data-stu-id="23dff-109">You can access the collection in Postman in two ways: by consuming it or by contributing to it.</span></span> <span data-ttu-id="23dff-110">Primeiro, o [Postman](https://www.getpostman.com/) precisará estar em execução no seu computador.</span><span class="sxs-lookup"><span data-stu-id="23dff-110">You will need to have [Postman](https://www.getpostman.com/) running on your computer first.</span></span>

### <a name="consume-the-collection"></a><span data-ttu-id="23dff-111">Adquirir a coleção</span><span class="sxs-lookup"><span data-stu-id="23dff-111">Consume the collection</span></span>
<span data-ttu-id="23dff-112">Adquirir a coleção é a maneira mais fácil de começar a usar as APIs do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="23dff-112">Consuming the collection is the easiest way to get started with Microsoft Graph APIs.</span></span> <span data-ttu-id="23dff-113">Para importar as coleções do Postman:</span><span class="sxs-lookup"><span data-stu-id="23dff-113">To import the Postman collections:</span></span>

1. <span data-ttu-id="23dff-114">Baixe e registre-se no [Postman](https://www.getpostman.com/).</span><span class="sxs-lookup"><span data-stu-id="23dff-114">Download and register for [Postman](https://www.getpostman.com/).</span></span>
2. <span data-ttu-id="23dff-115">Selecione **Arquivo | Importar ...**.</span><span class="sxs-lookup"><span data-stu-id="23dff-115">Choose **File | Import ...**.</span></span>
3. <span data-ttu-id="23dff-116">Selecione **Importar do link**.</span><span class="sxs-lookup"><span data-stu-id="23dff-116">Select **Import From Link**.</span></span>
4. <span data-ttu-id="23dff-117">Cole os dois URLs a seguir e selecione **Importar** após cada um.</span><span class="sxs-lookup"><span data-stu-id="23dff-117">Paste the following two URLs and choose **Import** after each.</span></span>

    ```
      https://raw.githubusercontent.com/microsoftgraph/microsoftgraph-postman-collections/master/Microsoft%20Graph.postman_collection.json
      
    ```
    ```
      https://raw.githubusercontent.com/microsoftgraph/microsoftgraph-postman-collections/master/Microsoft%20Graph.postman_environment.json

    ```

<span data-ttu-id="23dff-118">Você deverá ver o **ambiente do Microsoft Graph** na lista suspensa do ambiente na parte superior direita, próximo ao ícone de olho.</span><span class="sxs-lookup"><span data-stu-id="23dff-118">You should now see the **Microsoft Graph environment** in the top right environment drop down by the eye icon.</span></span> <span data-ttu-id="23dff-119">Agora, você precisará [configurar o seu ambiente](#using-the-collection).</span><span class="sxs-lookup"><span data-stu-id="23dff-119">Now you need to  [set up your environment](#using-the-collection).</span></span>

## <a name="using-the-collection"></a><span data-ttu-id="23dff-120">Usando a coleção</span><span class="sxs-lookup"><span data-stu-id="23dff-120">Using the collection</span></span>
<span data-ttu-id="23dff-121">Depois de obter a coleção **Microsoft Graph** e o **ambiente Microsoft Graph** no Postman, siga estas etapas.</span><span class="sxs-lookup"><span data-stu-id="23dff-121">After you have the **Microsoft Graph** collection and the **Microsoft Graph environment** in Postman, follow these steps.</span></span>

### <a name="set-up-application-api-calls"></a><span data-ttu-id="23dff-122">Configure as chamadas de API do aplicativo</span><span class="sxs-lookup"><span data-stu-id="23dff-122">Set up application API calls</span></span>

1. <span data-ttu-id="23dff-123">Escolha a opção **Sem ambiente** na lista suspensa na parte superior direita.</span><span class="sxs-lookup"><span data-stu-id="23dff-123">Choose the **No environment** drop down in top right corner.</span></span>
2. <span data-ttu-id="23dff-124">Selecione **ambiente do Microsoft Graph**.</span><span class="sxs-lookup"><span data-stu-id="23dff-124">Select **Microsoft Graph environment**.</span></span>
3. <span data-ttu-id="23dff-125">Selecione o ícone de **olho** à direita e, em seguida, **Editar**.</span><span class="sxs-lookup"><span data-stu-id="23dff-125">Choose the **eye** icon to the right and then choose **Edit**.</span></span>
4. <span data-ttu-id="23dff-126">Insira o seu aplicativo da plataforma de identidade da Microsoft nas variáveis **atuais** (e não **iniciais**): **ClientID**, **ClientSecret** e **TenantID**.</span><span class="sxs-lookup"><span data-stu-id="23dff-126">Enter your Microsoft Identity Application in the **current** (not **initial**) variables: **ClientID**, **ClientSecret** and **TenantID**.</span></span> 
 <span data-ttu-id="23dff-127">Para obter mais informações sobre como criar um aplicativo e autorizar o fluxo único do aplicativo, confira a postagem do blog [Usar o Postman para fazer chamadas do Microsoft Graph](https://developer.microsoft.com/pt-BR/graph/blogs/30daysmsgraph-day-13-postman-to-make-microsoft-graph-calls/).</span><span class="sxs-lookup"><span data-stu-id="23dff-127">For more information about how to create an application and to admin consent the app-only flow, see the [Use Postman to make Microsoft Graph calls](https://developer.microsoft.com/pt-BR/graph/blogs/30daysmsgraph-day-13-postman-to-make-microsoft-graph-calls/) blog post.</span></span>

5. <span data-ttu-id="23dff-128">Selecione **Atualizar**.</span><span class="sxs-lookup"><span data-stu-id="23dff-128">Select **Update**.</span></span> <span data-ttu-id="23dff-129">Feche a caixa de diálogo **Gerenciar Ambientes**.</span><span class="sxs-lookup"><span data-stu-id="23dff-129">Close the **Manage Environments** dialog box.</span></span> <span data-ttu-id="23dff-130">Na coleção do **Microsoft Graph | Aplicativo** no lado esquerdo, selecione **Obter Token de Acesso Único do Aplicativo**.</span><span class="sxs-lookup"><span data-stu-id="23dff-130">In the **MicrosoftGraph | Application** collection on left side, choose **Get App-only Access Token**.</span></span> <span data-ttu-id="23dff-131">Em seguida, no lado direito, selecione **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="23dff-131">Then choose **Send** on the right.</span></span>
6. <span data-ttu-id="23dff-132">Expanda a pasta **Aplicativo | Usuários** e selecione **Obter Usuários**.</span><span class="sxs-lookup"><span data-stu-id="23dff-132">Expand the **Application | Users** folder and choose **Get Users**.</span></span> <span data-ttu-id="23dff-133">Em seguida, clique em **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="23dff-133">Then choose **Send**.</span></span>

<span data-ttu-id="23dff-134">Agora você está pronto para usar as coleções do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="23dff-134">You are now up and running with the Microsoft Graph collections.</span></span>

><span data-ttu-id="23dff-135">**Observação:** se você deseja executar outras APIs na coleção, você precisará concordar com as permissões necessárias do seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="23dff-135">**Note:** If you want to run other APIs in the collection, you will need to consent the required permissions for your application.</span></span>

### <a name="set-up-on-behalf-of-api-calls"></a><span data-ttu-id="23dff-136">Configurar as chamadas de API em nome de</span><span class="sxs-lookup"><span data-stu-id="23dff-136">Set up on-behalf-of API calls</span></span>
<span data-ttu-id="23dff-137">A maneira mais simples de configurar chamadas de APIs em nome de é fornecer um **UserName** e **UserPassword** nas configurações de ambiente e usar o **Em Nome de um Usuário | Obter Token de Acesso do Usuário**.</span><span class="sxs-lookup"><span data-stu-id="23dff-137">The simplest way to set up on-behalf-of API calls is to provide a **UserName** and **UserPassword** in the environment settings and use the **On Behalf of a User | Get User Access Token**.</span></span> 

><span data-ttu-id="23dff-138">**Importante:** não recomendamos o uso de contas de usuário de produção, pois essas informações são armazenadas diretamente no Postman.</span><span class="sxs-lookup"><span data-stu-id="23dff-138">**Important:** We don't recommend using production user accounts because this information is stored directly in Postman.</span></span> <span data-ttu-id="23dff-139">Também não recomendamos o uso deste método para obter tokens de acesso na produção.</span><span class="sxs-lookup"><span data-stu-id="23dff-139">We also don't  recommend using this approach to obtain access tokens in production.</span></span> <span data-ttu-id="23dff-140">Use-o apenas para fins de teste.</span><span class="sxs-lookup"><span data-stu-id="23dff-140">Use it only for testing purposes.</span></span>

<span data-ttu-id="23dff-141">Se você não deseja armazenar nomes de usuário e senhas em variáveis de ambiente que sincronizam com a sua conta de nuvem do Postman, é possível usar a função **Obter Novo Token de Acesso** para obter um token sem sair do Postman.</span><span class="sxs-lookup"><span data-stu-id="23dff-141">If you don't want to store user names and passwords in environment variables that sync to your Postman cloud account, you can use the  **Get New Access Token** capability to get a token without leaving Postman.</span></span>

1. <span data-ttu-id="23dff-142">Selecione **Em nome de um Usuário | Obter Token de Acesso usando o Postman**.</span><span class="sxs-lookup"><span data-stu-id="23dff-142">Select **On behalf of a User | Get Access Token using Postman**.</span></span>
2. <span data-ttu-id="23dff-143">Selecione a guia **Autorização**.</span><span class="sxs-lookup"><span data-stu-id="23dff-143">Choose the **Authorization** tab.</span></span>
3. <span data-ttu-id="23dff-144">Selecione o botão **obter token de acesso**.</span><span class="sxs-lookup"><span data-stu-id="23dff-144">Choose the **get access token** button.</span></span>
4. <span data-ttu-id="23dff-145">Preencha os campos a seguir com os seus valores reais de locatário e aplicativo.</span><span class="sxs-lookup"><span data-stu-id="23dff-145">Fill out the following boxes with your real tenant and application values.</span></span> <span data-ttu-id="23dff-146">Note que aqui você não poderá usar as variáveis de ambiente; você terá que usar os valores reais.</span><span class="sxs-lookup"><span data-stu-id="23dff-146">Note that you cannot use the environment variables here; you have to use the actual values.</span></span> <span data-ttu-id="23dff-147">Eles podem ser encontrados selecionando **EndPoints** na lâmina do aplicativo em portal.azure.com.</span><span class="sxs-lookup"><span data-stu-id="23dff-147">You can find them by selecting **EndPoints** in the application blade in portal.azure.com.</span></span>

    - <span data-ttu-id="23dff-148">URL de retorno de chamada: https://app.getpostman.com/oauth2/callback</span><span class="sxs-lookup"><span data-stu-id="23dff-148">Callback URL: https://app.getpostman.com/oauth2/callback</span></span>
    - <span data-ttu-id="23dff-149">URL de Autenticação: https://login.microsoftonline.com/**TENANTID**/oauth2/v2.0/authorize</span><span class="sxs-lookup"><span data-stu-id="23dff-149">Auth URL: https://login.microsoftonline.com/**TENANTID**/oauth2/v2.0/authorize</span></span>
    - <span data-ttu-id="23dff-150">URL do Token de Acesso: https://login.microsoftonline.com/**TENANTID**/oauth2/v2.0/token</span><span class="sxs-lookup"><span data-stu-id="23dff-150">Access Token URL: https://login.microsoftonline.com/**TENANTID**/oauth2/v2.0/token</span></span>
    - <span data-ttu-id="23dff-151">ID do Cliente: **CLIENTID**</span><span class="sxs-lookup"><span data-stu-id="23dff-151">Client ID: **CLIENTID**</span></span>
    - <span data-ttu-id="23dff-152">Segredo do Cliente: **CLIENTSECRET**</span><span class="sxs-lookup"><span data-stu-id="23dff-152">Client Secret: **CLIENTSECRET**</span></span>
    - <span data-ttu-id="23dff-153">Escopo: https://graph.microsoft.com/.default</span><span class="sxs-lookup"><span data-stu-id="23dff-153">Scope: https://graph.microsoft.com/.default</span></span>
    - <span data-ttu-id="23dff-154">Estado: **RANDOMSTRING**</span><span class="sxs-lookup"><span data-stu-id="23dff-154">State: **RANDOMSTRING**</span></span>
 
5. <span data-ttu-id="23dff-155">Selecione **Solicitar Token**.</span><span class="sxs-lookup"><span data-stu-id="23dff-155">Choose **Request Token**.</span></span> <span data-ttu-id="23dff-156">Você deverá ver um prompt de interface de usuário para entrar e autorizar permissões.</span><span class="sxs-lookup"><span data-stu-id="23dff-156">You should see a UI prompt to sign in and consent permissions.</span></span>
6. <span data-ttu-id="23dff-157">Copie o token de acesso, abra as suas variáveis de ambiente e cole-o no campo **UserAccessToken**.</span><span class="sxs-lookup"><span data-stu-id="23dff-157">Copy the access token, open your environment variables, and paste it into the **UserAccessToken** field.</span></span>

<span data-ttu-id="23dff-158">Agora todas as suas solicitações irão funcionar.</span><span class="sxs-lookup"><span data-stu-id="23dff-158">Now all your requests will work.</span></span>


### <a name="contribute-to-the-collection"></a><span data-ttu-id="23dff-159">Contribua para a coleção</span><span class="sxs-lookup"><span data-stu-id="23dff-159">Contribute to the collection</span></span>
<span data-ttu-id="23dff-160">Se você desejar contribuir com suas próprias solicitações, você precisará bifurcar o repositório github das [coleções do Microsoft Graph Postman](https://github.com/microsoftgraph/microsoftgraph-postman-collections).</span><span class="sxs-lookup"><span data-stu-id="23dff-160">If you want to contribute your own requests, you will need to fork the [Microsoft Graph Postman collections](https://github.com/microsoftgraph/microsoftgraph-postman-collections) github repo.</span></span> 

<span data-ttu-id="23dff-161">Para detalhes sobre como fazer isso, assista ao vídeo a seguir.</span><span class="sxs-lookup"><span data-stu-id="23dff-161">For details about how to do this, watch the following video.</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/4tg-OBdv_8o]
