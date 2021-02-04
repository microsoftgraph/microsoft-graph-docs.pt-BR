---
title: Enviar notificações de feed de atividades aos usuários no Microsoft Teams
description: Envie notificações de feed de atividades aos usuários no Microsoft Teams usando o aplicativo Teams e o Microsoft Graph.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 940ffba39293a3b01df67c47b6ff6b5e09821767
ms.sourcegitcommit: d02c438bcd58e8f64bfcd5fba0b40e436b46570e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/04/2021
ms.locfileid: "50101892"
---
# <a name="send-activity-feed-notifications-to-users-in-microsoft-teams"></a><span data-ttu-id="70a10-103">Enviar notificações de feed de atividades aos usuários no Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="70a10-103">Send activity feed notifications to users in Microsoft Teams</span></span>

<span data-ttu-id="70a10-104">O feed de atividades do Microsoft Teams permite que os usuários triagem itens que exigem atenção notificando-os sobre alterações.</span><span class="sxs-lookup"><span data-stu-id="70a10-104">The Microsoft Teams activity feed enables users to triage items that require attention by notifying them of changes.</span></span> <span data-ttu-id="70a10-105">Você pode usar as APIs de notificação de feed de atividades no Microsoft Graph para estender essa funcionalidade para seus aplicativos.</span><span class="sxs-lookup"><span data-stu-id="70a10-105">You can use the activity feed notification APIs in Microsoft Graph to extend this functionality to your apps.</span></span> <span data-ttu-id="70a10-106">Isso permite que seus aplicativos forneçam experiências mais completas e envolvam melhor os usuários, ajudando a mantê-los atualizados com as alterações nas ferramentas e nos fluxos de trabalho que eles usam.</span><span class="sxs-lookup"><span data-stu-id="70a10-106">This allows your apps to provide richer experiences and better engage users by helping to keep them up to date with changes in the tools and workflows they use.</span></span>

## <a name="understanding-the-basics-of-activity-feed-notification"></a><span data-ttu-id="70a10-107">Noções básicas da notificação de feed de atividades</span><span class="sxs-lookup"><span data-stu-id="70a10-107">Understanding the basics of activity feed notification</span></span>

<span data-ttu-id="70a10-108">As notificações de feed de atividades no Microsoft Teams são compostas por vários bits de informações, exibidas juntas, conforme mostrado na imagem a seguir.</span><span class="sxs-lookup"><span data-stu-id="70a10-108">Activity feed notifications in Microsoft Teams are comprised of multiple bits of information, displayed together, as shown in the following image.</span></span>

![Imagem mostrando componentes de uma notificação de feed de atividades](images/teams-activityfeednotifications/notificationtemplate.png)

<span data-ttu-id="70a10-110">Os componentes incluem:</span><span class="sxs-lookup"><span data-stu-id="70a10-110">The components include:</span></span>
- <span data-ttu-id="70a10-111">O ator que iniciou a atividade</span><span class="sxs-lookup"><span data-stu-id="70a10-111">The actor who initiated the activity</span></span>
- <span data-ttu-id="70a10-112">Um ícone que representa o tipo de atividade</span><span class="sxs-lookup"><span data-stu-id="70a10-112">An icon that represents the activity type</span></span>
- <span data-ttu-id="70a10-113">O motivo pelo qual o ator fez a atividade</span><span class="sxs-lookup"><span data-stu-id="70a10-113">The reason the actor did the activity</span></span>
- <span data-ttu-id="70a10-114">Uma visualização de texto</span><span class="sxs-lookup"><span data-stu-id="70a10-114">A text preview</span></span>
- <span data-ttu-id="70a10-115">Um carimbo de data/hora</span><span class="sxs-lookup"><span data-stu-id="70a10-115">A time stamp</span></span>
- <span data-ttu-id="70a10-116">O local da atividade</span><span class="sxs-lookup"><span data-stu-id="70a10-116">The location of the activity</span></span>

