---
title: 'chat: sendActivityNotification'
description: Envie uma notificação de feed de atividade no escopo de um chat.
author: eddie-lee-msft
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: eabe78843dd9b1e2e71fd433a61e04154e9aafcc
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51474118"
---
# <a name="chat-sendactivitynotification"></a><span data-ttu-id="02fa8-103">chat: sendActivityNotification</span><span class="sxs-lookup"><span data-stu-id="02fa8-103">chat: sendActivityNotification</span></span>
<span data-ttu-id="02fa8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02fa8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="02fa8-105">Envie uma notificação de feed de atividade no escopo de um chat.</span><span class="sxs-lookup"><span data-stu-id="02fa8-105">Send an activity feed notification in scope of a chat.</span></span> <span data-ttu-id="02fa8-106">Para obter mais detalhes sobre como enviar notificações e os requisitos para fazer isso, consulte [sending Teams activity notifications](/graph/teams-send-activityfeednotifications).</span><span class="sxs-lookup"><span data-stu-id="02fa8-106">For more details about sending notifications and the requirements for doing so, see [sending Teams activity notifications](/graph/teams-send-activityfeednotifications).</span></span>

## <a name="permissions"></a><span data-ttu-id="02fa8-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="02fa8-107">Permissions</span></span>
<span data-ttu-id="02fa8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02fa8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02fa8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02fa8-110">Permission type</span></span>|<span data-ttu-id="02fa8-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="02fa8-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02fa8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02fa8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="02fa8-113">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="02fa8-113">TeamsActivity.Send</span></span>|
|<span data-ttu-id="02fa8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02fa8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02fa8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02fa8-115">Not Supported.</span></span>|
|<span data-ttu-id="02fa8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="02fa8-116">Application</span></span>|<span data-ttu-id="02fa8-117">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="02fa8-117">TeamsActivity.Send</span></span>|

