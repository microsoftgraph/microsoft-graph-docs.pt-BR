---
title: 'team: sendActivityNotification'
description: Envie uma notificação de feed de atividade no escopo de uma equipe.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 81b081ddf045cc1406903bd7d9b88edffc05480d
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2021
ms.locfileid: "53317114"
---
# <a name="team-sendactivitynotification"></a><span data-ttu-id="7286c-103">team: sendActivityNotification</span><span class="sxs-lookup"><span data-stu-id="7286c-103">team: sendActivityNotification</span></span>
<span data-ttu-id="7286c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7286c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7286c-105">Envie uma notificação de feed de atividade no escopo de uma equipe.</span><span class="sxs-lookup"><span data-stu-id="7286c-105">Send an activity feed notification in the scope of a team.</span></span> <span data-ttu-id="7286c-106">Para obter mais detalhes sobre o envio de notificações e os requisitos para fazer isso, consulte [o Teams de atividades.](/graph/teams-send-activityfeednotifications)</span><span class="sxs-lookup"><span data-stu-id="7286c-106">For more details about sending notifications and the requirements for doing so, see [sending Teams activity notifications](/graph/teams-send-activityfeednotifications).</span></span>

## <a name="permissions"></a><span data-ttu-id="7286c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="7286c-107">Permissions</span></span>
<span data-ttu-id="7286c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7286c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7286c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7286c-110">Permission type</span></span>|<span data-ttu-id="7286c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7286c-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7286c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7286c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7286c-113">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="7286c-113">TeamsActivity.Send</span></span>|
|<span data-ttu-id="7286c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7286c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7286c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7286c-115">Not Supported.</span></span>|
|<span data-ttu-id="7286c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7286c-116">Application</span></span>|<span data-ttu-id="7286c-117">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="7286c-117">TeamsActivity.Send</span></span>|