<span data-ttu-id="70a10-117">O exemplo a seguir mostra como esses componentes juntos fornecem os detalhes sobre uma notificação.</span><span class="sxs-lookup"><span data-stu-id="70a10-117">The following example shows how these components together provide the details about a notification.</span></span> <span data-ttu-id="70a10-118">Este exemplo é uma notificação sobre um usuário mencionado em uma comunidade do Yammer.</span><span class="sxs-lookup"><span data-stu-id="70a10-118">This example is a notification about a user mentioned in a Yammer community.</span></span>

![Exemplo de notificação de actifity do Yammer](images/teams-activityfeednotifications/examplefeednotification.png)

## <a name="requirements-for-using-the-activity-feed-notification-apis"></a><span data-ttu-id="70a10-120">Requisitos para usar as APIs de notificação do feed de atividades</span><span class="sxs-lookup"><span data-stu-id="70a10-120">Requirements for using the activity feed notification APIs</span></span>

<span data-ttu-id="70a10-121">As APIs de feed de atividades funcionam com um [aplicativo do Teams.](/microsoftteams/platform/overview)</span><span class="sxs-lookup"><span data-stu-id="70a10-121">Activity feed APIs work with a [Teams app](/microsoftteams/platform/overview).</span></span> <span data-ttu-id="70a10-122">A seguir estão os requisitos para o envio de notificações do feed de atividades:</span><span class="sxs-lookup"><span data-stu-id="70a10-122">The following are the requirements for sending activity feed notifications:</span></span>

