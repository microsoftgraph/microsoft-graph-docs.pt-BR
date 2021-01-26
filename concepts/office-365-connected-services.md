---
title: Como chamar os serviços do Microsoft 365 no Visual Studio 2017 com a API do Microsoft Graph
description: Você pode usar os serviços conectados no Visual Studio para configurar seu aplicativo para chamar a API do Microsoft Graph. Este artigo descreve como obter a foto de perfil de um usuário conectado, carregá-la no OneDrive e enviar um email com um link de compartilhamento para a foto.
localization_priority: Priority
ms.prod: reports
author: sarahwxy
ms.openlocfilehash: ce2d4bc8ccaa2ebae79c4d65ca243aeb9d489b54
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982282"
---
# <a name="call-microsoft-365-services-in-visual-studio-2017-with-the-microsoft-graph-api"></a><span data-ttu-id="5e710-104">Como chamar os serviços do Microsoft 365 no Visual Studio 2017 com a API do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="5e710-104">Call Microsoft 365 services in Visual Studio 2017 with the Microsoft Graph API</span></span>

<span data-ttu-id="5e710-p102">Você pode usar os serviços conectados no Visual Studio para configurar seu aplicativo para chamar a API do Microsoft Graph. Este artigo descreve como obter a foto de perfil de um usuário conectado, carregá-la no OneDrive e enviar um email com um link de compartilhamento para a foto.</span><span class="sxs-lookup"><span data-stu-id="5e710-p102">You can use the Connected Services in Visual Studio to configure your app to call the Microsoft Graph API. This article describes how to get a signed in user's profile photo, upload it to OneDrive, and send an email with a sharing link to the photo.</span></span>

## <a name="get-set-up"></a><span data-ttu-id="5e710-107">Prepare-se</span><span class="sxs-lookup"><span data-stu-id="5e710-107">Get set up</span></span>

<span data-ttu-id="5e710-108">Para usar os serviços conectados do Office 365 com o Microsoft Graph, você precisará fazer o seguinte:</span><span class="sxs-lookup"><span data-stu-id="5e710-108">To use the Office 365 Connected Services with Microsoft Graph, you'll need to do the following:</span></span>

