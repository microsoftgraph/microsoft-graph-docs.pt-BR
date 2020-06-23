---
title: Chamar serviços do Office 365 no Visual Studio 2017 com a API do Microsoft Graph
description: You can use the Connected Services in Visual Studio to configure your app to call the Microsoft Graph API. This article describes how to get a signed in user's profile photo, upload it to OneDrive, and send an email with a sharing link to the photo.
localization_priority: Priority
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: a051b4011ab2efef7179680bb5bcbab1e717d8cc
ms.sourcegitcommit: d0f88dcb7f4c72196c45a00cccbb9fc30b715637
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42926663"
---
# <a name="call-office-365-services-in-visual-studio-2017-with-the-microsoft-graph-api"></a><span data-ttu-id="57d7c-104">Chamar serviços do Office 365 no Visual Studio 2017 com a API do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="57d7c-104">Call Office 365 services in Visual Studio 2017 with the Microsoft Graph API</span></span>

<span data-ttu-id="57d7c-105">You can use the Connected Services in Visual Studio to configure your app to call the Microsoft Graph API.</span><span class="sxs-lookup"><span data-stu-id="57d7c-105">You can use the Connected Services in Visual Studio to configure your app to call the Microsoft Graph API.</span></span> <span data-ttu-id="57d7c-106">This article describes how to get a signed in user's profile photo, upload it to OneDrive, and send an email with a sharing link to the photo.</span><span class="sxs-lookup"><span data-stu-id="57d7c-106">This article describes how to get a signed in user's profile photo, upload it to OneDrive, and send an email with a sharing link to the photo.</span></span>

## <a name="get-set-up"></a><span data-ttu-id="57d7c-107">Prepare-se</span><span class="sxs-lookup"><span data-stu-id="57d7c-107">Get set up</span></span>

<span data-ttu-id="57d7c-108">Para usar os serviços conectados do Office 365 com o Microsoft Graph, você precisará fazer o seguinte:</span><span class="sxs-lookup"><span data-stu-id="57d7c-108">To use the Office 365 Connected Services with Microsoft Graph, you'll need to do the following:</span></span>

