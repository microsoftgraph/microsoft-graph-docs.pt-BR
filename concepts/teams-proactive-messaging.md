---
title: Mensagens pró-ativas usando um bot no Microsoft Teams
description: Enviar uma mensagem proativa para um usuário do Microsoft Teams com um aplicativo personalizado instalando primeiro o bot usando o Microsoft Graph.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e8222931709ab504106c86209ec186140b4a2087
ms.sourcegitcommit: fc9edd17aebed91768e31416e1c1ee0b64d5ce06
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/27/2019
ms.locfileid: "39621646"
---
# <a name="proactive-messaging-using-a-bot-in-microsoft-teams"></a><span data-ttu-id="b73bd-103">Mensagens pró-ativas usando um bot no Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="b73bd-103">Proactive messaging using a bot in Microsoft Teams</span></span>

<span data-ttu-id="b73bd-104">Uma mensagem proativa é uma mensagem enviada a um usuário do Microsoft Teams sem um usuário que inicia a conversa.</span><span class="sxs-lookup"><span data-stu-id="b73bd-104">A proactive message is a message sent to a Microsoft Teams user without a user initiating the conversation.</span></span> <span data-ttu-id="b73bd-105">Aplicativos personalizados no Microsoft Teams podem enviar mensagens pró-ativas para usuários usando um bot.</span><span class="sxs-lookup"><span data-stu-id="b73bd-105">Custom apps in Microsoft Teams can send proactive messages to users using a bot.</span></span> <span data-ttu-id="b73bd-106">No entanto, para fazer isso, o bot precisa ser instalado como um aplicativo pessoal ou em uma equipe da qual o usuário é membro.</span><span class="sxs-lookup"><span data-stu-id="b73bd-106">However, to do so, the bot needs to be installed either as a personal app, or in a team that the user is a member of.</span></span> <span data-ttu-id="b73bd-107">Esse requisito pode ser proibitivo em cenários em que você precisará proativamente enviar uma mensagem a um grupo de usuários que podem ou não ter o aplicativo Teams instalado.</span><span class="sxs-lookup"><span data-stu-id="b73bd-107">This requirement can be prohibitive in scenarios where you need to proactively message a group of users that might or might not have the Teams app installed.</span></span>

<span data-ttu-id="b73bd-108">Este artigo descreve como você pode combinar o Microsoft Graph com um aplicativo do Microsoft Teams para instalar o aplicativo para seus usuários e, em seguida, usar seu aplicativo Teams para enviar uma mensagem pró-ativa, sem exigir que ele instale o aplicativo manualmente.</span><span class="sxs-lookup"><span data-stu-id="b73bd-108">This article outlines how you can combine Microsoft Graph with a Microsoft Teams app to install the app for your users and then use your Teams app to send them a proactive message, without requiring them to manually install the app.</span></span>

<span data-ttu-id="b73bd-109">Em um nível alto, você precisará:</span><span class="sxs-lookup"><span data-stu-id="b73bd-109">At a high level, you'll need to:</span></span>

