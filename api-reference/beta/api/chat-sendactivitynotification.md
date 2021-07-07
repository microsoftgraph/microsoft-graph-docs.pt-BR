---
title: 'chat: sendActivityNotification'
description: Envie uma notificação de feed de atividade no escopo de um chat.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6335c98549a76fbf0baf13613738251770edeca9
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2021
ms.locfileid: "53316910"
---
# <a name="chat-sendactivitynotification"></a><span data-ttu-id="ed716-103">chat: sendActivityNotification</span><span class="sxs-lookup"><span data-stu-id="ed716-103">chat: sendActivityNotification</span></span>
<span data-ttu-id="ed716-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed716-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed716-105">Envie uma notificação de feed de atividade no escopo de um chat.</span><span class="sxs-lookup"><span data-stu-id="ed716-105">Send an activity feed notification in scope of a chat.</span></span> <span data-ttu-id="ed716-106">Para obter mais detalhes sobre o envio de notificações e os requisitos para fazer isso, consulte [o Teams de atividades.](/graph/teams-send-activityfeednotifications)</span><span class="sxs-lookup"><span data-stu-id="ed716-106">For more details about sending notifications and the requirements for doing so, see [sending Teams activity notifications](/graph/teams-send-activityfeednotifications).</span></span>

## <a name="permissions"></a><span data-ttu-id="ed716-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="ed716-107">Permissions</span></span>
<span data-ttu-id="ed716-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed716-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed716-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ed716-110">Permission type</span></span>|<span data-ttu-id="ed716-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ed716-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed716-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ed716-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ed716-113">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="ed716-113">TeamsActivity.Send</span></span>|
|<span data-ttu-id="ed716-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ed716-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed716-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ed716-115">Not Supported.</span></span>|
|<span data-ttu-id="ed716-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ed716-116">Application</span></span>|<span data-ttu-id="ed716-117">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="ed716-117">TeamsActivity.Send</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed716-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ed716-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /chats/{chatId}/sendActivityNotification
```

## <a name="request-headers"></a><span data-ttu-id="ed716-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ed716-119">Request headers</span></span>
|<span data-ttu-id="ed716-120">Nome</span><span class="sxs-lookup"><span data-stu-id="ed716-120">Name</span></span>|<span data-ttu-id="ed716-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed716-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ed716-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ed716-122">Authorization</span></span>|<span data-ttu-id="ed716-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ed716-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ed716-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ed716-125">Content-Type</span></span>|<span data-ttu-id="ed716-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ed716-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed716-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ed716-128">Request body</span></span>
<span data-ttu-id="ed716-129">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="ed716-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ed716-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="ed716-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ed716-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ed716-131">Parameter</span></span>|<span data-ttu-id="ed716-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="ed716-132">Type</span></span>|<span data-ttu-id="ed716-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed716-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed716-134">topic</span><span class="sxs-lookup"><span data-stu-id="ed716-134">topic</span></span>|[<span data-ttu-id="ed716-135">teamworkActivityTopic</span><span class="sxs-lookup"><span data-stu-id="ed716-135">teamworkActivityTopic</span></span>](../resources/teamworkactivitytopic.md)|<span data-ttu-id="ed716-136">Tópico da notificação.</span><span class="sxs-lookup"><span data-stu-id="ed716-136">Topic of the notification.</span></span> <span data-ttu-id="ed716-137">Especifica o recurso que está sendo falado.</span><span class="sxs-lookup"><span data-stu-id="ed716-137">Specifies the resource being talked about.</span></span>|
|<span data-ttu-id="ed716-138">activityType</span><span class="sxs-lookup"><span data-stu-id="ed716-138">activityType</span></span>|<span data-ttu-id="ed716-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ed716-139">String</span></span>|<span data-ttu-id="ed716-140">Tipo de atividade.</span><span class="sxs-lookup"><span data-stu-id="ed716-140">Activity type.</span></span> <span data-ttu-id="ed716-141">Isso deve ser declarado no manifesto Teams [app](/microsoftteams/platform/overview).</span><span class="sxs-lookup"><span data-stu-id="ed716-141">This must be declared in the [Teams app manifest](/microsoftteams/platform/overview).</span></span>|
|<span data-ttu-id="ed716-142">chainId</span><span class="sxs-lookup"><span data-stu-id="ed716-142">chainId</span></span>|<span data-ttu-id="ed716-143">Int64</span><span class="sxs-lookup"><span data-stu-id="ed716-143">Int64</span></span>|<span data-ttu-id="ed716-144">Opcional.</span><span class="sxs-lookup"><span data-stu-id="ed716-144">Optional.</span></span> <span data-ttu-id="ed716-145">Usado para substituir uma notificação anterior.</span><span class="sxs-lookup"><span data-stu-id="ed716-145">Used to override a previous notification.</span></span> <span data-ttu-id="ed716-146">Use o mesmo `chainId` em solicitações subsequentes para substituir a notificação anterior.</span><span class="sxs-lookup"><span data-stu-id="ed716-146">Use the same `chainId` in subsequent requests to override the previous notification.</span></span>|
|<span data-ttu-id="ed716-147">previewText</span><span class="sxs-lookup"><span data-stu-id="ed716-147">previewText</span></span>|[<span data-ttu-id="ed716-148">itemBody</span><span class="sxs-lookup"><span data-stu-id="ed716-148">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="ed716-149">Visualizar texto para a notificação.</span><span class="sxs-lookup"><span data-stu-id="ed716-149">Preview text for the notification.</span></span> <span data-ttu-id="ed716-150">Microsoft Teams mostrará apenas os primeiros 150 caracteres.</span><span class="sxs-lookup"><span data-stu-id="ed716-150">Microsoft Teams will only show first 150 characters.</span></span>|
|<span data-ttu-id="ed716-151">templateParameters</span><span class="sxs-lookup"><span data-stu-id="ed716-151">templateParameters</span></span>|<span data-ttu-id="ed716-152">Coleção [keyValuePair](../resources/keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="ed716-152">[keyValuePair](../resources/keyvaluepair.md) collection</span></span>|<span data-ttu-id="ed716-153">Valores para variáveis de modelo definidas na entrada de feed de atividade `activityType` correspondentes [Teams manifesto do aplicativo](/microsoftteams/platform/overview).</span><span class="sxs-lookup"><span data-stu-id="ed716-153">Values for template variables defined in the activity feed entry corresponding to `activityType` in [Teams app manifest](/microsoftteams/platform/overview).</span></span>|
|<span data-ttu-id="ed716-154">destinatário</span><span class="sxs-lookup"><span data-stu-id="ed716-154">recipient</span></span>|[<span data-ttu-id="ed716-155">teamworkNotificationRecipient</span><span class="sxs-lookup"><span data-stu-id="ed716-155">teamworkNotificationRecipient</span></span>](../resources/teamworknotificationrecipient.md)|<span data-ttu-id="ed716-156">Destinatário da notificação.</span><span class="sxs-lookup"><span data-stu-id="ed716-156">Recipient of the notification.</span></span> <span data-ttu-id="ed716-157">Consulte também [aadUserNotificationRecipient](../resources/aadusernotificationrecipient.md) e [chatMembersNotificationRecipient](../resources/chatmembersnotificationrecipient.md).</span><span class="sxs-lookup"><span data-stu-id="ed716-157">See also [aadUserNotificationRecipient](../resources/aadusernotificationrecipient.md) and [chatMembersNotificationRecipient](../resources/chatmembersnotificationrecipient.md).</span></span> |

<span data-ttu-id="ed716-158">Os seguintes recursos são suportados ao definir o `source` valor da propriedade **topic** como `entityURL` :</span><span class="sxs-lookup"><span data-stu-id="ed716-158">The following resources are supported when setting the `source` value of the **topic** property to `entityURL`:</span></span>

- [<span data-ttu-id="ed716-159">chat</span><span class="sxs-lookup"><span data-stu-id="ed716-159">chat</span></span>](../resources/chat.md)
- [<span data-ttu-id="ed716-160">chatMessage</span><span class="sxs-lookup"><span data-stu-id="ed716-160">chatMessage</span></span>](../resources/chatmessage.md)

> <span data-ttu-id="ed716-161">**Observação:** A URL da entidade deve ser igual ou um recurso filho do chat na URL.</span><span class="sxs-lookup"><span data-stu-id="ed716-161">**Note:** The entity URL must be the same as or a child resource of the chat in the URL.</span></span> <span data-ttu-id="ed716-162">Além disso, o [Teams aplicativo deve](/microsoftteams/platform/overview) ser instalado no chat.</span><span class="sxs-lookup"><span data-stu-id="ed716-162">Additionally, the [Teams app](/microsoftteams/platform/overview) must be installed in the chat.</span></span>

## <a name="response"></a><span data-ttu-id="ed716-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed716-163">Response</span></span>

<span data-ttu-id="ed716-164">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ed716-164">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="ed716-165">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ed716-165">Examples</span></span>

### <a name="example-1-notify-a-user-about-a-task-created-in-a-chat"></a><span data-ttu-id="ed716-166">Exemplo 1: Notificar um usuário sobre uma tarefa criada em um chat</span><span class="sxs-lookup"><span data-stu-id="ed716-166">Example 1: Notify a user about a task created in a chat</span></span>

<span data-ttu-id="ed716-167">Este exemplo mostra como você pode enviar uma notificação de feed de atividade para uma nova tarefa criada em um chat.</span><span class="sxs-lookup"><span data-stu-id="ed716-167">This example shows how you can send an activity feed notification for a new task created in a chat.</span></span> <span data-ttu-id="ed716-168">Para obter mais detalhes, consulte [sending Teams activity notifications](/graph/teams-send-activityfeednotifications).</span><span class="sxs-lookup"><span data-stu-id="ed716-168">For more details, see [sending Teams activity notifications](/graph/teams-send-activityfeednotifications).</span></span>

#### <a name="request"></a><span data-ttu-id="ed716-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ed716-169">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ed716-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="ed716-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chat_sendactivitynotification_1"
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
            "value": "Task 12322"
        }
    ] 
}
```
# <a name="c"></a>[<span data-ttu-id="ed716-171">C#</span><span class="sxs-lookup"><span data-stu-id="ed716-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chat-sendactivitynotification-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ed716-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ed716-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chat-sendactivitynotification-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ed716-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ed716-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chat-sendactivitynotification-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ed716-174">Java</span><span class="sxs-lookup"><span data-stu-id="ed716-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chat-sendactivitynotification-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ed716-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed716-175">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-notify-a-user-about-an-approval-needed-in-a-chat-message"></a><span data-ttu-id="ed716-176">Exemplo 2: Notificar um usuário sobre uma aprovação necessária em uma mensagem de chat</span><span class="sxs-lookup"><span data-stu-id="ed716-176">Example 2: Notify a user about an approval needed in a chat message</span></span>