## <a name="http-request"></a><span data-ttu-id="02fa8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02fa8-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /chats/{chatId}/sendActivityNotification
```

## <a name="request-headers"></a><span data-ttu-id="02fa8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="02fa8-119">Request headers</span></span>
|<span data-ttu-id="02fa8-120">Nome</span><span class="sxs-lookup"><span data-stu-id="02fa8-120">Name</span></span>|<span data-ttu-id="02fa8-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="02fa8-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="02fa8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="02fa8-122">Authorization</span></span>|<span data-ttu-id="02fa8-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02fa8-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="02fa8-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="02fa8-125">Content-Type</span></span>|<span data-ttu-id="02fa8-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02fa8-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="02fa8-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02fa8-128">Request body</span></span>
<span data-ttu-id="02fa8-129">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="02fa8-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="02fa8-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="02fa8-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="02fa8-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="02fa8-131">Parameter</span></span>|<span data-ttu-id="02fa8-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="02fa8-132">Type</span></span>|<span data-ttu-id="02fa8-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="02fa8-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02fa8-134">topic</span><span class="sxs-lookup"><span data-stu-id="02fa8-134">topic</span></span>|[<span data-ttu-id="02fa8-135">teamworkActivityTopic</span><span class="sxs-lookup"><span data-stu-id="02fa8-135">teamworkActivityTopic</span></span>](../resources/teamworkactivitytopic.md)|<span data-ttu-id="02fa8-136">Tópico da notificação.</span><span class="sxs-lookup"><span data-stu-id="02fa8-136">Topic of the notification.</span></span> <span data-ttu-id="02fa8-137">Especifica o recurso que está sendo falado.</span><span class="sxs-lookup"><span data-stu-id="02fa8-137">Specifies the resource being talked about.</span></span>|
|<span data-ttu-id="02fa8-138">activityType</span><span class="sxs-lookup"><span data-stu-id="02fa8-138">activityType</span></span>|<span data-ttu-id="02fa8-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02fa8-139">String</span></span>|<span data-ttu-id="02fa8-140">Tipo de atividade.</span><span class="sxs-lookup"><span data-stu-id="02fa8-140">Activity type.</span></span> <span data-ttu-id="02fa8-141">Isso deve ser declarado no manifesto do [aplicativo teams.](/microsoftteams/platform/overview)</span><span class="sxs-lookup"><span data-stu-id="02fa8-141">This must be declared in the [Teams app manifest](/microsoftteams/platform/overview).</span></span>|
|<span data-ttu-id="02fa8-142">chainId</span><span class="sxs-lookup"><span data-stu-id="02fa8-142">chainId</span></span>|<span data-ttu-id="02fa8-143">Int64</span><span class="sxs-lookup"><span data-stu-id="02fa8-143">Int64</span></span>|<span data-ttu-id="02fa8-144">Opcional.</span><span class="sxs-lookup"><span data-stu-id="02fa8-144">Optional.</span></span> <span data-ttu-id="02fa8-145">Usado para substituir uma notificação anterior.</span><span class="sxs-lookup"><span data-stu-id="02fa8-145">Used to override a previous notification.</span></span> <span data-ttu-id="02fa8-146">Use o mesmo `chainId` em solicitações subsequentes para substituir a notificação anterior.</span><span class="sxs-lookup"><span data-stu-id="02fa8-146">Use the same `chainId` in subsequent requests to override the previous notification.</span></span>|
|<span data-ttu-id="02fa8-147">previewText</span><span class="sxs-lookup"><span data-stu-id="02fa8-147">previewText</span></span>|[<span data-ttu-id="02fa8-148">itemBody</span><span class="sxs-lookup"><span data-stu-id="02fa8-148">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="02fa8-149">Visualizar texto para a notificação.</span><span class="sxs-lookup"><span data-stu-id="02fa8-149">Preview text for the notification.</span></span> <span data-ttu-id="02fa8-150">O Microsoft Teams mostrará apenas os primeiros 150 caracteres.</span><span class="sxs-lookup"><span data-stu-id="02fa8-150">Microsoft Teams will only show first 150 characters.</span></span>|
|<span data-ttu-id="02fa8-151">templateParameters</span><span class="sxs-lookup"><span data-stu-id="02fa8-151">templateParameters</span></span>|<span data-ttu-id="02fa8-152">Coleção [keyValuePair](../resources/keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="02fa8-152">[keyValuePair](../resources/keyvaluepair.md) collection</span></span>|<span data-ttu-id="02fa8-153">Valores para variáveis de modelo definidas na entrada de feed de atividade correspondente `activityType` ao manifesto do aplicativo do [Teams.](/microsoftteams/platform/overview)</span><span class="sxs-lookup"><span data-stu-id="02fa8-153">Values for template variables defined in the activity feed entry corresponding to `activityType` in [Teams app manifest](/microsoftteams/platform/overview).</span></span>|
|<span data-ttu-id="02fa8-154">destinatário</span><span class="sxs-lookup"><span data-stu-id="02fa8-154">recipient</span></span>|[<span data-ttu-id="02fa8-155">teamworkNotificationRecipient</span><span class="sxs-lookup"><span data-stu-id="02fa8-155">teamworkNotificationRecipient</span></span>](../resources/teamworknotificationrecipient.md)|<span data-ttu-id="02fa8-156">Destinatário da notificação.</span><span class="sxs-lookup"><span data-stu-id="02fa8-156">Recipient of the notification.</span></span> <span data-ttu-id="02fa8-157">Somente usuários do Azure AD são suportados.</span><span class="sxs-lookup"><span data-stu-id="02fa8-157">Only Azure AD users are supported.</span></span> <span data-ttu-id="02fa8-158">Consulte também [aadUserNotificationRecipient](../resources/aadusernotificationrecipient.md).</span><span class="sxs-lookup"><span data-stu-id="02fa8-158">See also [aadUserNotificationRecipient](../resources/aadusernotificationrecipient.md).</span></span> |

<span data-ttu-id="02fa8-159">Os seguintes recursos são suportados ao definir o `source` valor da propriedade **topic** como `entityURL` :</span><span class="sxs-lookup"><span data-stu-id="02fa8-159">The following resources are supported when setting the `source` value of the **topic** property to `entityURL`:</span></span>

- [<span data-ttu-id="02fa8-160">chat</span><span class="sxs-lookup"><span data-stu-id="02fa8-160">chat</span></span>](../resources/chat.md)
- [<span data-ttu-id="02fa8-161">chatMessage</span><span class="sxs-lookup"><span data-stu-id="02fa8-161">chatMessage</span></span>](../resources/chatmessage.md)

> <span data-ttu-id="02fa8-162">**Observação:** A URL da entidade deve ser igual ou um recurso filho do chat na URL.</span><span class="sxs-lookup"><span data-stu-id="02fa8-162">**Note:** The entity URL must be the same as or a child resource of the chat in the URL.</span></span> <span data-ttu-id="02fa8-163">Além disso, o [aplicativo do Teams](/microsoftteams/platform/overview) deve ser instalado no chat.</span><span class="sxs-lookup"><span data-stu-id="02fa8-163">Additionally, the [Teams app](/microsoftteams/platform/overview) must be installed in the chat.</span></span>

## <a name="response"></a><span data-ttu-id="02fa8-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="02fa8-164">Response</span></span>

<span data-ttu-id="02fa8-165">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="02fa8-165">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="02fa8-166">Exemplos</span><span class="sxs-lookup"><span data-stu-id="02fa8-166">Examples</span></span>

### <a name="example-1-notify-a-user-about-a-task-created-in-a-chat"></a><span data-ttu-id="02fa8-167">Exemplo 1: Notificar um usuário sobre uma tarefa criada em um chat</span><span class="sxs-lookup"><span data-stu-id="02fa8-167">Example 1: Notify a user about a task created in a chat</span></span>

<span data-ttu-id="02fa8-168">Este exemplo mostra como você pode enviar uma notificação de feed de atividade para uma nova tarefa criada em um chat.</span><span class="sxs-lookup"><span data-stu-id="02fa8-168">This example shows how you can send an activity feed notification for a new task created in a chat.</span></span> <span data-ttu-id="02fa8-169">Para obter mais detalhes, consulte [sending Teams activity notifications](/graph/teams-send-activityfeednotifications).</span><span class="sxs-lookup"><span data-stu-id="02fa8-169">For more details, see [sending Teams activity notifications](/graph/teams-send-activityfeednotifications).</span></span>

#### <a name="request"></a><span data-ttu-id="02fa8-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02fa8-170">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "chat_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/chats/{chatId}/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/v1.0/chats/{chatId}"
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
            "value": "Task 12322"
        }
    ] 
}
```

