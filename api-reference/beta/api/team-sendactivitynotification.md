---
title: 'equipe: sendActivityNotification'
description: Enviar uma notificação de feed de atividades no escopo de uma equipe.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6db256a71c17e4c940669aaf96f61f70285c8f3e
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523378"
---
# <a name="team-sendactivitynotification"></a><span data-ttu-id="61cbb-103">equipe: sendActivityNotification</span><span class="sxs-lookup"><span data-stu-id="61cbb-103">team: sendActivityNotification</span></span>
<span data-ttu-id="61cbb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61cbb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="61cbb-105">Enviar uma notificação de feed de atividades no escopo de uma equipe.</span><span class="sxs-lookup"><span data-stu-id="61cbb-105">Send an activity feed notification in the scope of a team.</span></span> <span data-ttu-id="61cbb-106">Para obter mais detalhes sobre o envio de notificações e os requisitos para fazer isso, consulte [enviando notificações de atividade do teams](/graph/teams-send-activityfeednotifications).</span><span class="sxs-lookup"><span data-stu-id="61cbb-106">For more details about sending notifications and the requirements for doing so, see [sending Teams activity notifications](/graph/teams-send-activityfeednotifications).</span></span>

## <a name="permissions"></a><span data-ttu-id="61cbb-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="61cbb-107">Permissions</span></span>
<span data-ttu-id="61cbb-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61cbb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61cbb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="61cbb-110">Permission type</span></span>|<span data-ttu-id="61cbb-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="61cbb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="61cbb-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="61cbb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="61cbb-113">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="61cbb-113">TeamsActivity.Send</span></span>|
|<span data-ttu-id="61cbb-114">Delegada (conta Microsoft pessoal)</span><span class="sxs-lookup"><span data-stu-id="61cbb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="61cbb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61cbb-115">Not Supported.</span></span>|
|<span data-ttu-id="61cbb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="61cbb-116">Application</span></span>|<span data-ttu-id="61cbb-117">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="61cbb-117">TeamsActivity.Send</span></span>|