<span data-ttu-id="ed716-177">Semelhante ao exemplo anterior, este exemplo usa `entityUrl` para `topic` o .</span><span class="sxs-lookup"><span data-stu-id="ed716-177">Similar to the previous example, this example uses `entityUrl` for the `topic`.</span></span> <span data-ttu-id="ed716-178">No entanto, nesse caso, ele se vincula a uma mensagem no chat.</span><span class="sxs-lookup"><span data-stu-id="ed716-178">However, in this case, it links to a message in the chat.</span></span> <span data-ttu-id="ed716-179">A mensagem pode conter um cartão com o botão de aprovação.</span><span class="sxs-lookup"><span data-stu-id="ed716-179">The message can contains a card with the approval button on it.</span></span>

#### <a name="request"></a><span data-ttu-id="ed716-180">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ed716-180">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ed716-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="ed716-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chat_sendactivitynotification_2"
}
-->
``` http
POST https://graph.microsoft.com/beta/chats/{chatId}/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/beta/chats/{chatId}/messages/{messageId}"
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
# <a name="c"></a>[<span data-ttu-id="ed716-182">C#</span><span class="sxs-lookup"><span data-stu-id="ed716-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chat-sendactivitynotification-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ed716-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ed716-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chat-sendactivitynotification-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ed716-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ed716-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chat-sendactivitynotification-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ed716-185">Java</span><span class="sxs-lookup"><span data-stu-id="ed716-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chat-sendactivitynotification-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ed716-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed716-186">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-3-notify-a-user-about-an-event-in-relation-to-a-chat"></a><span data-ttu-id="ed716-187">Exemplo 3: Notificar um usuário sobre um evento em relação a um chat</span><span class="sxs-lookup"><span data-stu-id="ed716-187">Example 3: Notify a user about an event in relation to a chat</span></span>

<span data-ttu-id="ed716-188">Como mostrado nos exemplos anteriores, você pode vincular a diferentes aspectos do chat.</span><span class="sxs-lookup"><span data-stu-id="ed716-188">As shown in the previous examples, you can link to different aspects of the chat.</span></span> <span data-ttu-id="ed716-189">No entanto, se você deseja vincular a um aspecto que não faz parte do chat ou não é representado pelo Microsoft Graph, você pode definir a origem do para e passar um valor personalizado para `topic` `text` ele.</span><span class="sxs-lookup"><span data-stu-id="ed716-189">However, if you want to link to an aspect that is not part of the chat, or is not represented by Microsoft Graph, you can set the source of the `topic` to `text` and pass in a custom value for it.</span></span> <span data-ttu-id="ed716-190">Além disso, `webUrl` é necessário ao definir a fonte como `topic` `text` .</span><span class="sxs-lookup"><span data-stu-id="ed716-190">Also, `webUrl` is required when setting `topic` source to `text`.</span></span>

#### <a name="request"></a><span data-ttu-id="ed716-191">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ed716-191">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ed716-192">HTTP</span><span class="sxs-lookup"><span data-stu-id="ed716-192">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chat_sendactivitynotification_3"
}
-->
``` http
POST https://graph.microsoft.com/beta/chats/{chatId}/sendActivityNotification
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
# <a name="c"></a>[<span data-ttu-id="ed716-193">C#</span><span class="sxs-lookup"><span data-stu-id="ed716-193">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chat-sendactivitynotification-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ed716-194">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ed716-194">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chat-sendactivitynotification-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ed716-195">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ed716-195">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chat-sendactivitynotification-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ed716-196">Java</span><span class="sxs-lookup"><span data-stu-id="ed716-196">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chat-sendactivitynotification-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ed716-197">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed716-197">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-4-notify-the-chat-members-about-a-task-created-in-a-chat"></a><span data-ttu-id="ed716-198">Exemplo 4: Notificar os membros do chat sobre uma tarefa criada em um chat</span><span class="sxs-lookup"><span data-stu-id="ed716-198">Example 4: Notify the chat members about a task created in a chat</span></span>