- <span data-ttu-id="70a10-123">O manifesto do aplicativo Teams deve ter a ID de aplicativo do Azure AD adicionada à `webApplicationInfo` seção.</span><span class="sxs-lookup"><span data-stu-id="70a10-123">The Teams app manifest must have the Azure AD app ID added to the `webApplicationInfo` section.</span></span> <span data-ttu-id="70a10-124">Para obter detalhes, consulte [o esquema de manifesto.](/microsoftteams/platform/resources/schema/manifest-schema)</span><span class="sxs-lookup"><span data-stu-id="70a10-124">For details, see [manifest schema](/microsoftteams/platform/resources/schema/manifest-schema).</span></span>
- <span data-ttu-id="70a10-125">Os tipos de atividade devem ser declarados na `activities` seção.</span><span class="sxs-lookup"><span data-stu-id="70a10-125">Activity types must be declared in the `activities` section.</span></span> <span data-ttu-id="70a10-126">Para obter detalhes, consulte [o esquema de manifesto.](/microsoftteams/platform/resources/schema/manifest-schema)</span><span class="sxs-lookup"><span data-stu-id="70a10-126">For details, see [manifest schema](/microsoftteams/platform/resources/schema/manifest-schema).</span></span>
- <span data-ttu-id="70a10-127">O aplicativo Teams deve ser instalado para o destinatário, pessoalmente, ou em uma [equipe](/graph/api/resources/team?preserve-view=true) ou [chat](/graph/api/resources/chat?preserve-view=true) do que ele faz parte.</span><span class="sxs-lookup"><span data-stu-id="70a10-127">The Teams app must be installed for the recipient, either personally, or in a [team](/graph/api/resources/team?preserve-view=true) or [chat](/graph/api/resources/chat?preserve-view=true) they are part of.</span></span> <span data-ttu-id="70a10-128">Para saber mais, confira a [instalação do aplicativo Teams.](/graph/api/resources/teamsappinstallation?preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="70a10-128">For more information, see [Teams app installation](/graph/api/resources/teamsappinstallation?preserve-view=true).</span></span>

### <a name="teams-app-manifest-changes"></a><span data-ttu-id="70a10-129">Alterações no manifesto do aplicativo Teams</span><span class="sxs-lookup"><span data-stu-id="70a10-129">Teams app manifest changes</span></span>

<span data-ttu-id="70a10-130">Esta seção descreve as alterações que precisam ser adicionadas ao manifesto do aplicativo Teams.</span><span class="sxs-lookup"><span data-stu-id="70a10-130">This section describes the changes that need to be added to Teams app manifest.</span></span> <span data-ttu-id="70a10-131">Observe que você deve estar usando a versão [do manifesto do aplicativo Teams](/microsoftteams/platform/resources/schema/manifest-schema) ou `1.7` superior.</span><span class="sxs-lookup"><span data-stu-id="70a10-131">Note that you must be using the [Teams app manifest](/microsoftteams/platform/resources/schema/manifest-schema) version `1.7` or greater.</span></span>

```json
"$schema": "https://developer.microsoft.com/json-schemas/teams/v1.7/MicrosoftTeams.schema.json",
"manifestVersion": "1.7",
````

#### <a name="webapplicationinfo-section-changes"></a><span data-ttu-id="70a10-132">Alterações na seção webApplicationInfo</span><span class="sxs-lookup"><span data-stu-id="70a10-132">webApplicationInfo section changes</span></span>

```json
"webApplicationInfo":
{
    "id": "a3111f15-658e-457c-9689-fd20fe907330",
    "resource": "https://contosoapp.com"
}
```

|<span data-ttu-id="70a10-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="70a10-133">Parameter</span></span>|<span data-ttu-id="70a10-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="70a10-134">Type</span></span>|<span data-ttu-id="70a10-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="70a10-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70a10-136">id</span><span class="sxs-lookup"><span data-stu-id="70a10-136">id</span></span>|<span data-ttu-id="70a10-137">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="70a10-137">string</span></span>|<span data-ttu-id="70a10-138">ID do aplicativo Azure AD (ID do cliente).</span><span class="sxs-lookup"><span data-stu-id="70a10-138">Azure AD app ID (client ID).</span></span>|
|<span data-ttu-id="70a10-139">recurso</span><span class="sxs-lookup"><span data-stu-id="70a10-139">resource</span></span>|<span data-ttu-id="70a10-140">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="70a10-140">string</span></span>|<span data-ttu-id="70a10-141">Recurso associado ao aplicativo Azure AD.</span><span class="sxs-lookup"><span data-stu-id="70a10-141">Resource associated with the Azure AD app.</span></span> <span data-ttu-id="70a10-142">Também conhecido como URL de resposta ou redirecionamento no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="70a10-142">Also known as reply or redirect URL in the Azure Portal.</span></span>|

> <span data-ttu-id="70a10-143">**Observação:** Você pode receber um erro se vários aplicativos do Teams no mesmo escopo (equipe, chat ou usuário) estão usando o mesmo aplicativo do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="70a10-143">**Note:** You might get an error if multiple Teams apps in the same scope (team, chat or user) are using the same Azure AD app.</span></span> <span data-ttu-id="70a10-144">Certifique-se de que você esteja usando aplicativos exclusivos do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="70a10-144">Make sure that you're using unique Azure AD apps.</span></span>

#### <a name="activities-section-changes"></a><span data-ttu-id="70a10-145">alterações na seção de atividades</span><span class="sxs-lookup"><span data-stu-id="70a10-145">activities section changes</span></span>

```json
"activities":
{
  "activityTypes": [
    {
      "type": "taskCreated",
      "description": "Task Created Activity",
      "templateText": "{actor} created task {taskId} for you"
    },
    {
      "type": "approvalRequired",
      "description": "Deployment requires your approval",
      "templateText": "{actor} created a new deployment {deploymentId}"
    }
  ]
}
```

|<span data-ttu-id="70a10-146">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="70a10-146">Parameter</span></span>|<span data-ttu-id="70a10-147">Tipo</span><span class="sxs-lookup"><span data-stu-id="70a10-147">Type</span></span>|<span data-ttu-id="70a10-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="70a10-148">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70a10-149">type</span><span class="sxs-lookup"><span data-stu-id="70a10-149">type</span></span>|<span data-ttu-id="70a10-150">string</span><span class="sxs-lookup"><span data-stu-id="70a10-150">string</span></span>|<span data-ttu-id="70a10-151">Tipo de atividade.</span><span class="sxs-lookup"><span data-stu-id="70a10-151">Type of activity.</span></span> <span data-ttu-id="70a10-152">Isso precisa ser exclusivo em um manifesto específico.</span><span class="sxs-lookup"><span data-stu-id="70a10-152">This needs to be unique in a specific manifest.</span></span>|
|<span data-ttu-id="70a10-153">description</span><span class="sxs-lookup"><span data-stu-id="70a10-153">description</span></span>|<span data-ttu-id="70a10-154">string</span><span class="sxs-lookup"><span data-stu-id="70a10-154">string</span></span>|<span data-ttu-id="70a10-155">Descrição curta acessível para humanos.</span><span class="sxs-lookup"><span data-stu-id="70a10-155">Human-readable short description.</span></span> <span data-ttu-id="70a10-156">Isso ficará visível no cliente do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="70a10-156">This will be visible on the Microsoft Teams client.</span></span>|
|<span data-ttu-id="70a10-157">templateText</span><span class="sxs-lookup"><span data-stu-id="70a10-157">templateText</span></span>|<span data-ttu-id="70a10-158">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="70a10-158">string</span></span>|<span data-ttu-id="70a10-159">Texto do modelo para a notificação de atividade.</span><span class="sxs-lookup"><span data-stu-id="70a10-159">Template text for the activity notification.</span></span> <span data-ttu-id="70a10-160">Você pode declarar seus parâmetros encapsulando parâmetros em `{}` .</span><span class="sxs-lookup"><span data-stu-id="70a10-160">You can declare your parameters by encapsulating parameters in `{}`.</span></span>|

><span data-ttu-id="70a10-161">**Observação:** `actor` é um parâmetro especial que sempre leva o nome do chamador.</span><span class="sxs-lookup"><span data-stu-id="70a10-161">**Note:** `actor` is a special parameter that always takes the name of the caller.</span></span> <span data-ttu-id="70a10-162">Em chamadas delegadas, `actor` é o nome do usuário.</span><span class="sxs-lookup"><span data-stu-id="70a10-162">In delegated calls, `actor` is the user's name.</span></span> <span data-ttu-id="70a10-163">Em chamadas somente de aplicativo, ele recebe o nome do aplicativo Teams.</span><span class="sxs-lookup"><span data-stu-id="70a10-163">In application-only calls, it takes the name of the Teams app.</span></span>

### <a name="installing-the-teams-app"></a><span data-ttu-id="70a10-164">Instalando o aplicativo Teams</span><span class="sxs-lookup"><span data-stu-id="70a10-164">Installing the Teams app</span></span>

<span data-ttu-id="70a10-165">Os aplicativos do Teams podem ser instalados em uma equipe, um chat ou para um usuário pessoalmente e podem ser distribuídos de várias maneiras.</span><span class="sxs-lookup"><span data-stu-id="70a10-165">Teams apps can be installed in a team, a chat, or for a user personally, and can be distributed in multiple ways.</span></span> <span data-ttu-id="70a10-166">Para obter detalhes, confira [os métodos de distribuição de aplicativos do Teams.](/microsoftteams/platform/concepts/deploy-and-publish/overview)</span><span class="sxs-lookup"><span data-stu-id="70a10-166">For details, see [Teams app distribution methods](/microsoftteams/platform/concepts/deploy-and-publish/overview).</span></span> <span data-ttu-id="70a10-167">Normalmente, o [sideload é](/microsoftteams/platform/concepts/deploy-and-publish/apps-upload) preferencial para fins de desenvolvimento.</span><span class="sxs-lookup"><span data-stu-id="70a10-167">Typically, [sideloading](/microsoftteams/platform/concepts/deploy-and-publish/apps-upload) is preferred for development purposes.</span></span> <span data-ttu-id="70a10-168">Após o desenvolvimento, você pode escolher o método de distribuição certo com base em se você deseja distribuir para um locatário ou para todos os locatários.</span><span class="sxs-lookup"><span data-stu-id="70a10-168">After development, you can choose the right distribution method based on whether you want to distribute to one tenant or to all tenants.</span></span>

<span data-ttu-id="70a10-169">Você também pode usar APIs [de instalação de aplicativos](/graph/api/resources/teamsappinstallation?preserve-view=true) do Teams para gerenciar instalações de aplicativos do Teams.</span><span class="sxs-lookup"><span data-stu-id="70a10-169">You can also use [Teams app installation](/graph/api/resources/teamsappinstallation?preserve-view=true) APIs to manage Teams app installations.</span></span>

## <a name="sending-activity-feed-notifications-to-users"></a><span data-ttu-id="70a10-170">Enviar notificações de feed de atividades aos usuários</span><span class="sxs-lookup"><span data-stu-id="70a10-170">Sending activity feed notifications to users</span></span>

<span data-ttu-id="70a10-171">Como um aplicativo do Teams pode ser instalado para um usuário, em uma equipe ou em um chat, as notificações também podem ser enviadas nesses três contextos:</span><span class="sxs-lookup"><span data-stu-id="70a10-171">Because a Teams app can be installed for a user, in a team, or in a chat, the notifications can be sent in these three contexts as well:</span></span>

- [<span data-ttu-id="70a10-172">Enviar notificação para o usuário em um chat</span><span class="sxs-lookup"><span data-stu-id="70a10-172">Send notification to user in a chat</span></span>](/graph/api/chat-sendactivitynotification)
- [<span data-ttu-id="70a10-173">Enviar notificação para o usuário em uma equipe</span><span class="sxs-lookup"><span data-stu-id="70a10-173">Send notification to user in a team</span></span>](/graph/api/team-sendactivitynotification)
- [<span data-ttu-id="70a10-174">Enviar notificação para o usuário</span><span class="sxs-lookup"><span data-stu-id="70a10-174">Send notification to user</span></span>](/graph/api/userteamwork-sendactivitynotification)

<span data-ttu-id="70a10-175">Para obter detalhes sobre quais tópicos são suportados para cada cenário, consulte as APIs específicas.</span><span class="sxs-lookup"><span data-stu-id="70a10-175">For details about what topics are supported for each scenario, see the specific APIs.</span></span> <span data-ttu-id="70a10-176">Tópicos personalizados baseados em texto são suportados para todos os cenários.</span><span class="sxs-lookup"><span data-stu-id="70a10-176">Custom text-based topics are supported for all scenarios.</span></span>

### <a name="example-1-notify-a-user-about-a-task-created-in-a-chat"></a><span data-ttu-id="70a10-177">Exemplo 1: Notificar um usuário sobre uma tarefa criada em um chat</span><span class="sxs-lookup"><span data-stu-id="70a10-177">Example 1: Notify a user about a task created in a chat</span></span>

<span data-ttu-id="70a10-178">Este exemplo mostra como você pode enviar uma notificação de feed de atividades para uma nova tarefa criada em um chat.</span><span class="sxs-lookup"><span data-stu-id="70a10-178">This example shows how you can send an activity feed notification for a new task created in a chat.</span></span> <span data-ttu-id="70a10-179">Nesse caso, o aplicativo Teams deve ser instalado em um chat com ID e o usuário também deve fazer parte `chatId` `569363e2-4e49-4661-87f2-16f245c5d66a` do chat.</span><span class="sxs-lookup"><span data-stu-id="70a10-179">In this case, the Teams app must be installed in a chat with Id `chatId` and user `569363e2-4e49-4661-87f2-16f245c5d66a` must be part of the chat as well.</span></span>

#### <a name="request"></a><span data-ttu-id="70a10-180">Solicitação</span><span class="sxs-lookup"><span data-stu-id="70a10-180">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "chat_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/beta/chats/{chatId}/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/beta/chats/{chatId}"
    },
    "activityType": "taskCreated",
    "previewText": {
        "content": "New Task Created"
    },
    "recipient": {
        "@odata.type": "microsoft.graph.aadUserNotificationRecipient",
        "userId": "569363e2-4e49-4661-87f2-16f245c5d66a"
    },
    "templateParameters": [
        {
            "name": "taskId",
            "value": "12322"
        }
    ]
}
```

#### <a name="response"></a><span data-ttu-id="70a10-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="70a10-181">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-notify-a-user-about-a-task-created-in-a-team"></a><span data-ttu-id="70a10-182">Exemplo 2: Notificar um usuário sobre uma tarefa criada em uma equipe</span><span class="sxs-lookup"><span data-stu-id="70a10-182">Example 2: Notify a user about a task created in a team</span></span>

<span data-ttu-id="70a10-183">Este exemplo mostra como você pode enviar uma notificação de feed de atividades para uma equipe.</span><span class="sxs-lookup"><span data-stu-id="70a10-183">This example shows how you can send an activity feed notification for a team.</span></span> <span data-ttu-id="70a10-184">Este exemplo notifica o proprietário da equipe sobre uma nova tarefa criada que requer sua atenção.</span><span class="sxs-lookup"><span data-stu-id="70a10-184">This example notifies the team owner about a new task created that requires their attention.</span></span>

#### <a name="request"></a><span data-ttu-id="70a10-185">Solicitação</span><span class="sxs-lookup"><span data-stu-id="70a10-185">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/beta/teams/{teamId}/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/beta/teams/{teamId}"
    },
    "activityType": "taskCreated",
    "previewText": {
        "content": "New Task Created"
    },
    "recipient": {
        "@odata.type": "microsoft.graph.aadUserNotificationRecipient",
        "userId": "569363e2-4e49-4661-87f2-16f245c5d66a"
    },
    "templateParameters": [
        {
            "name": "taskId",
            "value": "12322"
        }
    ]
}
```

#### <a name="response"></a><span data-ttu-id="70a10-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="70a10-186">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-3-notify-a-user-about-an-event-using-a-custom-topic"></a><span data-ttu-id="70a10-187">Exemplo 3: Notificar um usuário sobre um evento usando um tópico personalizado</span><span class="sxs-lookup"><span data-stu-id="70a10-187">Example 3: Notify a user about an event using a custom topic</span></span>

<span data-ttu-id="70a10-188">Conforme visto nos exemplos anteriores, você pode vincular a diferentes aspectos de uma equipe ou de um chat.</span><span class="sxs-lookup"><span data-stu-id="70a10-188">As seen in the previous examples, you can link to different aspects of a team or a chat.</span></span> <span data-ttu-id="70a10-189">No entanto, se você quiser vincular a um aspecto que não faz parte da equipe ou não é representado pelo Microsoft Graph, ou se quiser personalizar o nome, você pode definir a origem do para e passar um valor personalizado para `topic` `text` ele.</span><span class="sxs-lookup"><span data-stu-id="70a10-189">However, if you want to link to an aspect that is not part of the team or is not represented by Microsoft Graph, or if you want to customize the name, you can set the source of the `topic` to `text` and pass in a custom value for it.</span></span> <span data-ttu-id="70a10-190">Além disso, `webUrl` é necessário quando você usa a fonte como `topic` `text` .</span><span class="sxs-lookup"><span data-stu-id="70a10-190">Additionally, `webUrl` is required when you use `topic` source as `text`.</span></span>

<span data-ttu-id="70a10-191">O exemplo de notificação do Yammer mostrado anteriormente usa um tópico personalizado porque os recursos do Yammer não são suportados pelo Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="70a10-191">The Yammer notification example shown earlier uses a custom topic because Yammer's resources are not supported by Microsoft Graph.</span></span>

> <span data-ttu-id="70a10-192">**Observação:** `webUrl` deve começar com o domínio do Microsoft Teams (teams.microsoft.com por exemplo).</span><span class="sxs-lookup"><span data-stu-id="70a10-192">**Note:** `webUrl` must start with the Microsoft Teams domain (teams.microsoft.com for example).</span></span>

#### <a name="request"></a><span data-ttu-id="70a10-193">Solicitação</span><span class="sxs-lookup"><span data-stu-id="70a10-193">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/beta/teams/{teamId}/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "text",
        "value": "Deployment Approvals Channel",
        "webUrl": "https://teams.microsoft.com/l/message/19:448cfd2ac2a7490a9084a9ed14cttr78c@thread.skype/1605223780000?tenantId=c8b1bf45-3834-4ecf-971a-b4c755ee677d&groupId=d4c2a937-f097-435a-bc91-5c1683ca7245&parentMessageId=1605223771864&teamName=Approvals&channelName=Azure%20DevOps&createdTime=1605223780000"
    },
    "activityType": "approvalRequired",
    "previewText": {
        "content": "New deployment requires your approval"
    },
    "recipient": {
        "@odata.type": "Microsoft.Teams.GraphSvc.aadUserNotificationRecipient",
        "userId": "569363e2-4e49-4661-87f2-16f245c5d66a"
    },
    "templateParameters": [
        {
            "name": "deploymentId",
            "value": "6788662"
        }
    ]
}
```