## <a name="http-request"></a><span data-ttu-id="61cbb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="61cbb-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /teams/{teamId}/sendActivityNotification
```

## <a name="request-headers"></a><span data-ttu-id="61cbb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="61cbb-119">Request headers</span></span>
|<span data-ttu-id="61cbb-120">Nome</span><span class="sxs-lookup"><span data-stu-id="61cbb-120">Name</span></span>|<span data-ttu-id="61cbb-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="61cbb-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="61cbb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="61cbb-122">Authorization</span></span>|<span data-ttu-id="61cbb-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="61cbb-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="61cbb-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="61cbb-125">Content-Type</span></span>|<span data-ttu-id="61cbb-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="61cbb-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="61cbb-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="61cbb-128">Request body</span></span>
<span data-ttu-id="61cbb-129">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="61cbb-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="61cbb-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="61cbb-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="61cbb-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="61cbb-131">Parameter</span></span>|<span data-ttu-id="61cbb-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="61cbb-132">Type</span></span>|<span data-ttu-id="61cbb-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="61cbb-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61cbb-134">topic</span><span class="sxs-lookup"><span data-stu-id="61cbb-134">topic</span></span>|[<span data-ttu-id="61cbb-135">teamworkActivityTopic</span><span class="sxs-lookup"><span data-stu-id="61cbb-135">teamworkActivityTopic</span></span>](../resources/teamworkactivitytopic.md)|<span data-ttu-id="61cbb-136">Tópico da notificação.</span><span class="sxs-lookup"><span data-stu-id="61cbb-136">Topic of the notification.</span></span> <span data-ttu-id="61cbb-137">Especifica o recurso que está sendo falamos.</span><span class="sxs-lookup"><span data-stu-id="61cbb-137">Specifies the resource being talked about.</span></span>|
|<span data-ttu-id="61cbb-138">activityType</span><span class="sxs-lookup"><span data-stu-id="61cbb-138">activityType</span></span>|<span data-ttu-id="61cbb-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="61cbb-139">String</span></span>|<span data-ttu-id="61cbb-140">Tipo de atividade.</span><span class="sxs-lookup"><span data-stu-id="61cbb-140">Activity type.</span></span> <span data-ttu-id="61cbb-141">Isso deve ser declarado no [manifesto do aplicativo Teams](/microsoftteams/platform/overview).</span><span class="sxs-lookup"><span data-stu-id="61cbb-141">This must be declared in the [Teams app manifest](/microsoftteams/platform/overview).</span></span>|
|<span data-ttu-id="61cbb-142">chainid</span><span class="sxs-lookup"><span data-stu-id="61cbb-142">chainId</span></span>|<span data-ttu-id="61cbb-143">Int64</span><span class="sxs-lookup"><span data-stu-id="61cbb-143">Int64</span></span>|<span data-ttu-id="61cbb-144">Opcional.</span><span class="sxs-lookup"><span data-stu-id="61cbb-144">Optional.</span></span> <span data-ttu-id="61cbb-145">Usado para substituir uma notificação anterior.</span><span class="sxs-lookup"><span data-stu-id="61cbb-145">Used to override a previous notification.</span></span> <span data-ttu-id="61cbb-146">Use o mesmo `chainId` nas solicitações subsequentes para substituir a notificação anterior.</span><span class="sxs-lookup"><span data-stu-id="61cbb-146">Use the same `chainId` in subsequent requests to override the previous notification.</span></span>|
|<span data-ttu-id="61cbb-147">previewText</span><span class="sxs-lookup"><span data-stu-id="61cbb-147">previewText</span></span>|[<span data-ttu-id="61cbb-148">itemBody</span><span class="sxs-lookup"><span data-stu-id="61cbb-148">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="61cbb-149">Visualizar o texto da notificação.</span><span class="sxs-lookup"><span data-stu-id="61cbb-149">Preview text for the notification.</span></span> <span data-ttu-id="61cbb-150">O Microsoft Teams só mostrará os primeiros 150 caracteres.</span><span class="sxs-lookup"><span data-stu-id="61cbb-150">Microsoft Teams will only show first 150 characters.</span></span>|
|<span data-ttu-id="61cbb-151">TemplateParameters</span><span class="sxs-lookup"><span data-stu-id="61cbb-151">templateParameters</span></span>|<span data-ttu-id="61cbb-152">Coleção [keyValuePair](../resources/keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="61cbb-152">[keyValuePair](../resources/keyvaluepair.md) collection</span></span>|<span data-ttu-id="61cbb-153">Valores para variáveis de modelo definidas na entrada de feed de atividade correspondente ao `activityType` [manifesto do aplicativo Teams](/microsoftteams/platform/overview).</span><span class="sxs-lookup"><span data-stu-id="61cbb-153">Values for template variables defined in the activity feed entry corresponding to `activityType` in [Teams app manifest](/microsoftteams/platform/overview).</span></span>|
|<span data-ttu-id="61cbb-154">destinatário</span><span class="sxs-lookup"><span data-stu-id="61cbb-154">recipient</span></span>|[<span data-ttu-id="61cbb-155">teamworkNotificationRecipient</span><span class="sxs-lookup"><span data-stu-id="61cbb-155">teamworkNotificationRecipient</span></span>](../resources/teamworknotificationrecipient.md)|<span data-ttu-id="61cbb-156">Destinatário da notificação.</span><span class="sxs-lookup"><span data-stu-id="61cbb-156">Recipient of the notification.</span></span> <span data-ttu-id="61cbb-157">Só há suporte para usuários do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="61cbb-157">Only Azure AD users are supported.</span></span> <span data-ttu-id="61cbb-158">Confira também [aadUserNotificationRecipient](../resources/aadusernotificationrecipient.md).</span><span class="sxs-lookup"><span data-stu-id="61cbb-158">See also [aadUserNotificationRecipient](../resources/aadusernotificationrecipient.md).</span></span> |

<span data-ttu-id="61cbb-159">Os recursos a seguir têm suporte ao definir o `source` valor da propriedade **topic** como `entityUrl` :</span><span class="sxs-lookup"><span data-stu-id="61cbb-159">The following resources are supported when setting the `source` value of the **topic** property to `entityUrl`:</span></span>

- [<span data-ttu-id="61cbb-160">team</span><span class="sxs-lookup"><span data-stu-id="61cbb-160">team</span></span>](../resources/team.md)
- [<span data-ttu-id="61cbb-161">channel</span><span class="sxs-lookup"><span data-stu-id="61cbb-161">channel</span></span>](../resources/channel.md)
- [<span data-ttu-id="61cbb-162">chatMesage</span><span class="sxs-lookup"><span data-stu-id="61cbb-162">chatMesage</span></span>](../resources/chatmessage.md)
- [<span data-ttu-id="61cbb-163">teamsTab</span><span class="sxs-lookup"><span data-stu-id="61cbb-163">teamsTab</span></span>](../resources/teamstab.md)

> <span data-ttu-id="61cbb-164">**Observação:** A URL da entidade deve ser o mesmo recurso ou filho da equipe na URL.</span><span class="sxs-lookup"><span data-stu-id="61cbb-164">**Note:** The entity url must be same or child resource of the team in the url.</span></span> <span data-ttu-id="61cbb-165">Além disso, o [aplicativo Teams](/microsoftteams/platform/overview) deve estar instalado na equipe.</span><span class="sxs-lookup"><span data-stu-id="61cbb-165">Additionally, the [Teams app](/microsoftteams/platform/overview) must be installed in the team.</span></span>

## <a name="response"></a><span data-ttu-id="61cbb-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="61cbb-166">Response</span></span>

<span data-ttu-id="61cbb-167">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="61cbb-167">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="61cbb-168">Exemplos</span><span class="sxs-lookup"><span data-stu-id="61cbb-168">Examples</span></span>

### <a name="example-1-notify-a-user-about-pending-finance-approval-requests"></a><span data-ttu-id="61cbb-169">Exemplo 1: notificar um usuário sobre solicitações de aprovação financeira pendentes</span><span class="sxs-lookup"><span data-stu-id="61cbb-169">Example 1: Notify a user about pending finance approval requests</span></span>

<span data-ttu-id="61cbb-170">Este exemplo mostra como você pode enviar uma notificação de feed de atividades para uma equipe.</span><span class="sxs-lookup"><span data-stu-id="61cbb-170">This example shows how you can send an activity feed notification for a team.</span></span> <span data-ttu-id="61cbb-171">Este exemplo notifica o proprietário da equipe sobre solicitações de aprovação financeira pendentes.</span><span class="sxs-lookup"><span data-stu-id="61cbb-171">This example notifies the team owner about pending finance approval requests.</span></span>

#### <a name="request"></a><span data-ttu-id="61cbb-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="61cbb-172">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="61cbb-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="61cbb-173">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="61cbb-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="61cbb-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/team-sendactivitynotification-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="61cbb-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="61cbb-175">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-notify-a-user-about-a-channel-tab"></a><span data-ttu-id="61cbb-176">Exemplo 2: notificar um usuário sobre uma guia de canal</span><span class="sxs-lookup"><span data-stu-id="61cbb-176">Example 2: Notify a user about a channel tab</span></span>

<span data-ttu-id="61cbb-177">Semelhante ao exemplo anterior, este exemplo usa `entityUrl` o `topic` .</span><span class="sxs-lookup"><span data-stu-id="61cbb-177">Similar to the previous example, this example uses `entityUrl` for the `topic`.</span></span> <span data-ttu-id="61cbb-178">No entanto, este exemplo vincula a uma [guia](../resources/teamstab.md) em um [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="61cbb-178">However, this example links to a [tab](../resources/teamstab.md) in a [channel](../resources/channel.md).</span></span> <span data-ttu-id="61cbb-179">A guia hospeda uma página mostrando o usuário o status de sua reserva de Hotel.</span><span class="sxs-lookup"><span data-stu-id="61cbb-179">The tab hosts a page showing the user the status of their hotel reservation.</span></span> <span data-ttu-id="61cbb-180">Selecionar a notificação levará o usuário à guia, onde eles podem verificar a reserva.</span><span class="sxs-lookup"><span data-stu-id="61cbb-180">Selecting the notification will take the user to the tab, where they can check their reservation.</span></span>

#### <a name="request"></a><span data-ttu-id="61cbb-181">Solicitação</span><span class="sxs-lookup"><span data-stu-id="61cbb-181">Request</span></span>
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

#### <a name="response"></a><span data-ttu-id="61cbb-182">Resposta</span><span class="sxs-lookup"><span data-stu-id="61cbb-182">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-3-notify-a-user-about-an-event-using-custom-topic"></a><span data-ttu-id="61cbb-183">Exemplo 3: notificar um usuário sobre um evento usando o tópico personalizado</span><span class="sxs-lookup"><span data-stu-id="61cbb-183">Example 3: Notify a user about an event using custom topic</span></span>

<span data-ttu-id="61cbb-184">Como visto nos exemplos anteriores, você pode vincular a diferentes aspectos da equipe.</span><span class="sxs-lookup"><span data-stu-id="61cbb-184">As seen in the previous examples, you can link to different aspects of the team.</span></span> <span data-ttu-id="61cbb-185">No entanto, se você deseja vincular a um aspecto que não faz parte da equipe ou não é representado pelo Microsoft Graph ou deseja personalizar o nome, você pode definir a fonte do `topic` para `text` e passar um valor personalizado para ele.</span><span class="sxs-lookup"><span data-stu-id="61cbb-185">However, if you want to link to an aspect that is not part of the team or is not represented by Microsoft Graph, or you want to customize the name, you can set the source of the `topic` to `text` and pass in a custom value for it.</span></span> <span data-ttu-id="61cbb-186">`webUrl` é necessário ao definir `topic` source como `text` .</span><span class="sxs-lookup"><span data-stu-id="61cbb-186">`webUrl` is required when setting `topic` source to `text`.</span></span>

#### <a name="request"></a><span data-ttu-id="61cbb-187">Solicitação</span><span class="sxs-lookup"><span data-stu-id="61cbb-187">Request</span></span>
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

#### <a name="response"></a><span data-ttu-id="61cbb-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="61cbb-188">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```