- <span data-ttu-id="5e710-p103">Baixe o [Visual Studio 2017 Preview](https://www.visualstudio.com/vs/preview/), caso ainda não tenha feito isso. Se estiver usando uma versão anterior do Visual Studio, você pode usar o Visual Studio 2017 Preview lado a lado com sua versão atual.</span><span class="sxs-lookup"><span data-stu-id="5e710-p103">Download the [Visual Studio 2017 Preview](https://www.visualstudio.com/vs/preview/), if you haven't already. If you're using an earlier version of Visual Studio, you can use Visual Studio 2017 Preview side by side with your current version.</span></span>

- <span data-ttu-id="5e710-p104">Obtenha uma assinatura do Microsoft 365. Para obter uma avaliação gratuita, entre no [Programa para Desenvolvedores do Microsoft 365](https://developer.microsoft.com/microsoft-365/dev-program).</span><span class="sxs-lookup"><span data-stu-id="5e710-p104">Get a Microsoft 365 subscription. To get a free trial, join the [Microsoft 365 Developer program](https://developer.microsoft.com/microsoft-365/dev-program).</span></span>

## <a name="get-the-starter-project"></a><span data-ttu-id="5e710-113">Obter o projeto inicial</span><span class="sxs-lookup"><span data-stu-id="5e710-113">Get the starter project</span></span>

<span data-ttu-id="5e710-p105">Baixe a [Amostra de Serviços Conectados Microsoft Graph ASP.NET](https://github.com/microsoftgraph/aspnet-connect-sample/archive/Office365connectedservice.zip). Este exemplo inclui as referências de que você precisa para autenticar o Microsoft Graph. Depois de baixar o projeto inicial, descompacte e abra a amostra no Visual Studio 2017 Preview.</span><span class="sxs-lookup"><span data-stu-id="5e710-p105">Download the [Microsoft Graph ASP.NET Connected Services Sample](https://github.com/microsoftgraph/aspnet-connect-sample/archive/Office365connectedservice.zip). This sample includes the references that you need to authenticate against Microsoft Graph. After you download the starter project, unzip, and open the sample in Visual Studio 2017 Preview.</span></span>

## <a name="add-the-connected-service"></a><span data-ttu-id="5e710-117">Adicionar o Serviço Conectado</span><span class="sxs-lookup"><span data-stu-id="5e710-117">Add the Connected Service</span></span>

<span data-ttu-id="5e710-118">Agora você está pronto para adicionar o serviço Microsoft Graph ao seu projeto do Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="5e710-118">You're now ready to add the Microsoft Graph service to your Visual Studio project.</span></span> 

1. <span data-ttu-id="5e710-119">No Gerenciador de Soluções, escolha **Serviços Conectados** para abrir a guia Serviços Conectados.</span><span class="sxs-lookup"><span data-stu-id="5e710-119">In Solution Explorer, choose **Connected Services** to open the Connected Services tab.</span></span> 

2. <span data-ttu-id="5e710-120">Escolha o provedor de **Acesso aos Serviços do Microsoft 365 com o Microsoft Graph**.</span><span class="sxs-lookup"><span data-stu-id="5e710-120">Choose the **Access Microsoft 365 services with Microsoft Graph** provider.</span></span> <span data-ttu-id="5e710-121">Siga o assistente.</span><span class="sxs-lookup"><span data-stu-id="5e710-121">Follow the wizard.</span></span> <span data-ttu-id="5e710-122">Selecione as seguintes permissões (você pode alterá-las posteriormente):</span><span class="sxs-lookup"><span data-stu-id="5e710-122">Select the following permissions (you can change the permissions later):</span></span>

    - <span data-ttu-id="5e710-123">Nas APIs **Arquivo** defina permissões como **Ter acesso total a seus arquivos**.</span><span class="sxs-lookup"><span data-stu-id="5e710-123">For the **File** APIs, set permissions to **Have full access to your files**.</span></span>
    - <span data-ttu-id="5e710-124">Nas APIs **Email**, defina permissões como **Enviar email como você**.</span><span class="sxs-lookup"><span data-stu-id="5e710-124">For the **Mail** APIs, set permissions to **Send mail as you**.</span></span>
    - <span data-ttu-id="5e710-125">Nas APIs **Usuário**, defina as permissões como **Conectar e ler o seu perfil**.</span><span class="sxs-lookup"><span data-stu-id="5e710-125">For the **User** APIs, set permissions to **Sign you in and read your profile**.</span></span>

## <a name="call-the-microsoft-graph-api"></a><span data-ttu-id="5e710-126">Chamar a API do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="5e710-126">Call the Microsoft Graph API</span></span>

<span data-ttu-id="5e710-p107">A amostra inicial é configurada para enviar um email simples. Você pode usar o Microsoft Graph para atualizar a amostra para enviar um email com um link para a foto de perfil do usuário conectado no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="5e710-p107">The starter sample is configured to send a simple email. You can use Microsoft Graph to update the sample to send an email with a link to the signed-in user's profile photo in OneDrive.</span></span>

1. <span data-ttu-id="5e710-129">Acesse 'Models\GraphService.cs', que hospeda o código para chamar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="5e710-129">Go to 'Models\GraphService.cs', which hosts the code to call Microsoft Graph.</span></span>

2. <span data-ttu-id="5e710-p108">Localizar e **Cancelar Comentários** em chamadas para o SDK nos seguintes métodos. Isso mostra como chamar o Microsoft Graph para obter uma foto de perfil, carregar um arquivo no OneDrive e obter um link de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="5e710-p108">Find and **Uncomment** calls to the SDK in the following methods. This shows how to call Microsoft Graph to get a profile photo, upload a file to OneDrive, and get a sharing link.</span></span>

    ```csharp
        GetCurrentUserPhotoStream(GraphServiceClient graphClient)
    ```
    
    ```csharp
        UploadFileToOneDrive(GraphServiceClient graphClient, byte[] file)
    ```

    ```csharp
        GetSharingLink(GraphServiceClient graphClient, string Id)
    ```
 
> <span data-ttu-id="5e710-132">**Dica:** cada comentário começa com "//Uncomment:"</span><span class="sxs-lookup"><span data-stu-id="5e710-132">**Tip:** Each comment starts with '//Uncomment:'</span></span>
 

## <a name="run-the-sample"></a><span data-ttu-id="5e710-133">Executar o exemplo</span><span class="sxs-lookup"><span data-stu-id="5e710-133">Run the sample</span></span>
<span data-ttu-id="5e710-p109">Criar e executar o exemplo. Em seguida, escolha o link **Entrar** na parte superior direita e escolha **Obter endereço de email** seguido por **Enviar email**.</span><span class="sxs-lookup"><span data-stu-id="5e710-p109">Build and run the sample. Next, choose the **Sign-in** link on the top right, and then choose **Get email address** followed by **Send email**.</span></span>

<span data-ttu-id="5e710-136">Isso enviará um email que inclui um link para sua foto do perfil.</span><span class="sxs-lookup"><span data-stu-id="5e710-136">This will send an email that includes a link to your profile photo.</span></span>

><span data-ttu-id="5e710-137">**Observações:**</span><span class="sxs-lookup"><span data-stu-id="5e710-137">**Notes:**</span></span>

>- <span data-ttu-id="5e710-138">Se você interromper e executar novamente a amostra do Visual Studio, talvez precise sair explicitamente para que o exemplo funcione.</span><span class="sxs-lookup"><span data-stu-id="5e710-138">If you stop and rerun the sample from Visual Studio, you might need to explicitly sign out for the sample to work.</span></span>
>- <span data-ttu-id="5e710-139">Se você receber uma exceção que indica que o usuário não está autenticado, talvez precise repetir a etapa [Adicionar o Serviço Conectado](#add-the-connected-service).</span><span class="sxs-lookup"><span data-stu-id="5e710-139">If you get an exception that indicates that the User is not authenticated, you might need to repeat the [Add the Connected Service](#add-the-connected-service) step.</span></span>
    

## <a name="explore-the-code"></a><span data-ttu-id="5e710-140">Explore o código</span><span class="sxs-lookup"><span data-stu-id="5e710-140">Explore the code</span></span>

<span data-ttu-id="5e710-p110">Agora você pode usar o Visual Studio 2017 para conectar e configurar seus serviços. O exemplo inicial cria a estrutura e as referências para você.</span><span class="sxs-lookup"><span data-stu-id="5e710-p110">You can now use Visual Studio 2017 to connect to and configure your services. The starter sample creates the scaffolding and references for you.</span></span>  

<span data-ttu-id="5e710-143">O exemplo inicial inclui os seguintes arquivos:</span><span class="sxs-lookup"><span data-stu-id="5e710-143">The starter sample includes the following files:</span></span>

- <span data-ttu-id="5e710-144">[Startup.Auth.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/App_Start/Startup.Auth.cs) – autentica o usuário atual e inicializa o cache de token do exemplo.</span><span class="sxs-lookup"><span data-stu-id="5e710-144">[Startup.Auth.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/App_Start/Startup.Auth.cs) - Authenticates the current user and initializes the sample's token cache.</span></span>

- <span data-ttu-id="5e710-p111">Models\\[SessionTokenCache.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/TokenStorage/SessionTokenCache.cs) – armazena as informações de token do usuário. Você pode substituir pelo seu próprio cache de token personalizado. Para saber mais, veja [Armazenamento de tokens de acesso em cache em um aplicativo de vários locatários](/azure/architecture/multitenant-identity/token-cache).</span><span class="sxs-lookup"><span data-stu-id="5e710-p111">Models\\[SessionTokenCache.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/TokenStorage/SessionTokenCache.cs) - Stores the user's token information. You can replace this with your own custom token cache. For more information, see [Caching access tokens in a multitenant application](/azure/architecture/multitenant-identity/token-cache).</span></span>

- <span data-ttu-id="5e710-148">Models\\[SampleAuthProvider.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Helpers/SampleAuthProvider.cs) – implementa a interface IAuthProvider local e obtém um token de acesso.</span><span class="sxs-lookup"><span data-stu-id="5e710-148">Models\\[SampleAuthProvider.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Helpers/SampleAuthProvider.cs) - Implements the local IAuthProvider interface, and gets an access token.</span></span> 

- <span data-ttu-id="5e710-149">Helpers\\[SDKHelper.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Helpers/SDKHelper.cs) – inicializa o **GraphServiceClient**, na [Biblioteca do Cliente .NET para Microsoft Graph](https://github.com/microsoftgraph/msgraph-sdk-dotnet), que é usada para interagir com o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="5e710-149">Helpers\\[SDKHelper.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Helpers/SDKHelper.cs) - Initializes the **GraphServiceClient** from the [Microsoft Graph .NET Client Library](https://github.com/microsoftgraph/msgraph-sdk-dotnet) that is used to interact with the Microsoft Graph.</span></span>

- <span data-ttu-id="5e710-150">Controllers\\[HomeController.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Controllers/HomeController.cs) – contêm os métodos que usam o **GraphServiceClient** para criar e enviar chamadas para o serviço do Microsoft Graph e processar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5e710-150">Controllers\\[HomeController.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Controllers/HomeController.cs) - Contains methods that use the **GraphServiceClient** to build and send calls to the Microsoft Graph service and to process the response.</span></span>

- <span data-ttu-id="5e710-151">Modos de exibição\\Página Inicial\\[Graph.cshtml](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Views/Home/Graph.cshtml) – contêm a interface de usuário da amostra.</span><span class="sxs-lookup"><span data-stu-id="5e710-151">Views\\Home\\[Graph.cshtml](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Views/Home/Graph.cshtml) - Contains the UI for the sample.</span></span> 


## <a name="need-help"></a><span data-ttu-id="5e710-152">Precisa de ajuda?</span><span class="sxs-lookup"><span data-stu-id="5e710-152">Need help?</span></span>

<span data-ttu-id="5e710-p112">Se precisar de ajuda, publique suas perguntas no [StackOverflow](https://stackoverflow.com/questions/tagged/microsoftgraph?sort=newest). Marque sua postagem com {microsoftgraph}.</span><span class="sxs-lookup"><span data-stu-id="5e710-p112">If you need help, post your questions on [StackOverflow](https://stackoverflow.com/questions/tagged/microsoftgraph?sort=newest). Tag your post with {microsoftgraph}.</span></span>