- <span data-ttu-id="57d7c-109">Download the [Visual Studio 2017 Preview](https://www.visualstudio.com/vs/preview/), if you haven't already.</span><span class="sxs-lookup"><span data-stu-id="57d7c-109">Download the [Visual Studio 2017 Preview](https://www.visualstudio.com/vs/preview/), if you haven't already.</span></span> <span data-ttu-id="57d7c-110">If you're using an earlier version of Visual Studio, you can use Visual Studio 2017 Preview side by side with your current version.</span><span class="sxs-lookup"><span data-stu-id="57d7c-110">If you're using an earlier version of Visual Studio, you can use Visual Studio 2017 Preview side by side with your current version.</span></span>

- <span data-ttu-id="57d7c-111">Get a Microsoft 365 subscription.</span><span class="sxs-lookup"><span data-stu-id="57d7c-111">Get a Microsoft 365 subscription.</span></span> <span data-ttu-id="57d7c-112">To get a free trial, join the [Microsoft 365 Developer program](https://developer.microsoft.com/microsoft-365/dev-program).</span><span class="sxs-lookup"><span data-stu-id="57d7c-112">To get a free trial, join the [Microsoft 365 Developer program](https://developer.microsoft.com/microsoft-365/dev-program).</span></span>

## <a name="get-the-starter-project"></a><span data-ttu-id="57d7c-113">Obter o projeto inicial</span><span class="sxs-lookup"><span data-stu-id="57d7c-113">Get the starter project</span></span>

<span data-ttu-id="57d7c-114">Download the [Microsoft Graph ASP.NET Connected Services Sample](https://github.com/microsoftgraph/aspnet-connect-sample/archive/Office365connectedservice.zip).</span><span class="sxs-lookup"><span data-stu-id="57d7c-114">Download the [Microsoft Graph ASP.NET Connected Services Sample](https://github.com/microsoftgraph/aspnet-connect-sample/archive/Office365connectedservice.zip).</span></span> <span data-ttu-id="57d7c-115">This sample includes the references that you need to authenticate against Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="57d7c-115">This sample includes the references that you need to authenticate against Microsoft Graph.</span></span> <span data-ttu-id="57d7c-116">After you download the starter project, unzip, and open the sample in Visual Studio 2017 Preview.</span><span class="sxs-lookup"><span data-stu-id="57d7c-116">After you download the starter project, unzip, and open the sample in Visual Studio 2017 Preview.</span></span>

## <a name="add-the-connected-service"></a><span data-ttu-id="57d7c-117">Adicionar o Serviço Conectado</span><span class="sxs-lookup"><span data-stu-id="57d7c-117">Add the Connected Service</span></span>

<span data-ttu-id="57d7c-118">Agora você está pronto para adicionar o serviço Microsoft Graph ao seu projeto do Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="57d7c-118">You're now ready to add the Microsoft Graph service to your Visual Studio project.</span></span> 

1. <span data-ttu-id="57d7c-119">No Gerenciador de Soluções, escolha **Serviços Conectados** para abrir a guia Serviços Conectados.</span><span class="sxs-lookup"><span data-stu-id="57d7c-119">In Solution Explorer, choose **Connected Services** to open the Connected Services tab.</span></span> 

2. <span data-ttu-id="57d7c-120">Escolha o provedor de **Acesso aos Serviços do Office 365 com o Microsoft Graph**.</span><span class="sxs-lookup"><span data-stu-id="57d7c-120">Choose the **Access Office 365 Services with Microsoft Graph** provider.</span></span> <span data-ttu-id="57d7c-121">Siga o assistente.</span><span class="sxs-lookup"><span data-stu-id="57d7c-121">Follow the wizard.</span></span> <span data-ttu-id="57d7c-122">Selecione as seguintes permissões (você pode alterá-las posteriormente):</span><span class="sxs-lookup"><span data-stu-id="57d7c-122">Select the following permissions (you can change the permissions later):</span></span>

    - <span data-ttu-id="57d7c-123">Nas APIs **Arquivo** defina permissões como **Ter acesso total a seus arquivos**.</span><span class="sxs-lookup"><span data-stu-id="57d7c-123">For the **File** APIs, set permissions to **Have full access to your files**.</span></span>
    - <span data-ttu-id="57d7c-124">Nas APIs **Email**, defina permissões como **Enviar email como você**.</span><span class="sxs-lookup"><span data-stu-id="57d7c-124">For the **Mail** APIs, set permissions to **Send mail as you**.</span></span>
    - <span data-ttu-id="57d7c-125">Nas APIs **Usuário**, defina as permissões como **Conectar e ler o seu perfil**.</span><span class="sxs-lookup"><span data-stu-id="57d7c-125">For the **User** APIs, set permissions to **Sign you in and read your profile**.</span></span>

## <a name="call-the-microsoft-graph-api"></a><span data-ttu-id="57d7c-126">Chamar a API do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="57d7c-126">Call the Microsoft Graph API</span></span>

<span data-ttu-id="57d7c-127">The starter sample is configured to send a simple email.</span><span class="sxs-lookup"><span data-stu-id="57d7c-127">The starter sample is configured to send a simple email.</span></span> <span data-ttu-id="57d7c-128">You can use Microsoft Graph to update the sample to send an email with a link to the signed-in user's profile photo in OneDrive.</span><span class="sxs-lookup"><span data-stu-id="57d7c-128">You can use Microsoft Graph to update the sample to send an email with a link to the signed-in user's profile photo in OneDrive.</span></span>

1. <span data-ttu-id="57d7c-129">Acesse 'Models\GraphService.cs', que hospeda o código para chamar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="57d7c-129">Go to 'Models\GraphService.cs', which hosts the code to call Microsoft Graph.</span></span>

2. <span data-ttu-id="57d7c-130">Find and **Uncomment** calls to the SDK in the following methods.</span><span class="sxs-lookup"><span data-stu-id="57d7c-130">Find and **Uncomment** calls to the SDK in the following methods.</span></span> <span data-ttu-id="57d7c-131">This shows how to call Microsoft Graph to get a profile photo, upload a file to OneDrive, and get a sharing link.</span><span class="sxs-lookup"><span data-stu-id="57d7c-131">This shows how to call Microsoft Graph to get a profile photo, upload a file to OneDrive, and get a sharing link.</span></span>

    ```csharp
        GetCurrentUserPhotoStream(GraphServiceClient graphClient)
    ```
    
    ```csharp
        UploadFileToOneDrive(GraphServiceClient graphClient, byte[] file)
    ```

    ```csharp
        GetSharingLink(GraphServiceClient graphClient, string Id)
    ```
 
> <span data-ttu-id="57d7c-132">**Dica:** cada comentário começa com "//Uncomment:"</span><span class="sxs-lookup"><span data-stu-id="57d7c-132">**Tip:** Each comment starts with '//Uncomment:'</span></span>
 

## <a name="run-the-sample"></a><span data-ttu-id="57d7c-133">Executar o exemplo</span><span class="sxs-lookup"><span data-stu-id="57d7c-133">Run the sample</span></span>
<span data-ttu-id="57d7c-134">Build and run the sample.</span><span class="sxs-lookup"><span data-stu-id="57d7c-134">Build and run the sample.</span></span> <span data-ttu-id="57d7c-135">Next, choose the **Sign-in** link on the top right, and then choose **Get email address** followed by **Send email**.</span><span class="sxs-lookup"><span data-stu-id="57d7c-135">Next, choose the **Sign-in** link on the top right, and then choose **Get email address** followed by **Send email**.</span></span>

<span data-ttu-id="57d7c-136">Isso enviará um email que inclui um link para sua foto do perfil.</span><span class="sxs-lookup"><span data-stu-id="57d7c-136">This will send an email that includes a link to your profile photo.</span></span>

><span data-ttu-id="57d7c-137">**Observações:**</span><span class="sxs-lookup"><span data-stu-id="57d7c-137">**Notes:**</span></span>

>- <span data-ttu-id="57d7c-138">Se você interromper e executar novamente a amostra do Visual Studio, talvez precise sair explicitamente para que o exemplo funcione.</span><span class="sxs-lookup"><span data-stu-id="57d7c-138">If you stop and rerun the sample from Visual Studio, you might need to explicitly sign out for the sample to work.</span></span>
>- <span data-ttu-id="57d7c-139">Se você receber uma exceção que indica que o usuário não está autenticado, talvez precise repetir a etapa [Adicionar o Serviço Conectado](#add-the-connected-service).</span><span class="sxs-lookup"><span data-stu-id="57d7c-139">If you get an exception that indicates that the User is not authenticated, you might need to repeat the [Add the Connected Service](#add-the-connected-service) step.</span></span>
    

## <a name="explore-the-code"></a><span data-ttu-id="57d7c-140">Explore o código</span><span class="sxs-lookup"><span data-stu-id="57d7c-140">Explore the code</span></span>

<span data-ttu-id="57d7c-141">You can now use Visual Studio 2017 to connect to and configure your services.</span><span class="sxs-lookup"><span data-stu-id="57d7c-141">You can now use Visual Studio 2017 to connect to and configure your services.</span></span> <span data-ttu-id="57d7c-142">The starter sample creates the scaffolding and references for you.</span><span class="sxs-lookup"><span data-stu-id="57d7c-142">The starter sample creates the scaffolding and references for you.</span></span>  

<span data-ttu-id="57d7c-143">O exemplo inicial inclui os seguintes arquivos:</span><span class="sxs-lookup"><span data-stu-id="57d7c-143">The starter sample includes the following files:</span></span>

- <span data-ttu-id="57d7c-144">[Startup.Auth.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/App_Start/Startup.Auth.cs) – autentica o usuário atual e inicializa o cache de token do exemplo.</span><span class="sxs-lookup"><span data-stu-id="57d7c-144">[Startup.Auth.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/App_Start/Startup.Auth.cs) - Authenticates the current user and initializes the sample's token cache.</span></span>

- <span data-ttu-id="57d7c-145">Models\\[SessionTokenCache.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/TokenStorage/SessionTokenCache.cs) - Stores the user's token information.</span><span class="sxs-lookup"><span data-stu-id="57d7c-145">Models\\[SessionTokenCache.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/TokenStorage/SessionTokenCache.cs) - Stores the user's token information.</span></span> <span data-ttu-id="57d7c-146">You can replace this with your own custom token cache.</span><span class="sxs-lookup"><span data-stu-id="57d7c-146">You can replace this with your own custom token cache.</span></span> <span data-ttu-id="57d7c-147">For more information, see [Caching access tokens in a multitenant application](https://azure.microsoft.com/documentation/articles/guidance-multitenant-identity-token-cache/).</span><span class="sxs-lookup"><span data-stu-id="57d7c-147">For more information, see [Caching access tokens in a multitenant application](https://azure.microsoft.com/documentation/articles/guidance-multitenant-identity-token-cache/).</span></span>

- <span data-ttu-id="57d7c-148">Models\\[SampleAuthProvider.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Helpers/SampleAuthProvider.cs) – implementa a interface IAuthProvider local e obtém um token de acesso.</span><span class="sxs-lookup"><span data-stu-id="57d7c-148">Models\\[SampleAuthProvider.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Helpers/SampleAuthProvider.cs) - Implements the local IAuthProvider interface, and gets an access token.</span></span> 

- <span data-ttu-id="57d7c-149">Helpers\\[SDKHelper.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Helpers/SDKHelper.cs) – inicializa o **GraphServiceClient**, na [Biblioteca do Cliente .NET para Microsoft Graph](https://github.com/microsoftgraph/msgraph-sdk-dotnet), que é usada para interagir com o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="57d7c-149">Helpers\\[SDKHelper.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Helpers/SDKHelper.cs) - Initializes the **GraphServiceClient** from the [Microsoft Graph .NET Client Library](https://github.com/microsoftgraph/msgraph-sdk-dotnet) that is used to interact with the Microsoft Graph.</span></span>

- <span data-ttu-id="57d7c-150">Controllers\\[HomeController.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Controllers/HomeController.cs) – contêm os métodos que usam o **GraphServiceClient** para criar e enviar chamadas para o serviço do Microsoft Graph e processar a resposta.</span><span class="sxs-lookup"><span data-stu-id="57d7c-150">Controllers\\[HomeController.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Controllers/HomeController.cs) - Contains methods that use the **GraphServiceClient** to build and send calls to the Microsoft Graph service and to process the response.</span></span>

- <span data-ttu-id="57d7c-151">Modos de exibição\\Página Inicial\\[Graph.cshtml](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Views/Home/Graph.cshtml) – contêm a interface de usuário da amostra.</span><span class="sxs-lookup"><span data-stu-id="57d7c-151">Views\\Home\\[Graph.cshtml](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Views/Home/Graph.cshtml) - Contains the UI for the sample.</span></span> 


## <a name="need-help"></a><span data-ttu-id="57d7c-152">Precisa de ajuda?</span><span class="sxs-lookup"><span data-stu-id="57d7c-152">Need help?</span></span>

<span data-ttu-id="57d7c-153">If you need help, post your questions on [StackOverflow](https://stackoverflow.com/questions/tagged/microsoftgraph?sort=newest).</span><span class="sxs-lookup"><span data-stu-id="57d7c-153">If you need help, post your questions on [StackOverflow](https://stackoverflow.com/questions/tagged/microsoftgraph?sort=newest).</span></span> <span data-ttu-id="57d7c-154">Tag your post with {microsoftgraph}.</span><span class="sxs-lookup"><span data-stu-id="57d7c-154">Tag your post with {microsoftgraph}.</span></span>