#### <a name="response"></a><span data-ttu-id="02fa8-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="02fa8-171">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-notify-a-user-about-a-approval-needed-in-a-chat-message"></a><span data-ttu-id="02fa8-172">Exemplo 2: Notificar um usuário sobre uma aprovação necessária em uma mensagem de chat</span><span class="sxs-lookup"><span data-stu-id="02fa8-172">Example 2: Notify a user about a approval needed in a chat message</span></span>

<span data-ttu-id="02fa8-173">Semelhante ao exemplo anterior, este exemplo usa `entityUrl` para `topic` o .</span><span class="sxs-lookup"><span data-stu-id="02fa8-173">Similar to the previous example, this example uses `entityUrl` for the `topic`.</span></span> <span data-ttu-id="02fa8-174">No entanto, nesse caso, ele se vincula a uma mensagem no chat.</span><span class="sxs-lookup"><span data-stu-id="02fa8-174">However, in this case, it links to a message in the chat.</span></span> <span data-ttu-id="02fa8-175">A mensagem pode conter um cartão com o botão de aprovação.</span><span class="sxs-lookup"><span data-stu-id="02fa8-175">The message can contains a card with the approval button on it.</span></span>

#### <a name="request"></a><span data-ttu-id="02fa8-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02fa8-176">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "chat_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/chats/{chatId}/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/v1.0/chats/{chatId}/messages/{messageId}"
    },
    "activityType": "approvalRequired",
    "previewText": {
        "content": "Deployment requires your approval"
    },
    "recipient": {
        "@odata.type": "Microsoft.Teams.GraphSvc.aadUserNotificationRecipient",
        "userId": "569363e2-4e49-4661-87f2-16f245c5d66a"
    },
    "templateParameters": [
        {
            "name": "approvalTaskId",
            "value": "2020AAGGTAPP"
        }
    ]
}
```

#### <a name="response"></a><span data-ttu-id="02fa8-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="02fa8-177">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-3-notify-a-user-about-an-event-in-relation-to-a-chat"></a><span data-ttu-id="02fa8-178">Exemplo 3: Notificar um usuário sobre um evento em relação a um chat</span><span class="sxs-lookup"><span data-stu-id="02fa8-178">Example 3: Notify a user about an event in relation to a chat</span></span>

<span data-ttu-id="02fa8-179">Como mostrado nos exemplos anteriores, você pode vincular a diferentes aspectos do chat.</span><span class="sxs-lookup"><span data-stu-id="02fa8-179">As shown in the previous examples, you can link to different aspects of the chat.</span></span> <span data-ttu-id="02fa8-180">No entanto, se você deseja vincular a um aspecto que não faz parte do chat ou não é representado pelo Microsoft Graph, você pode definir a origem do para e passar um valor personalizado para `topic` `text` ele.</span><span class="sxs-lookup"><span data-stu-id="02fa8-180">However, if you want to link to an aspect that is not part of the chat, or is not represented by Microsoft Graph, you can set the source of the `topic` to `text` and pass in a custom value for it.</span></span> <span data-ttu-id="02fa8-181">Além disso, `webUrl` é necessário ao definir a fonte como `topic` `text` .</span><span class="sxs-lookup"><span data-stu-id="02fa8-181">Also, `webUrl` is required when setting `topic` source to `text`.</span></span>

#### <a name="request"></a><span data-ttu-id="02fa8-182">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02fa8-182">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "chat_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/chats/{chatId}/sendActivityNotification
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

#### <a name="response"></a><span data-ttu-id="02fa8-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="02fa8-183">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```
