---
title: 'team: sendActivityNotification'
description: Envie uma notificação de feed de atividade no escopo de uma equipe.
author: eddie-lee-msft
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0473e199d7a8cf5bb6dc10a3199240450021c8b6
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473999"
---
# <a name="team-sendactivitynotification"></a><span data-ttu-id="70843-103">team: sendActivityNotification</span><span class="sxs-lookup"><span data-stu-id="70843-103">team: sendActivityNotification</span></span>
<span data-ttu-id="70843-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70843-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="70843-105">Envie uma notificação de feed de atividade no escopo de uma equipe.</span><span class="sxs-lookup"><span data-stu-id="70843-105">Send an activity feed notification in the scope of a team.</span></span> <span data-ttu-id="70843-106">Para obter mais detalhes sobre como enviar notificações e os requisitos para fazer isso, consulte [sending Teams activity notifications](/graph/teams-send-activityfeednotifications).</span><span class="sxs-lookup"><span data-stu-id="70843-106">For more details about sending notifications and the requirements for doing so, see [sending Teams activity notifications](/graph/teams-send-activityfeednotifications).</span></span>

## <a name="permissions"></a><span data-ttu-id="70843-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="70843-107">Permissions</span></span>
<span data-ttu-id="70843-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70843-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70843-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="70843-110">Permission type</span></span>|<span data-ttu-id="70843-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="70843-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70843-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="70843-112">Delegated (work or school account)</span></span>|<span data-ttu-id="70843-113">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="70843-113">TeamsActivity.Send</span></span>|
|<span data-ttu-id="70843-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="70843-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="70843-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="70843-115">Not Supported.</span></span>|
|<span data-ttu-id="70843-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="70843-116">Application</span></span>|<span data-ttu-id="70843-117">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="70843-117">TeamsActivity.Send</span></span>|