* [<span data-ttu-id="b73bd-110">Criar seu aplicativo e bot do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="b73bd-110">Create your Teams app and bot</span></span>](#create-your-teams-app-and-bot)
* [<span data-ttu-id="b73bd-111">Implantar seu aplicativo no catálogo de aplicativos do locatário</span><span class="sxs-lookup"><span data-stu-id="b73bd-111">Deploy your app to your tenant app catalog</span></span>](#deploy-your-app-to-your-tenant-app-catalog)
* [<span data-ttu-id="b73bd-112">Instalar o aplicativo para seus usuários</span><span class="sxs-lookup"><span data-stu-id="b73bd-112">Install the app for your users</span></span>](#install-the-app-for-your-users)

## <a name="create-your-teams-app-and-bot"></a><span data-ttu-id="b73bd-113">Criar seu aplicativo e bot do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="b73bd-113">Create your Teams app and bot</span></span>

<span data-ttu-id="b73bd-114">Se você ainda não tiver um aplicativo do Microsoft Teams com um bot que possa enviar a mensagem, você precisará criar um.</span><span class="sxs-lookup"><span data-stu-id="b73bd-114">If you do not already have a Microsoft Teams app with a bot that can send the message, you'll need to create one.</span></span> <span data-ttu-id="b73bd-115">Consulte [Add bots to Teams apps](https://docs.microsoft.com/microsoftteams/platform/concepts/bots/bots-overview) na documentação da plataforma do teams.</span><span class="sxs-lookup"><span data-stu-id="b73bd-115">See [Add bots to Teams apps](https://docs.microsoft.com/microsoftteams/platform/concepts/bots/bots-overview) in the Teams platform documentation.</span></span> <span data-ttu-id="b73bd-116">Para obter informações sobre como criar um bot para mensagens proativas, consulte [Proactive Messaging for bots](https://docs.microsoft.com/microsoftteams/platform/concepts/bots/bot-conversations/bots-conv-proactive).</span><span class="sxs-lookup"><span data-stu-id="b73bd-116">For specifics about creating a bot for proactive messaging, see [Proactive messaging for bots](https://docs.microsoft.com/microsoftteams/platform/concepts/bots/bot-conversations/bots-conv-proactive).</span></span>

<span data-ttu-id="b73bd-117">Você também pode usar o [modelo de aplicativo Company Communicator](https://github.com/OfficeDev/microsoft-teams-company-communicator-app) como um bom ponto de partida para seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b73bd-117">You can also use the [Company Communicator app template](https://github.com/OfficeDev/microsoft-teams-company-communicator-app) as a good starting point for your app.</span></span> <span data-ttu-id="b73bd-118">Este modelo de aplicativo é um aplicativo Microsoft Teams pronto para produção capaz de criar, agendar e distribuir mensagens em toda a empresa.</span><span class="sxs-lookup"><span data-stu-id="b73bd-118">This app template is a production-ready Microsoft Teams app capable of creating, scheduling, and distributing company-wide messages.</span></span>

<span data-ttu-id="b73bd-119">Ao criar seu aplicativo, certifique-se de anotar o `id` que você usa em seu manifesto de aplicativo; Você precisará dele para instalar o aplicativo em uma etapa posterior.</span><span class="sxs-lookup"><span data-stu-id="b73bd-119">When creating your app, make sure that you take note of the `id` you use in your application manifest; you'll need it to install the app in a subsequent step.</span></span>

<span data-ttu-id="b73bd-120">Se você estiver fazendo isso para uma organização de grande porte, as mensagens de boas-vindas do seu bot podem ser limitadas.</span><span class="sxs-lookup"><span data-stu-id="b73bd-120">If you're doing this for a large organization, the welcome messages from your bot might get throttled.</span></span> <span data-ttu-id="b73bd-121">Se possível, execute as instalações em lotes e implemente a funcionalidade de back-out no bot.</span><span class="sxs-lookup"><span data-stu-id="b73bd-121">If possible, perform the installations in batches, and implement back-off functionality in your bot.</span></span> <span data-ttu-id="b73bd-122">Para obter detalhes, consulte [tratamento da limitação da taxa](/microsoftteams/platform/concepts/bots/rate-limit).</span><span class="sxs-lookup"><span data-stu-id="b73bd-122">For details, see [handling rate limiting](/microsoftteams/platform/concepts/bots/rate-limit).</span></span>

## <a name="deploy-your-app-to-your-tenant-app-catalog"></a><span data-ttu-id="b73bd-123">Implantar seu aplicativo no catálogo de aplicativos do locatário</span><span class="sxs-lookup"><span data-stu-id="b73bd-123">Deploy your app to your tenant app catalog</span></span>

<span data-ttu-id="b73bd-124">O Microsoft Graph só pode instalar aplicativos que foram adicionados ao catálogo de aplicativos de locatários ou estão disponíveis no repositório de aplicativos públicos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="b73bd-124">Microsoft Graph can only install apps that have been added to your tenant app catalog, or are available in the public Microsoft Teams app store.</span></span> <span data-ttu-id="b73bd-125">Se você estiver trabalhando com um novo aplicativo, será necessário verificar se ele é o [Catálogo de aplicativos do locatário](https://docs.microsoft.com/microsoftteams/platform/publishing/apps-publish#microsoft-teams-tenant-app-catalog).</span><span class="sxs-lookup"><span data-stu-id="b73bd-125">If you're working with a new app, you'll need to make sure it is [tenant app catalog](https://docs.microsoft.com/microsoftteams/platform/publishing/apps-publish#microsoft-teams-tenant-app-catalog).</span></span>

## <a name="install-the-app-for-your-users"></a><span data-ttu-id="b73bd-126">Instalar o aplicativo para seus usuários</span><span class="sxs-lookup"><span data-stu-id="b73bd-126">Install the app for your users</span></span>

<span data-ttu-id="b73bd-127">Para instalar o aplicativo Teams para seus usuários, primeiro você precisará garantir que o seu aplicativo do Microsoft Graph tenha as permissões corretas – você precisará de User. ReadWrite. All ou Directory. ReadWrite. All para instalar o aplicativo Teams.</span><span class="sxs-lookup"><span data-stu-id="b73bd-127">To install the Teams app for your users, you'll first need to ensure that your Microsoft Graph application has the right permissions – you'll need User.ReadWrite.All or Directory.ReadWrite.All to install the Teams app.</span></span> <span data-ttu-id="b73bd-128">Você também precisará de chat. Read. All para uma etapa posterior.</span><span class="sxs-lookup"><span data-stu-id="b73bd-128">You'll also need Chat.Read.All for a subsequent step.</span></span> <span data-ttu-id="b73bd-129">As duas permissões exigirão o consentimento do administrador e você precisará usar permissões de aplicativo, em vez de usuário delegadas, porque você instalará aplicativos para usuários que não são de sua conta.</span><span class="sxs-lookup"><span data-stu-id="b73bd-129">Both permissions will require admin consent, and you'll need to use application permissions rather than user delegated because you will be installing apps to users other than yourself.</span></span>

### <a name="check-to-see-if-the-app-is-already-installed"></a><span data-ttu-id="b73bd-130">Verifique se o aplicativo já está instalado</span><span class="sxs-lookup"><span data-stu-id="b73bd-130">Check to see if the app is already installed</span></span>

<span data-ttu-id="b73bd-131">Primeiro, convém verificar se o aplicativo de equipes já está instalado para os usuários dos quais você deseja instalá-lo, conforme mostrado no exemplo.</span><span class="sxs-lookup"><span data-stu-id="b73bd-131">First, you'll want to check to see if your Teams app is already installed for the users you want to install it from, as shown in the example.</span></span>

```http
GET /users/{user-id}/teamwork/installedApps?$expand=teamsAppDefinition&$filter=teamsAppDefinition/teamsAppId eq '{teamsAppid}'
```

<span data-ttu-id="b73bd-132">Em `{teamsAppId}` que é `id` o manifesto do aplicativo Teams que você fez anotar anteriormente.</span><span class="sxs-lookup"><span data-stu-id="b73bd-132">Where `{teamsAppId}` is the `id` in the Teams app manifest that you made note of previously.</span></span> <span data-ttu-id="b73bd-133">Observe que isso pode ser diferente das chamadas `appid` para o Microsoft Graph e do seu `botId`.</span><span class="sxs-lookup"><span data-stu-id="b73bd-133">Note that this might be different from your `appid` for Microsoft Graph calls, and from your `botId`.</span></span> <span data-ttu-id="b73bd-134">Você pode achar útil instalar manualmente o aplicativo para um usuário e testar a chamada em relação a esse usuário para garantir que você tem o valor correto `id` .</span><span class="sxs-lookup"><span data-stu-id="b73bd-134">You might find it useful to manually install the app for a user and test the call against that user to ensure that you've got the correct `id` value.</span></span>

<span data-ttu-id="b73bd-135">A chamada retornará uma matriz vazia se o aplicativo não estiver instalado ou uma matriz com um único [teamsAppInstallation](/graph/api/resources/teamsappinstallation?view=graph-rest-beta) se já estiver instalada.</span><span class="sxs-lookup"><span data-stu-id="b73bd-135">The call will return an empty array if the app is not installed, or an array with a single [teamsAppInstallation](/graph/api/resources/teamsappinstallation?view=graph-rest-beta) if it is already installed.</span></span>

### <a name="install-the-app"></a><span data-ttu-id="b73bd-136">Instalar o aplicativo</span><span class="sxs-lookup"><span data-stu-id="b73bd-136">Install the app</span></span>

<span data-ttu-id="b73bd-137">Se o aplicativo ainda não estiver instalado para esse usuário, você poderá instalá-lo, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="b73bd-137">If the app is not already installed for that user, you can then install it as shown in the following example.</span></span>

```http
POST /users/{user-id}/teamwork/installedApps
{
   "teamsApp@odata.bind" : "https://graph.microsoft.com/beta/appCatalogs/teamsApps/{teamsAppid}"
}
```

<span data-ttu-id="b73bd-138">Para obter mais informações, consulte [install App for User](/graph/api/user-add-teamsappinstallation?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="b73bd-138">For more information, see [Install app for user](/graph/api/user-add-teamsappinstallation?view=graph-rest-beta).</span></span>

<span data-ttu-id="b73bd-139">Se o usuário tiver o Microsoft Teams em execução, ele poderá ou não ver a instalação do aplicativo imediatamente – talvez seja necessário reiniciar o aplicativo para ver a instalação.</span><span class="sxs-lookup"><span data-stu-id="b73bd-139">If the user has Microsoft Teams running, they might or might not see the app installation right away – they might need to restart the app to see the installation.</span></span>

## <a name="get-the-chat-thread-id"></a><span data-ttu-id="b73bd-140">Obter a ID do thread de chat</span><span class="sxs-lookup"><span data-stu-id="b73bd-140">Get the chat thread ID</span></span>

<span data-ttu-id="b73bd-141">Quando o aplicativo é instalado para o usuário, o bot receberá um `conversationUpdate` evento que conterá as informações necessárias para enviar a mensagem proativa.</span><span class="sxs-lookup"><span data-stu-id="b73bd-141">When the app is installed for the user, the bot will get receive a `conversationUpdate` event that will contain the necessary information for it to send the proactive message.</span></span> <span data-ttu-id="b73bd-142">Para mais informações, consulte [eventos de bot](https://docs.microsoft.com/microsoftteams/platform/concepts/bots/bots-notifications).</span><span class="sxs-lookup"><span data-stu-id="b73bd-142">For more information, see [Bot events](https://docs.microsoft.com/microsoftteams/platform/concepts/bots/bots-notifications).</span></span>

<span data-ttu-id="b73bd-143">Se você perder o `chatThreadId`, poderá encontrá-lo novamente chamando:</span><span class="sxs-lookup"><span data-stu-id="b73bd-143">If you lose the `chatThreadId`, you can find it again by calling:</span></span>

```http
GET /users/{user-id}/chats?$filter=installedApps/any(a:a/teamsApp/id eq '{teamsAppid}')
```

<span data-ttu-id="b73bd-144">A propriedade **ID** do resultado é a ID chatThread.</span><span class="sxs-lookup"><span data-stu-id="b73bd-144">The **id** property of the result is the chatThread ID.</span></span>

## <a name="sending-the-message"></a><span data-ttu-id="b73bd-145">Envio da mensagem</span><span class="sxs-lookup"><span data-stu-id="b73bd-145">Sending the message</span></span>

<span data-ttu-id="b73bd-146">Agora que seu bot tem as informações necessárias, você pode [Enviar uma mensagem proativa](https://docs.microsoft.com/microsoftteams/platform/concepts/bots/bot-conversations/bots-conv-proactive).</span><span class="sxs-lookup"><span data-stu-id="b73bd-146">Now that your bot has the necessary information, you can [send a proactive message](https://docs.microsoft.com/microsoftteams/platform/concepts/bots/bot-conversations/bots-conv-proactive).</span></span>

## <a name="c-sample"></a><span data-ttu-id="b73bd-147">Exemplo de C#</span><span class="sxs-lookup"><span data-stu-id="b73bd-147">C# sample</span></span>

<span data-ttu-id="b73bd-148">Consulte https://github.com/microsoftgraph/contoso-airlines-teams-sample/tree/nkramer-promsg (Observe a ramificação).</span><span class="sxs-lookup"><span data-stu-id="b73bd-148">See https://github.com/microsoftgraph/contoso-airlines-teams-sample/tree/nkramer-promsg (note the branch).</span></span>
<span data-ttu-id="b73bd-149">O código interessante está `InstallAppToAllUsers()` no [GraphService.cs](https://github.com/microsoftgraph/contoso-airlines-teams-sample/blob/nkramer-promsg/project/Models/GraphService.cs).</span><span class="sxs-lookup"><span data-stu-id="b73bd-149">Interesting code is in `InstallAppToAllUsers()` in [GraphService.cs](https://github.com/microsoftgraph/contoso-airlines-teams-sample/blob/nkramer-promsg/project/Models/GraphService.cs).</span></span>
