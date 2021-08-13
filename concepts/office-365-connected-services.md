---
title: Como chamar os serviços do Microsoft 365 no Visual Studio 2017 com a API do Microsoft Graph
description: Você pode usar os serviços conectados no Visual Studio para configurar seu aplicativo para chamar a API do Microsoft Graph. Este artigo descreve como obter a foto de perfil de um usuário conectado, carregá-la no OneDrive e enviar um email com um link de compartilhamento para a foto.
localization_priority: Priority
ms.prod: reports
author: sarahwxy
ms.openlocfilehash: 0a9dcd50126a7de5a27aadd7d47a492d2199f7b652bd5d8657e35b36b9afcef8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54218321"
---
# <a name="call-microsoft-365-services-in-visual-studio-2017-with-the-microsoft-graph-api"></a>Como chamar os serviços do Microsoft 365 no Visual Studio 2017 com a API do Microsoft Graph

Você pode usar os serviços conectados no Visual Studio para configurar seu aplicativo para chamar a API do Microsoft Graph. Este artigo descreve como obter a foto de perfil de um usuário conectado, carregá-la no OneDrive e enviar um email com um link de compartilhamento para a foto.

## <a name="get-set-up"></a>Prepare-se

Para usar os serviços conectados do Office 365 com o Microsoft Graph, você precisará fazer o seguinte:

- Baixe o [Visual Studio 2017 Preview](https://www.visualstudio.com/vs/preview/), caso ainda não tenha feito isso. Se estiver usando uma versão anterior do Visual Studio, você pode usar o Visual Studio 2017 Preview lado a lado com sua versão atual.

- Obtenha uma assinatura do Microsoft 365. Para obter uma avaliação gratuita, entre no [Programa para Desenvolvedores do Microsoft 365](https://developer.microsoft.com/microsoft-365/dev-program).

## <a name="get-the-starter-project"></a>Obter o projeto inicial

Baixe a [Amostra de Serviços Conectados Microsoft Graph ASP.NET](https://github.com/microsoftgraph/aspnet-connect-sample/archive/Office365connectedservice.zip). Este exemplo inclui as referências de que você precisa para autenticar o Microsoft Graph. Depois de baixar o projeto inicial, descompacte e abra a amostra no Visual Studio 2017 Preview.

## <a name="add-the-connected-service"></a>Adicionar o Serviço Conectado

Agora você está pronto para adicionar o serviço Microsoft Graph ao seu projeto do Visual Studio. 

1. No Gerenciador de Soluções, escolha **Serviços Conectados** para abrir a guia Serviços Conectados. 

2. Escolha o provedor de **Acesso aos Serviços do Microsoft 365 com o Microsoft Graph**. Siga o assistente. Selecione as seguintes permissões (você pode alterá-las posteriormente):

    - Nas APIs **Arquivo** defina permissões como **Ter acesso total a seus arquivos**.
    - Nas APIs **Email**, defina permissões como **Enviar email como você**.
    - Nas APIs **Usuário**, defina as permissões como **Conectar e ler o seu perfil**.

## <a name="call-the-microsoft-graph-api"></a>Chamar a API do Microsoft Graph

A amostra inicial é configurada para enviar um email simples. Você pode usar o Microsoft Graph para atualizar a amostra para enviar um email com um link para a foto de perfil do usuário conectado no OneDrive.

1. Acesse 'Models\GraphService.cs', que hospeda o código para chamar o Microsoft Graph.

2. Localizar e **Cancelar Comentários** em chamadas para o SDK nos seguintes métodos. Isso mostra como chamar o Microsoft Graph para obter uma foto de perfil, carregar um arquivo no OneDrive e obter um link de compartilhamento.

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
Criar e executar o exemplo. Em seguida, escolha o link **Entrar** na parte superior direita e escolha **Obter endereço de email** seguido por **Enviar email**.

Isso enviará um email que inclui um link para sua foto do perfil.

>**Observações:**

>- Se você interromper e executar novamente a amostra do Visual Studio, talvez precise sair explicitamente para que o exemplo funcione.
>- Se você receber uma exceção que indica que o usuário não está autenticado, talvez precise repetir a etapa [Adicionar o Serviço Conectado](#add-the-connected-service).
>- Certifique-se de entrar usando uma conta no mesmo domínio que a que você selecionou na etapa **Selecionar Domínio** do assistente.

## <a name="explore-the-code"></a>Explore o código

Agora você pode usar o Visual Studio 2017 para conectar e configurar seus serviços. O exemplo inicial cria a estrutura e as referências para você.  

O exemplo inicial inclui os seguintes arquivos:

- [Startup.Auth.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/App_Start/Startup.Auth.cs) – autentica o usuário atual e inicializa o cache de token do exemplo.

- \\TokenStorage[SessionTokenCache.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/TokenStorage/SessionTokenCache.cs) - Armazena as informações de token do usuário. Você pode substituí-lo por seu próprio cache de token personalizado. Para obter mais informações, confira [Cache de tokens de acesso em um aplicativo multilocatário](/azure/architecture/multitenant-identity/token-cache).

- Helpers\\[SampleAuthProvider.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Helpers/SampleAuthProvider.cs) – implementa a interface IAuthProvider local e obtém um token de acesso. 

- Helpers\\[SDKHelper.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Helpers/SDKHelper.cs) – inicializa o **GraphServiceClient**, na [Biblioteca do Cliente .NET para Microsoft Graph](https://github.com/microsoftgraph/msgraph-sdk-dotnet), que é usada para interagir com o Microsoft Graph.

- Controllers\\[HomeController.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Controllers/HomeController.cs) – contêm os métodos que usam o **GraphServiceClient** para criar e enviar chamadas para o serviço do Microsoft Graph e processar a resposta.

- Modos de exibição\\Página Inicial\\[Graph.cshtml](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Views/Home/Graph.cshtml) – contêm a interface de usuário da amostra. 


## <a name="need-help"></a>Precisa de ajuda?

Se precisar de ajuda, poste suas perguntas no [Microsoft Q&A](/answers/products/m365#microsoft-graph). Marque sua postagem com {microsoft-graph-identity}.