#### <a name="response"></a><span data-ttu-id="70a10-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="70a10-194">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

## <a name="customizing-how-the-notifications-alert-you"></a><span data-ttu-id="70a10-195">Personalização de como as notificações alertam você</span><span class="sxs-lookup"><span data-stu-id="70a10-195">Customizing how the notifications alert you</span></span>

<span data-ttu-id="70a10-196">Os usuários do Microsoft Teams podem personalizar as notificações que veem no feed, como uma faixa e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="70a10-196">Microsoft Teams users can customize the notifications they see in their feed, as a banner, and so on.</span></span> <span data-ttu-id="70a10-197">As notificações geradas por meio de APIs de feed de atividades também podem ser personalizadas.</span><span class="sxs-lookup"><span data-stu-id="70a10-197">Notifications generated through activity feed APIs can also be customized.</span></span> <span data-ttu-id="70a10-198">Os usuários podem escolher como serão notificados por meio das configurações no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="70a10-198">Users can choose how they are notified via settings in Microsoft Teams.</span></span> <span data-ttu-id="70a10-199">Os aplicativos do Teams aparecerão na lista de escolha do usuário, conforme mostrado na captura de tela a seguir.</span><span class="sxs-lookup"><span data-stu-id="70a10-199">Teams apps will appear in the list for the user to choose from, as shown in the following screenshot.</span></span>