## <a name="http-request"></a><span data-ttu-id="7286c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7286c-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /teams/{teamId}/sendActivityNotification
```

## <a name="request-headers"></a><span data-ttu-id="7286c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7286c-119">Request headers</span></span>
|<span data-ttu-id="7286c-120">Nome</span><span class="sxs-lookup"><span data-stu-id="7286c-120">Name</span></span>|<span data-ttu-id="7286c-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="7286c-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7286c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7286c-122">Authorization</span></span>|<span data-ttu-id="7286c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7286c-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="7286c-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7286c-125">Content-Type</span></span>|<span data-ttu-id="7286c-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7286c-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7286c-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7286c-128">Request body</span></span>
<span data-ttu-id="7286c-129">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="7286c-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="7286c-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="7286c-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="7286c-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="7286c-131">Parameter</span></span>|<span data-ttu-id="7286c-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="7286c-132">Type</span></span>|<span data-ttu-id="7286c-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="7286c-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7286c-134">topic</span><span class="sxs-lookup"><span data-stu-id="7286c-134">topic</span></span>|[<span data-ttu-id="7286c-135">teamworkActivityTopic</span><span class="sxs-lookup"><span data-stu-id="7286c-135">teamworkActivityTopic</span></span>](../resources/teamworkactivitytopic.md)|<span data-ttu-id="7286c-136">Tópico da notificação.</span><span class="sxs-lookup"><span data-stu-id="7286c-136">Topic of the notification.</span></span> <span data-ttu-id="7286c-137">Especifica o recurso que está sendo falado.</span><span class="sxs-lookup"><span data-stu-id="7286c-137">Specifies the resource being talked about.</span></span>|
|<span data-ttu-id="7286c-138">activityType</span><span class="sxs-lookup"><span data-stu-id="7286c-138">activityType</span></span>|<span data-ttu-id="7286c-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7286c-139">String</span></span>|<span data-ttu-id="7286c-140">Tipo de atividade.</span><span class="sxs-lookup"><span data-stu-id="7286c-140">Activity type.</span></span> <span data-ttu-id="7286c-141">Isso deve ser declarado no manifesto Teams [app](/microsoftteams/platform/overview).</span><span class="sxs-lookup"><span data-stu-id="7286c-141">This must be declared in the [Teams app manifest](/microsoftteams/platform/overview).</span></span>|
|<span data-ttu-id="7286c-142">chainId</span><span class="sxs-lookup"><span data-stu-id="7286c-142">chainId</span></span>|<span data-ttu-id="7286c-143">Int64</span><span class="sxs-lookup"><span data-stu-id="7286c-143">Int64</span></span>|<span data-ttu-id="7286c-144">Opcional.</span><span class="sxs-lookup"><span data-stu-id="7286c-144">Optional.</span></span> <span data-ttu-id="7286c-145">Usado para substituir uma notificação anterior.</span><span class="sxs-lookup"><span data-stu-id="7286c-145">Used to override a previous notification.</span></span> <span data-ttu-id="7286c-146">Use o mesmo `chainId` em solicitações subsequentes para substituir a notificação anterior.</span><span class="sxs-lookup"><span data-stu-id="7286c-146">Use the same `chainId` in subsequent requests to override the previous notification.</span></span>|
|<span data-ttu-id="7286c-147">previewText</span><span class="sxs-lookup"><span data-stu-id="7286c-147">previewText</span></span>|[<span data-ttu-id="7286c-148">itemBody</span><span class="sxs-lookup"><span data-stu-id="7286c-148">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="7286c-149">Visualizar texto para a notificação.</span><span class="sxs-lookup"><span data-stu-id="7286c-149">Preview text for the notification.</span></span> <span data-ttu-id="7286c-150">Microsoft Teams mostrará apenas os primeiros 150 caracteres.</span><span class="sxs-lookup"><span data-stu-id="7286c-150">Microsoft Teams will only show first 150 characters.</span></span>|
|<span data-ttu-id="7286c-151">templateParameters</span><span class="sxs-lookup"><span data-stu-id="7286c-151">templateParameters</span></span>|<span data-ttu-id="7286c-152">Coleção [keyValuePair](../resources/keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="7286c-152">[keyValuePair](../resources/keyvaluepair.md) collection</span></span>|<span data-ttu-id="7286c-153">Valores para variáveis de modelo definidas na entrada de feed de atividade `activityType` correspondentes [Teams manifesto do aplicativo](/microsoftteams/platform/overview).</span><span class="sxs-lookup"><span data-stu-id="7286c-153">Values for template variables defined in the activity feed entry corresponding to `activityType` in [Teams app manifest](/microsoftteams/platform/overview).</span></span>|
|<span data-ttu-id="7286c-154">destinatário</span><span class="sxs-lookup"><span data-stu-id="7286c-154">recipient</span></span>|[<span data-ttu-id="7286c-155">teamworkNotificationRecipient</span><span class="sxs-lookup"><span data-stu-id="7286c-155">teamworkNotificationRecipient</span></span>](../resources/teamworknotificationrecipient.md)|<span data-ttu-id="7286c-156">Destinatário da notificação.</span><span class="sxs-lookup"><span data-stu-id="7286c-156">Recipient of the notification.</span></span> <span data-ttu-id="7286c-157">Consulte também [aadUserNotificationRecipient](../resources/aadusernotificationrecipient.md), [teamMembersNotificationRecipient](../resources/teammembersnotificationrecipient.md)e [channelMembersNotificationRecipient](../resources/channelmembersnotificationrecipient.md).</span><span class="sxs-lookup"><span data-stu-id="7286c-157">See also [aadUserNotificationRecipient](../resources/aadusernotificationrecipient.md), [teamMembersNotificationRecipient](../resources/teammembersnotificationrecipient.md), and [channelMembersNotificationRecipient](../resources/channelmembersnotificationrecipient.md).</span></span> |

<span data-ttu-id="7286c-158">Os seguintes recursos são suportados ao definir o `source` valor da propriedade **topic** como `entityUrl` :</span><span class="sxs-lookup"><span data-stu-id="7286c-158">The following resources are supported when setting the `source` value of the **topic** property to `entityUrl`:</span></span>

- [<span data-ttu-id="7286c-159">team</span><span class="sxs-lookup"><span data-stu-id="7286c-159">team</span></span>](../resources/team.md)
- [<span data-ttu-id="7286c-160">channel</span><span class="sxs-lookup"><span data-stu-id="7286c-160">channel</span></span>](../resources/channel.md)
- [<span data-ttu-id="7286c-161">chatMesage</span><span class="sxs-lookup"><span data-stu-id="7286c-161">chatMesage</span></span>](../resources/chatmessage.md)
- [<span data-ttu-id="7286c-162">teamsTab</span><span class="sxs-lookup"><span data-stu-id="7286c-162">teamsTab</span></span>](../resources/teamstab.md)

> <span data-ttu-id="7286c-163">**Observação:** A URL da entidade deve ser o mesmo ou o recurso filho da equipe na URL.</span><span class="sxs-lookup"><span data-stu-id="7286c-163">**Note:** The entity URL must be same or child resource of the team in the URL.</span></span> <span data-ttu-id="7286c-164">Além disso, o [Teams aplicativo deve](/microsoftteams/platform/overview) ser instalado na equipe.</span><span class="sxs-lookup"><span data-stu-id="7286c-164">Additionally, the [Teams app](/microsoftteams/platform/overview) must be installed in the team.</span></span>

## <a name="response"></a><span data-ttu-id="7286c-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="7286c-165">Response</span></span>

<span data-ttu-id="7286c-166">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7286c-166">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="7286c-167">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7286c-167">Examples</span></span>

### <a name="example-1-notify-a-user-about-pending-finance-approval-requests"></a><span data-ttu-id="7286c-168">Exemplo 1: Notificar um usuário sobre solicitações pendentes de aprovação de finanças</span><span class="sxs-lookup"><span data-stu-id="7286c-168">Example 1: Notify a user about pending finance approval requests</span></span>

<span data-ttu-id="7286c-169">Este exemplo mostra como você pode enviar uma notificação de feed de atividade para uma equipe.</span><span class="sxs-lookup"><span data-stu-id="7286c-169">This example shows how you can send an activity feed notification for a team.</span></span> <span data-ttu-id="7286c-170">Este exemplo notifica o proprietário da equipe sobre solicitações pendentes de aprovação de finanças.</span><span class="sxs-lookup"><span data-stu-id="7286c-170">This example notifies the team owner about pending finance approval requests.</span></span>

#### <a name="request"></a><span data-ttu-id="7286c-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7286c-171">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7286c-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="7286c-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification_1"
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
    "activityType": "pendingFinanceApprovalRequests",
    "previewText": {
        "content": "Internal spending team has a pending finance approval requests"
    },
    "recipient": {
        "@odata.type": "microsoft.graph.aadUserNotificationRecipient",
        "userId": "569363e2-4e49-4661-87f2-16f245c5d66a"
    },
    "templateParameters": [
        {
            "name": "pendingRequestCount",
            "value": "5"
        }
    ] 
}
```
# <a name="javascript"></a>[<span data-ttu-id="7286c-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7286c-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/team-sendactivitynotification-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="7286c-174">C#</span><span class="sxs-lookup"><span data-stu-id="7286c-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/team-sendactivitynotification-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7286c-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7286c-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/team-sendactivitynotification-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7286c-176">Java</span><span class="sxs-lookup"><span data-stu-id="7286c-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/team-sendactivitynotification-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7286c-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="7286c-177">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-notify-a-user-about-a-channel-tab"></a><span data-ttu-id="7286c-178">Exemplo 2: Notificar um usuário sobre uma guia de canal</span><span class="sxs-lookup"><span data-stu-id="7286c-178">Example 2: Notify a user about a channel tab</span></span>