<span data-ttu-id="ed716-199">Este exemplo mostra como você pode enviar uma notificação de feed de atividade para todos os membros do chat.</span><span class="sxs-lookup"><span data-stu-id="ed716-199">This example shows how you can send an activity feed notification to all chat members.</span></span> <span data-ttu-id="ed716-200">Este exemplo é semelhante aos exemplos anteriores.</span><span class="sxs-lookup"><span data-stu-id="ed716-200">This example is similar to previous examples.</span></span> <span data-ttu-id="ed716-201">No entanto, nesse caso, o `recipient` [é um chatMembersNotificationRecipient](../resources/chatmembersnotificationrecipient.md).</span><span class="sxs-lookup"><span data-stu-id="ed716-201">However, in this case, the `recipient` is a [chatMembersNotificationRecipient](../resources/chatmembersnotificationrecipient.md).</span></span> <span data-ttu-id="ed716-202">Observe que `chatId` o especificado no deve corresponder ao especificado na URL de `recipient` `chatId` solicitação.</span><span class="sxs-lookup"><span data-stu-id="ed716-202">Note that the `chatId` specified in the `recipient` must match the `chatId` specified in the request URL.</span></span>

#### <a name="request"></a><span data-ttu-id="ed716-203">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ed716-203">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ed716-204">HTTP</span><span class="sxs-lookup"><span data-stu-id="ed716-204">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chat_sendactivitynotification_4"
}
-->

``` http
POST https://graph.microsoft.com/beta/chats/19:1c3af46e9e0f4a5293343c8813c47619@thread.v2/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/beta/chats/19:1c3af46e9e0f4a5293343c8813c47619@thread.v2"
    },
    "activityType": "taskCreated",
    "previewText": {
        "content": "New Task Created"
    },
    "recipient": {
        "@odata.type": "microsoft.graph.chatMembersNotificationRecipient",
        "chatId": "19:1c3af46e9e0f4a5293343c8813c47619@thread.v2"
    },
    "templateParameters": [
        {
            "name": "taskId",
            "value": "Task 12322"
        }
    ] 
}
```
# <a name="c"></a>[<span data-ttu-id="ed716-205">C#</span><span class="sxs-lookup"><span data-stu-id="ed716-205">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chat-sendactivitynotification-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ed716-206">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ed716-206">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chat-sendactivitynotification-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ed716-207">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ed716-207">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chat-sendactivitynotification-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ed716-208">Java</span><span class="sxs-lookup"><span data-stu-id="ed716-208">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chat-sendactivitynotification-4-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ed716-209">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed716-209">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```