![Captura de tela das configurações de Notificações no Teams, com a opção Personalizada realçada](images/teams-activityfeednotifications/notificationsettings.png)

<span data-ttu-id="70a10-201">Os usuários podem **clicar em Editar** ao lado de um aplicativo e personalizar as notificações, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="70a10-201">Users can click **Edit** next to an app and customize the notifications, as shown in the following example.</span></span> <span data-ttu-id="70a10-202">O `description` campo no manifesto do aplicativo Teams é exibido.</span><span class="sxs-lookup"><span data-stu-id="70a10-202">The `description` field in the Teams app manifest is displayed.</span></span>

![Screenshot showing notifications customized to Banner and feed for a Teams app](images/teams-activityfeednotifications/applevelnotificationsettings.png)

## <a name="faqs"></a><span data-ttu-id="70a10-204">Perguntas Frequentes</span><span class="sxs-lookup"><span data-stu-id="70a10-204">FAQs</span></span>

### <a name="who-needs-to-install-the-teams-app"></a><span data-ttu-id="70a10-205">Quem precisa instalar o aplicativo Teams?</span><span class="sxs-lookup"><span data-stu-id="70a10-205">Who needs to install the Teams app?</span></span>

<span data-ttu-id="70a10-206">O usuário de destino deve ter o aplicativo Teams que está enviando notificações instalado.</span><span class="sxs-lookup"><span data-stu-id="70a10-206">The target user must have the Teams app that is sending notifications installed.</span></span>