<span data-ttu-id="7286c-179">Semelhante ao exemplo anterior, este exemplo usa `entityUrl` para `topic` o .</span><span class="sxs-lookup"><span data-stu-id="7286c-179">Similar to the previous example, this example uses `entityUrl` for the `topic`.</span></span> <span data-ttu-id="7286c-180">No entanto, este exemplo se vincula a [uma guia](../resources/teamstab.md) em um [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="7286c-180">However, this example links to a [tab](../resources/teamstab.md) in a [channel](../resources/channel.md).</span></span> <span data-ttu-id="7286c-181">A guia hospeda uma página mostrando ao usuário o status de sua reserva de hotel.</span><span class="sxs-lookup"><span data-stu-id="7286c-181">The tab hosts a page showing the user the status of their hotel reservation.</span></span> <span data-ttu-id="7286c-182">Selecionar a notificação levará o usuário para a guia, onde ele pode verificar sua reserva.</span><span class="sxs-lookup"><span data-stu-id="7286c-182">Selecting the notification will take the user to the tab, where they can check their reservation.</span></span>

#### <a name="request"></a><span data-ttu-id="7286c-183">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7286c-183">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7286c-184">HTTP</span><span class="sxs-lookup"><span data-stu-id="7286c-184">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification_2"
}
-->
``` http
POST https://graph.microsoft.com/beta/teams/{teamId}/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/beta/teams/{teamId}/channels/{channelId}/tabs/{tabId}"
    },
    "activityType": "reservationUpdated",
    "previewText": {
        "content": "You have moved up the queue"
    },
    "recipient": {
        "@odata.type": "Microsoft.Teams.GraphSvc.aadUserNotificationRecipient",
        "userId": "569363e2-4e49-4661-87f2-16f245c5d66a"
    },
    "templateParameters": [
        {
            "name": "reservationId",
            "value": "TREEE433"
        },
        {
            "name": "currentSlot",
            "value": "23"
        }
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="7286c-185">C#</span><span class="sxs-lookup"><span data-stu-id="7286c-185">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/team-sendactivitynotification-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7286c-186">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7286c-186">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/team-sendactivitynotification-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7286c-187">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7286c-187">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/team-sendactivitynotification-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7286c-188">Java</span><span class="sxs-lookup"><span data-stu-id="7286c-188">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/team-sendactivitynotification-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7286c-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="7286c-189">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-3-notify-a-user-about-an-event-using-custom-topic"></a><span data-ttu-id="7286c-190">Exemplo 3: Notificar um usuário sobre um evento usando tópico personalizado</span><span class="sxs-lookup"><span data-stu-id="7286c-190">Example 3: Notify a user about an event using custom topic</span></span>

<span data-ttu-id="7286c-191">Como visto nos exemplos anteriores, você pode vincular a diferentes aspectos da equipe.</span><span class="sxs-lookup"><span data-stu-id="7286c-191">As seen in the previous examples, you can link to different aspects of the team.</span></span> <span data-ttu-id="7286c-192">No entanto, se você deseja vincular a um aspecto que não faz parte da equipe ou não é representado pela Microsoft Graph, ou deseja personalizar o nome, você pode definir a origem do para e passar um valor personalizado para `topic` `text` ele.</span><span class="sxs-lookup"><span data-stu-id="7286c-192">However, if you want to link to an aspect that is not part of the team or is not represented by Microsoft Graph, or you want to customize the name, you can set the source of the `topic` to `text` and pass in a custom value for it.</span></span> <span data-ttu-id="7286c-193">`webUrl` é necessário ao definir `topic` a fonte como `text` .</span><span class="sxs-lookup"><span data-stu-id="7286c-193">`webUrl` is required when setting `topic` source to `text`.</span></span>

#### <a name="request"></a><span data-ttu-id="7286c-194">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7286c-194">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7286c-195">HTTP</span><span class="sxs-lookup"><span data-stu-id="7286c-195">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification_3"
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
    "activityType": "deploymentApprovalRequired",
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
# <a name="c"></a>[<span data-ttu-id="7286c-196">C#</span><span class="sxs-lookup"><span data-stu-id="7286c-196">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/team-sendactivitynotification-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7286c-197">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7286c-197">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/team-sendactivitynotification-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7286c-198">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7286c-198">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/team-sendactivitynotification-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7286c-199">Java</span><span class="sxs-lookup"><span data-stu-id="7286c-199">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/team-sendactivitynotification-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7286c-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="7286c-200">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-4-notify-the-team-members-about-pending-finance-approval-requests"></a><span data-ttu-id="7286c-201">Exemplo 4: Notificar os membros da equipe sobre solicitações pendentes de aprovação de finanças</span><span class="sxs-lookup"><span data-stu-id="7286c-201">Example 4: Notify the team members about pending finance approval requests</span></span>

<span data-ttu-id="7286c-202">Este exemplo mostra como você pode enviar uma notificação de feed de atividade para todos os membros da equipe.</span><span class="sxs-lookup"><span data-stu-id="7286c-202">This example shows how you can send an activity feed notification to all team members.</span></span> <span data-ttu-id="7286c-203">Este exemplo é semelhante aos exemplos anteriores.</span><span class="sxs-lookup"><span data-stu-id="7286c-203">This example is similar to previous examples.</span></span> <span data-ttu-id="7286c-204">No entanto, nesse caso, `recipient` o [é um teamMembersNotificationRecipient](../resources/teammembersnotificationrecipient.md).</span><span class="sxs-lookup"><span data-stu-id="7286c-204">However, in this case, the `recipient` is a [teamMembersNotificationRecipient](../resources/teammembersnotificationrecipient.md).</span></span> <span data-ttu-id="7286c-205">Observe que `teamId` o especificado no deve corresponder ao especificado na URL de `recipient` `teamId` solicitação.</span><span class="sxs-lookup"><span data-stu-id="7286c-205">Note that the `teamId` specified in the `recipient` must match the `teamId` specified in the request URL.</span></span>

> <span data-ttu-id="7286c-206">**Observação:** A capacidade de enviar notificações a todos os membros da equipe é limitada a equipes com 10.000 membros ou menos.</span><span class="sxs-lookup"><span data-stu-id="7286c-206">**Note:** The ability to send notifications to all team members is limited to teams with 10,000 members or less.</span></span> <span data-ttu-id="7286c-207">Se a equipe exceder 10.000 membros, nenhum membro da equipe receberá uma notificação.</span><span class="sxs-lookup"><span data-stu-id="7286c-207">If the team exceeds 10,000 members, none of the team members will receive a notification.</span></span>

#### <a name="request"></a><span data-ttu-id="7286c-208">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7286c-208">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7286c-209">HTTP</span><span class="sxs-lookup"><span data-stu-id="7286c-209">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification_4"
}
-->

``` http
POST https://graph.microsoft.com/beta/teams/e8bece96-d393-4b9b-b8da-69cedef1a7e7/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/beta/teams/e8bece96-d393-4b9b-b8da-69cedef1a7e7"
    },
    "activityType": "pendingFinanceApprovalRequests",
    "previewText": {
        "content": "Internal spending team has a pending finance approval requests"
    },
    "recipient": {
        "@odata.type": "microsoft.graph.teamMembersNotificationRecipient",
        "teamId": "e8bece96-d393-4b9b-b8da-69cedef1a7e7"
    },
    "templateParameters": [
        {
            "name": "pendingRequestCount",
            "value": "5"
        }
    ] 
}
```
# <a name="c"></a>[<span data-ttu-id="7286c-210">C#</span><span class="sxs-lookup"><span data-stu-id="7286c-210">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/team-sendactivitynotification-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7286c-211">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7286c-211">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/team-sendactivitynotification-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7286c-212">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7286c-212">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/team-sendactivitynotification-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7286c-213">Java</span><span class="sxs-lookup"><span data-stu-id="7286c-213">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/team-sendactivitynotification-4-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7286c-214">Resposta</span><span class="sxs-lookup"><span data-stu-id="7286c-214">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-5-notify-the-channel-members-about-pending-finance-approval-requests"></a><span data-ttu-id="7286c-215">Exemplo 5: Notificar os membros do canal sobre solicitações pendentes de aprovação de finanças</span><span class="sxs-lookup"><span data-stu-id="7286c-215">Example 5: Notify the channel members about pending finance approval requests</span></span>

<span data-ttu-id="7286c-216">Este exemplo mostra como você pode enviar uma notificação de feed de atividade para todos os membros do canal.</span><span class="sxs-lookup"><span data-stu-id="7286c-216">This example shows how you can send an activity feed notification to all channel members.</span></span> <span data-ttu-id="7286c-217">Este exemplo é semelhante ao exemplo anterior.</span><span class="sxs-lookup"><span data-stu-id="7286c-217">This example is similar to the previous example.</span></span> <span data-ttu-id="7286c-218">No entanto, nesse caso, é `recipient` [um channelMembersNotificationRecipient](../resources/channelmembersnotificationrecipient.md).</span><span class="sxs-lookup"><span data-stu-id="7286c-218">However, in this case, the `recipient` is a [channelMembersNotificationRecipient](../resources/channelmembersnotificationrecipient.md).</span></span> <span data-ttu-id="7286c-219">Observe que `teamId` o especificado no deve corresponder ao especificado na URL de `recipient` `teamId` solicitação.</span><span class="sxs-lookup"><span data-stu-id="7286c-219">Note that the `teamId` specified in the `recipient` must match the `teamId` specified in the request URL.</span></span>

#### <a name="request"></a><span data-ttu-id="7286c-220">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7286c-220">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7286c-221">HTTP</span><span class="sxs-lookup"><span data-stu-id="7286c-221">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification_5"
}
-->

``` http
POST https://graph.microsoft.com/beta/teams/e8bece96-d393-4b9b-b8da-69cedef1a7e7/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/beta/teams/e8bece96-d393-4b9b-b8da-69cedef1a7e7"
    },
    "activityType": "pendingFinanceApprovalRequests",
    "previewText": {
        "content": "Internal spending team has a pending finance approval requests"
    },
    "recipient": {
        "@odata.type": "microsoft.graph.channelMembersNotificationRecipient",
        "teamId": "e8bece96-d393-4b9b-b8da-69cedef1a7e7",
        "channelId": "19:3d61a2309f094f4a9310b20f1db37520@thread.tacv2"
    },
    "templateParameters": [
        {
            "name": "pendingRequestCount",
            "value": "5"
        }
    ] 
}
```
# <a name="c"></a>[<span data-ttu-id="7286c-222">C#</span><span class="sxs-lookup"><span data-stu-id="7286c-222">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/team-sendactivitynotification-5-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7286c-223">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7286c-223">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/team-sendactivitynotification-5-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7286c-224">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7286c-224">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/team-sendactivitynotification-5-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7286c-225">Java</span><span class="sxs-lookup"><span data-stu-id="7286c-225">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/team-sendactivitynotification-5-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7286c-226">Resposta</span><span class="sxs-lookup"><span data-stu-id="7286c-226">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```
