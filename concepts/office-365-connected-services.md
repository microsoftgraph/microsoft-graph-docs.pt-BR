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
# <a name="call-office-365-services-in-visual-studio-2017-with-the-microsoft-graph-api"></a>Chamar serviços do Office 365 no Visual Studio 2017 com a API do Microsoft Graph

You can use the Connected Services in Visual Studio to configure your app to call the Microsoft Graph API. This article describes how to get a signed in user's profile photo, upload it to OneDrive, and send an email with a sharing link to the photo.

## <a name="get-set-up"></a>Prepare-se

Para usar os serviços conectados do Office 365 com o Microsoft Graph, você precisará fazer o seguinte:

- Download the [Visual Studio 2017 Preview](https://www.visualstudio.com/vs/preview/), if you haven't already. If you're using an earlier version of Visual Studio, you can use Visual Studio 2017 Preview side by side with your current version.

- Get a Microsoft 365 subscription. To get a free trial, join the [Microsoft 365 Developer program](https://developer.microsoft.com/microsoft-365/dev-program).

## <a name="get-the-starter-project"></a>Obter o projeto inicial

Download the [Microsoft Graph ASP.NET Connected Services Sample](https://github.com/microsoftgraph/aspnet-connect-sample/archive/Office365connectedservice.zip). This sample includes the references that you need to authenticate against Microsoft Graph. After you download the starter project, unzip, and open the sample in Visual Studio 2017 Preview.

## <a name="add-the-connected-service"></a>Adicionar o Serviço Conectado

Agora você está pronto para adicionar o serviço Microsoft Graph ao seu projeto do Visual Studio. 

1. No Gerenciador de Soluções, escolha **Serviços Conectados** para abrir a guia Serviços Conectados. 

2. Escolha o provedor de **Acesso aos Serviços do Office 365 com o Microsoft Graph**. Siga o assistente. Selecione as seguintes permissões (você pode alterá-las posteriormente):

    - Nas APIs **Arquivo** defina permissões como **Ter acesso total a seus arquivos**.
    - Nas APIs **Email**, defina permissões como **Enviar email como você**.
    - Nas APIs **Usuário**, defina as permissões como **Conectar e ler o seu perfil**.

## <a name="call-the-microsoft-graph-api"></a>Chamar a API do Microsoft Graph

The starter sample is configured to send a simple email. You can use Microsoft Graph to update the sample to send an email with a link to the signed-in user's profile photo in OneDrive.

1. Acesse 'Models\GraphService.cs', que hospeda o código para chamar o Microsoft Graph.

2. Find and **Uncomment** calls to the SDK in the following methods. This shows how to call Microsoft Graph to get a profile photo, upload a file to OneDrive, and get a sharing link.

    ```csharp
        GetCurrentUserPhotoStream(GraphServiceClient graphClient)
    ```
    
    ```csharp
        UploadFileToOneDrive(GraphServiceClient graphClient, byte[] file)
    ```

    ```csharp
        GetSharingLink(GraphServiceClient graphClient, string Id)
    ```
 
> **Dica:** cada comentário começa com "//Uncomment:"
 

## <a name="run-the-sample"></a>Executar o exemplo
Build and run the sample. Next, choose the **Sign-in** link on the top right, and then choose **Get email address** followed by **Send email**.

Isso enviará um email que inclui um link para sua foto do perfil.

>**Observações:**

>- Se você interromper e executar novamente a amostra do Visual Studio, talvez precise sair explicitamente para que o exemplo funcione.
>- Se você receber uma exceção que indica que o usuário não está autenticado, talvez precise repetir a etapa [Adicionar o Serviço Conectado](#add-the-connected-service).
    

## <a name="explore-the-code"></a>Explore o código

You can now use Visual Studio 2017 to connect to and configure your services. The starter sample creates the scaffolding and references for you.  

O exemplo inicial inclui os seguintes arquivos:

- [Startup.Auth.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/App_Start/Startup.Auth.cs) – autentica o usuário atual e inicializa o cache de token do exemplo.

- Models\\[SessionTokenCache.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/TokenStorage/SessionTokenCache.cs) - Stores the user's token information. You can replace this with your own custom token cache. For more information, see [Caching access tokens in a multitenant application](https://azure.microsoft.com/documentation/articles/guidance-multitenant-identity-token-cache/).

- Models\\[SampleAuthProvider.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Helpers/SampleAuthProvider.cs) – implementa a interface IAuthProvider local e obtém um token de acesso. 

- Helpers\\[SDKHelper.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Helpers/SDKHelper.cs) – inicializa o **GraphServiceClient**, na [Biblioteca do Cliente .NET para Microsoft Graph](https://github.com/microsoftgraph/msgraph-sdk-dotnet), que é usada para interagir com o Microsoft Graph.

- Controllers\\[HomeController.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Controllers/HomeController.cs) – contêm os métodos que usam o **GraphServiceClient** para criar e enviar chamadas para o serviço do Microsoft Graph e processar a resposta.

- Modos de exibição\\Página Inicial\\[Graph.cshtml](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Views/Home/Graph.cshtml) – contêm a interface de usuário da amostra. 


## <a name="need-help"></a>Precisa de ajuda?

If you need help, post your questions on [StackOverflow](https://stackoverflow.com/questions/tagged/microsoftgraph?sort=newest). Tag your post with {microsoftgraph}.