### <a name="can-a-user-send-notifications-to-themselves"></a><span data-ttu-id="70a10-207">Um usuário pode enviar notificações para si mesmo?</span><span class="sxs-lookup"><span data-stu-id="70a10-207">Can a user send notifications to themselves?</span></span>

<span data-ttu-id="70a10-208">Não, um usuário não pode enviar notificações para si mesmo.</span><span class="sxs-lookup"><span data-stu-id="70a10-208">No, a user cannot send notifications to themselves.</span></span> <span data-ttu-id="70a10-209">Para este cenário, use permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="70a10-209">For this scenario, use application permissions.</span></span>

### <a name="can-a-teams-app-control-how-the-notifications-are-shown-to-the-user"></a><span data-ttu-id="70a10-210">Um aplicativo do Teams pode controlar como as notificações são mostradas ao usuário?</span><span class="sxs-lookup"><span data-stu-id="70a10-210">Can a Teams app control how the notifications are shown to the user?</span></span>

<span data-ttu-id="70a10-211">Não, somente os usuários podem alterar as configurações de notificação.</span><span class="sxs-lookup"><span data-stu-id="70a10-211">No, only users are allowed to change notification settings.</span></span>

### <a name="i-installed-my-app-why-dont-i-see-notification-settings-under-the-user-account"></a><span data-ttu-id="70a10-212">Instalei meu aplicativo, por que não vejo as configurações de notificação na conta de usuário?</span><span class="sxs-lookup"><span data-stu-id="70a10-212">I installed my app, why don't I see notification settings under the user account?</span></span>