## <a name="http-request"></a><span data-ttu-id="70843-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="70843-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /teams/{teamId}/sendActivityNotification
```

## <a name="request-headers"></a><span data-ttu-id="70843-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="70843-119">Request headers</span></span>
|<span data-ttu-id="70843-120">Nome</span><span class="sxs-lookup"><span data-stu-id="70843-120">Name</span></span>|<span data-ttu-id="70843-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="70843-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="70843-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="70843-122">Authorization</span></span>|<span data-ttu-id="70843-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="70843-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="70843-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="70843-125">Content-Type</span></span>|<span data-ttu-id="70843-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="70843-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="70843-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="70843-128">Request body</span></span>
<span data-ttu-id="70843-129">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="70843-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="70843-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="70843-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="70843-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="70843-131">Parameter</span></span>|<span data-ttu-id="70843-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="70843-132">Type</span></span>|<span data-ttu-id="70843-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="70843-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70843-134">topic</span><span class="sxs-lookup"><span data-stu-id="70843-134">topic</span></span>|[<span data-ttu-id="70843-135">teamworkActivityTopic</span><span class="sxs-lookup"><span data-stu-id="70843-135">teamworkActivityTopic</span></span>](../resources/teamworkactivitytopic.md)|<span data-ttu-id="70843-136">Tópico da notificação.</span><span class="sxs-lookup"><span data-stu-id="70843-136">Topic of the notification.</span></span> <span data-ttu-id="70843-137">Especifica o recurso que está sendo falado.</span><span class="sxs-lookup"><span data-stu-id="70843-137">Specifies the resource being talked about.</span></span>|
|<span data-ttu-id="70843-138">activityType</span><span class="sxs-lookup"><span data-stu-id="70843-138">activityType</span></span>|<span data-ttu-id="70843-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="70843-139">String</span></span>|<span data-ttu-id="70843-140">Tipo de atividade.</span><span class="sxs-lookup"><span data-stu-id="70843-140">Activity type.</span></span> <span data-ttu-id="70843-141">Isso deve ser declarado no manifesto do [aplicativo teams.](/microsoftteams/platform/overview)</span><span class="sxs-lookup"><span data-stu-id="70843-141">This must be declared in the [Teams app manifest](/microsoftteams/platform/overview).</span></span>|
|<span data-ttu-id="70843-142">chainId</span><span class="sxs-lookup"><span data-stu-id="70843-142">chainId</span></span>|<span data-ttu-id="70843-143">Int64</span><span class="sxs-lookup"><span data-stu-id="70843-143">Int64</span></span>|<span data-ttu-id="70843-144">Opcional.</span><span class="sxs-lookup"><span data-stu-id="70843-144">Optional.</span></span> <span data-ttu-id="70843-145">Usado para substituir uma notificação anterior.</span><span class="sxs-lookup"><span data-stu-id="70843-145">Used to override a previous notification.</span></span> <span data-ttu-id="70843-146">Use o mesmo `chainId` em solicitações subsequentes para substituir a notificação anterior.</span><span class="sxs-lookup"><span data-stu-id="70843-146">Use the same `chainId` in subsequent requests to override the previous notification.</span></span>|
|<span data-ttu-id="70843-147">previewText</span><span class="sxs-lookup"><span data-stu-id="70843-147">previewText</span></span>|[<span data-ttu-id="70843-148">itemBody</span><span class="sxs-lookup"><span data-stu-id="70843-148">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="70843-149">Visualizar texto para a notificação.</span><span class="sxs-lookup"><span data-stu-id="70843-149">Preview text for the notification.</span></span> <span data-ttu-id="70843-150">O Microsoft Teams mostrará apenas os primeiros 150 caracteres.</span><span class="sxs-lookup"><span data-stu-id="70843-150">Microsoft Teams will only show first 150 characters.</span></span>|
|<span data-ttu-id="70843-151">templateParameters</span><span class="sxs-lookup"><span data-stu-id="70843-151">templateParameters</span></span>|<span data-ttu-id="70843-152">Coleção [keyValuePair](../resources/keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="70843-152">[keyValuePair](../resources/keyvaluepair.md) collection</span></span>|<span data-ttu-id="70843-153">Valores para variáveis de modelo definidas na entrada de feed de atividade correspondente `activityType` ao manifesto do aplicativo do [Teams.](/microsoftteams/platform/overview)</span><span class="sxs-lookup"><span data-stu-id="70843-153">Values for template variables defined in the activity feed entry corresponding to `activityType` in [Teams app manifest](/microsoftteams/platform/overview).</span></span>|
|<span data-ttu-id="70843-154">destinatário</span><span class="sxs-lookup"><span data-stu-id="70843-154">recipient</span></span>|[<span data-ttu-id="70843-155">teamworkNotificationRecipient</span><span class="sxs-lookup"><span data-stu-id="70843-155">teamworkNotificationRecipient</span></span>](../resources/teamworknotificationrecipient.md)|<span data-ttu-id="70843-156">Destinatário da notificação.</span><span class="sxs-lookup"><span data-stu-id="70843-156">Recipient of the notification.</span></span> <span data-ttu-id="70843-157">Somente usuários do Azure AD são suportados.</span><span class="sxs-lookup"><span data-stu-id="70843-157">Only Azure AD users are supported.</span></span> <span data-ttu-id="70843-158">Consulte também [aadUserNotificationRecipient](../resources/aadusernotificationrecipient.md).</span><span class="sxs-lookup"><span data-stu-id="70843-158">See also [aadUserNotificationRecipient](../resources/aadusernotificationrecipient.md).</span></span> |

<span data-ttu-id="70843-159">Os seguintes recursos são suportados ao definir o `source` valor da propriedade **topic** como `entityUrl` :</span><span class="sxs-lookup"><span data-stu-id="70843-159">The following resources are supported when setting the `source` value of the **topic** property to `entityUrl`:</span></span>

- [<span data-ttu-id="70843-160">equipe</span><span class="sxs-lookup"><span data-stu-id="70843-160">team</span></span>](../resources/team.md)
- [<span data-ttu-id="70843-161">channel</span><span class="sxs-lookup"><span data-stu-id="70843-161">channel</span></span>](../resources/channel.md)
- [<span data-ttu-id="70843-162">chatMesage</span><span class="sxs-lookup"><span data-stu-id="70843-162">chatMesage</span></span>](../resources/chatmessage.md)
- [<span data-ttu-id="70843-163">teamsTab</span><span class="sxs-lookup"><span data-stu-id="70843-163">teamsTab</span></span>](../resources/teamstab.md)

> <span data-ttu-id="70843-164">**Observação:** A URL da entidade deve ser o mesmo ou o recurso filho da equipe na URL.</span><span class="sxs-lookup"><span data-stu-id="70843-164">**Note:** The entity URL must be same or child resource of the team in the URL.</span></span> <span data-ttu-id="70843-165">Além disso, o [aplicativo do Teams](/microsoftteams/platform/overview) deve ser instalado na equipe.</span><span class="sxs-lookup"><span data-stu-id="70843-165">Additionally, the [Teams app](/microsoftteams/platform/overview) must be installed in the team.</span></span>

## <a name="response"></a><span data-ttu-id="70843-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="70843-166">Response</span></span>

<span data-ttu-id="70843-167">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="70843-167">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="70843-168">Exemplos</span><span class="sxs-lookup"><span data-stu-id="70843-168">Examples</span></span>

### <a name="example-1-notify-a-user-about-pending-finance-approval-requests"></a><span data-ttu-id="70843-169">Exemplo 1: Notificar um usuário sobre solicitações pendentes de aprovação de finanças</span><span class="sxs-lookup"><span data-stu-id="70843-169">Example 1: Notify a user about pending finance approval requests</span></span>

<span data-ttu-id="70843-170">Este exemplo mostra como você pode enviar uma notificação de feed de atividade para uma equipe.</span><span class="sxs-lookup"><span data-stu-id="70843-170">This example shows how you can send an activity feed notification for a team.</span></span> <span data-ttu-id="70843-171">Este exemplo notifica o proprietário da equipe sobre solicitações pendentes de aprovação de finanças.</span><span class="sxs-lookup"><span data-stu-id="70843-171">This example notifies the team owner about pending finance approval requests.</span></span>

#### <a name="request"></a><span data-ttu-id="70843-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="70843-172">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/v1.0/teams/{teamId}"
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


---


#### <a name="response"></a><span data-ttu-id="70843-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="70843-173">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-notify-a-user-about-a-channel-tab"></a><span data-ttu-id="70843-174">Exemplo 2: Notificar um usuário sobre uma guia de canal</span><span class="sxs-lookup"><span data-stu-id="70843-174">Example 2: Notify a user about a channel tab</span></span>

<span data-ttu-id="70843-175">Semelhante ao exemplo anterior, este exemplo usa `entityUrl` para `topic` o .</span><span class="sxs-lookup"><span data-stu-id="70843-175">Similar to the previous example, this example uses `entityUrl` for the `topic`.</span></span> <span data-ttu-id="70843-176">No entanto, este exemplo se vincula a [uma guia](../resources/teamstab.md) em um [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="70843-176">However, this example links to a [tab](../resources/teamstab.md) in a [channel](../resources/channel.md).</span></span> <span data-ttu-id="70843-177">A guia hospeda uma página mostrando ao usuário o status de sua reserva de hotel.</span><span class="sxs-lookup"><span data-stu-id="70843-177">The tab hosts a page showing the user the status of their hotel reservation.</span></span> <span data-ttu-id="70843-178">Selecionar a notificação levará o usuário para a guia, onde ele pode verificar sua reserva.</span><span class="sxs-lookup"><span data-stu-id="70843-178">Selecting the notification will take the user to the tab, where they can check their reservation.</span></span>

#### <a name="request"></a><span data-ttu-id="70843-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="70843-179">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/v1.0/teams/{teamId}/channels/{channelId}/tabs/{tabId}"
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

#### <a name="response"></a><span data-ttu-id="70843-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="70843-180">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-3-notify-a-user-about-an-event-using-custom-topic"></a><span data-ttu-id="70843-181">Exemplo 3: Notificar um usuário sobre um evento usando tópico personalizado</span><span class="sxs-lookup"><span data-stu-id="70843-181">Example 3: Notify a user about an event using custom topic</span></span>

<span data-ttu-id="70843-182">Como visto nos exemplos anteriores, você pode vincular a diferentes aspectos da equipe.</span><span class="sxs-lookup"><span data-stu-id="70843-182">As seen in the previous examples, you can link to different aspects of the team.</span></span> <span data-ttu-id="70843-183">No entanto, se você deseja vincular a um aspecto que não faz parte da equipe ou não é representado pelo Microsoft Graph, ou deseja personalizar o nome, você pode definir a origem do para e passar um valor personalizado para `topic` `text` ele.</span><span class="sxs-lookup"><span data-stu-id="70843-183">However, if you want to link to an aspect that is not part of the team or is not represented by Microsoft Graph, or you want to customize the name, you can set the source of the `topic` to `text` and pass in a custom value for it.</span></span> <span data-ttu-id="70843-184">`webUrl` é necessário ao definir `topic` a fonte como `text` .</span><span class="sxs-lookup"><span data-stu-id="70843-184">`webUrl` is required when setting `topic` source to `text`.</span></span>

#### <a name="request"></a><span data-ttu-id="70843-185">Solicitação</span><span class="sxs-lookup"><span data-stu-id="70843-185">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/sendActivityNotification
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

#### <a name="response"></a><span data-ttu-id="70843-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="70843-186">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```