<span data-ttu-id="70a10-213">As configurações aparecerão depois que a primeira notificação for enviada pelo aplicativo Teams.</span><span class="sxs-lookup"><span data-stu-id="70a10-213">The settings will appear after the first notification is sent by the Teams app.</span></span> <span data-ttu-id="70a10-214">Isso reduz o número de configurações que os usuários veem.</span><span class="sxs-lookup"><span data-stu-id="70a10-214">This reduces the number of settings that users see.</span></span>

### <a name="i-started-getting-a-409-conflict-error-how-do-i-resolve-it"></a><span data-ttu-id="70a10-215">Eu começo a receber um erro 409 (conflito), como faço para resolvê-lo?</span><span class="sxs-lookup"><span data-stu-id="70a10-215">I started getting a 409 (conflict) error, how do I resolve it?</span></span>

<span data-ttu-id="70a10-216">`Conflict` ocorrem principalmente quando vários aplicativos do Teams instalados no mesmo escopo (equipe, chat, usuário e assim por diante) têm a mesma appId do Azure AD na seção do `webApplicationInfo` manifesto.</span><span class="sxs-lookup"><span data-stu-id="70a10-216">`Conflict` errors primarily occur when multiple Teams apps installed in the same scope (team, chat, user, and so on) have the same Azure AD appId in the `webApplicationInfo` section of the manifest.</span></span> <span data-ttu-id="70a10-217">Quando isso acontece, você receberá um erro `Found multiple applications with the same Azure AD App ID 'Your AzureAD AppId'.` como.</span><span class="sxs-lookup"><span data-stu-id="70a10-217">When this happens, you will get an error such as `Found multiple applications with the same Azure AD App ID 'Your AzureAD AppId'.`.</span></span> <span data-ttu-id="70a10-218">Certifique-se de usar aplicativos exclusivos do Azure AD para aplicativos exclusivos do Teams.</span><span class="sxs-lookup"><span data-stu-id="70a10-218">Make sure that you use unique Azure AD apps for unique Teams apps.</span></span> <span data-ttu-id="70a10-219">Observe que você pode ter o mesmo aplicativo teams instalado em vários escopos (equipe + usuário, por exemplo).</span><span class="sxs-lookup"><span data-stu-id="70a10-219">Note that you can have the same Teams app installed in multiple scopes (team + user for example).</span></span>


