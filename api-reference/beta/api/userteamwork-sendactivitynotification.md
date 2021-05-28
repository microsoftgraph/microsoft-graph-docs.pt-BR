---
title: 'userTeamwork: sendActivityNotification'
description: Envie uma notificação de feed de atividade para um usuário.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 938bc52076218c2f31b06f24a5bcdbc9ea2091f2
ms.sourcegitcommit: a9a035e7cf7b500aebe5477c05361552e7c3a7ab
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/28/2021
ms.locfileid: "52696286"
---
# <a name="userteamwork-sendactivitynotification"></a><span data-ttu-id="41be9-103">userTeamwork: sendActivityNotification</span><span class="sxs-lookup"><span data-stu-id="41be9-103">userTeamwork: sendActivityNotification</span></span>
<span data-ttu-id="41be9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41be9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41be9-105">Envie uma notificação de feed de atividade para um usuário.</span><span class="sxs-lookup"><span data-stu-id="41be9-105">Send an activity feed notification to a user.</span></span> <span data-ttu-id="41be9-106">Para obter mais detalhes sobre o envio de notificações e os requisitos para fazer isso, consulte [o Teams de atividades.](/graph/teams-send-activityfeednotifications)</span><span class="sxs-lookup"><span data-stu-id="41be9-106">For more details about sending notifications and the requirements for doing so, see [sending Teams activity notifications](/graph/teams-send-activityfeednotifications).</span></span>

## <a name="permissions"></a><span data-ttu-id="41be9-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="41be9-107">Permissions</span></span>
<span data-ttu-id="41be9-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41be9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41be9-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="41be9-110">Permission type</span></span>|<span data-ttu-id="41be9-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="41be9-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41be9-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="41be9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="41be9-113">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="41be9-113">TeamsActivity.Send</span></span>|
|<span data-ttu-id="41be9-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="41be9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41be9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41be9-115">Not Supported.</span></span>|
|<span data-ttu-id="41be9-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="41be9-116">Application</span></span>|<span data-ttu-id="41be9-117">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="41be9-117">TeamsActivity.Send</span></span>|

## <a name="http-request"></a><span data-ttu-id="41be9-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="41be9-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{userId | user-principal-name}/teamwork/sendActivityNotification
```

## <a name="request-headers"></a><span data-ttu-id="41be9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="41be9-119">Request headers</span></span>
|<span data-ttu-id="41be9-120">Nome</span><span class="sxs-lookup"><span data-stu-id="41be9-120">Name</span></span>|<span data-ttu-id="41be9-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="41be9-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="41be9-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="41be9-122">Authorization</span></span>|<span data-ttu-id="41be9-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41be9-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="41be9-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="41be9-125">Content-Type</span></span>|<span data-ttu-id="41be9-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41be9-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="41be9-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="41be9-128">Request body</span></span>
<span data-ttu-id="41be9-129">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="41be9-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="41be9-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="41be9-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="41be9-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="41be9-131">Parameter</span></span>|<span data-ttu-id="41be9-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="41be9-132">Type</span></span>|<span data-ttu-id="41be9-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="41be9-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41be9-134">topic</span><span class="sxs-lookup"><span data-stu-id="41be9-134">topic</span></span>|[<span data-ttu-id="41be9-135">teamworkActivityTopic</span><span class="sxs-lookup"><span data-stu-id="41be9-135">teamworkActivityTopic</span></span>](../resources/teamworkactivitytopic.md)|<span data-ttu-id="41be9-136">Tópico da notificação.</span><span class="sxs-lookup"><span data-stu-id="41be9-136">Topic of the notification.</span></span> <span data-ttu-id="41be9-137">Especifica o recurso que está sendo falado.</span><span class="sxs-lookup"><span data-stu-id="41be9-137">Specifies the resource being talked about.</span></span>|
|<span data-ttu-id="41be9-138">activityType</span><span class="sxs-lookup"><span data-stu-id="41be9-138">activityType</span></span>|<span data-ttu-id="41be9-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="41be9-139">String</span></span>|<span data-ttu-id="41be9-140">Tipo de atividade.</span><span class="sxs-lookup"><span data-stu-id="41be9-140">Activity type.</span></span> <span data-ttu-id="41be9-141">Isso deve ser declarado no manifesto Teams [app](/microsoftteams/platform/overview).</span><span class="sxs-lookup"><span data-stu-id="41be9-141">This must be declared in the [Teams app manifest](/microsoftteams/platform/overview).</span></span>|
|<span data-ttu-id="41be9-142">chainId</span><span class="sxs-lookup"><span data-stu-id="41be9-142">chainId</span></span>|<span data-ttu-id="41be9-143">Int64</span><span class="sxs-lookup"><span data-stu-id="41be9-143">Int64</span></span>|<span data-ttu-id="41be9-144">Opcional.</span><span class="sxs-lookup"><span data-stu-id="41be9-144">Optional.</span></span> <span data-ttu-id="41be9-145">Usado para substituir uma notificação anterior.</span><span class="sxs-lookup"><span data-stu-id="41be9-145">Used to override a previous notification.</span></span> <span data-ttu-id="41be9-146">Use o mesmo `chainId` em solicitações subsequentes para substituir a notificação anterior.</span><span class="sxs-lookup"><span data-stu-id="41be9-146">Use the same `chainId` in subsequent requests to override the previous notification.</span></span>|
|<span data-ttu-id="41be9-147">previewText</span><span class="sxs-lookup"><span data-stu-id="41be9-147">previewText</span></span>|[<span data-ttu-id="41be9-148">itemBody</span><span class="sxs-lookup"><span data-stu-id="41be9-148">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="41be9-149">Visualizar texto para a notificação.</span><span class="sxs-lookup"><span data-stu-id="41be9-149">Preview text for the notification.</span></span> <span data-ttu-id="41be9-150">Microsoft Teams mostrará apenas os primeiros 150 caracteres.</span><span class="sxs-lookup"><span data-stu-id="41be9-150">Microsoft Teams will only show first 150 characters.</span></span>|
|<span data-ttu-id="41be9-151">templateParameters</span><span class="sxs-lookup"><span data-stu-id="41be9-151">templateParameters</span></span>|<span data-ttu-id="41be9-152">Coleção [keyValuePair](../resources/keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="41be9-152">[keyValuePair](../resources/keyvaluepair.md) collection</span></span>|<span data-ttu-id="41be9-153">Valores para variáveis de modelo definidas na entrada de feed de atividade `activityType` correspondentes [Teams manifesto do aplicativo](/microsoftteams/platform/overview).</span><span class="sxs-lookup"><span data-stu-id="41be9-153">Values for template variables defined in the activity feed entry corresponding to `activityType` in [Teams app manifest](/microsoftteams/platform/overview).</span></span>|

<span data-ttu-id="41be9-154">Os seguintes recursos são suportados ao definir o `source` valor da propriedade **topic** como `entityUrl` :</span><span class="sxs-lookup"><span data-stu-id="41be9-154">The following resources are supported when setting the `source` value of the **topic** property to `entityUrl`:</span></span>

- [<span data-ttu-id="41be9-155">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="41be9-155">teamsAppInstallation</span></span>](../resources/teamsappinstallation.md)
- [<span data-ttu-id="41be9-156">teamsCatalogApp</span><span class="sxs-lookup"><span data-stu-id="41be9-156">teamsCatalogApp</span></span>](../resources/teamscatalogapp.md)

## <a name="response"></a><span data-ttu-id="41be9-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="41be9-157">Response</span></span>

<span data-ttu-id="41be9-158">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="41be9-158">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="41be9-159">Exemplos</span><span class="sxs-lookup"><span data-stu-id="41be9-159">Examples</span></span>

### <a name="example-1-send-notification-to-a-user-for-a-task-created"></a><span data-ttu-id="41be9-160">Exemplo 1: Enviar notificação a um usuário para uma tarefa criada</span><span class="sxs-lookup"><span data-stu-id="41be9-160">Example 1: Send notification to a user for a task created</span></span>

#### <a name="request"></a><span data-ttu-id="41be9-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="41be9-161">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="41be9-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="41be9-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "userteamwork_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/beta/users/{userId}/teamwork/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/beta/users/{userId}/teamwork/installedApps/{installationId}"
    },
    "activityType": "taskCreated",
    "previewText": {
        "content": "New Task Created"
    },
    "templateParameters": [
        {
            "name": "taskId",
            "value": "Task 12322"
        }
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="41be9-163">C#</span><span class="sxs-lookup"><span data-stu-id="41be9-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/userteamwork-sendactivitynotification-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="41be9-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="41be9-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/userteamwork-sendactivitynotification-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="41be9-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="41be9-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/userteamwork-sendactivitynotification-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="41be9-166">Java</span><span class="sxs-lookup"><span data-stu-id="41be9-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/userteamwork-sendactivitynotification-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="41be9-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="41be9-167">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-notify-a-user-about-an-event-using-custom-topic"></a><span data-ttu-id="41be9-168">Exemplo 2: Notificar um usuário sobre um evento usando tópico personalizado</span><span class="sxs-lookup"><span data-stu-id="41be9-168">Example 2: Notify a user about an event using custom topic</span></span>

<span data-ttu-id="41be9-169">Se você quiser vincular um aspecto que não é representado pela Microsoft Graph, ou quiser personalizar o nome, você pode definir a origem do para e passar um valor personalizado para `topic` `text` ele.</span><span class="sxs-lookup"><span data-stu-id="41be9-169">If you want to link an aspect that is not represented by Microsoft Graph, or you want to customize the name, you can set the source of the `topic` to `text` and pass in a custom value for it.</span></span> <span data-ttu-id="41be9-170">`webUrl` é necessário ao usar a `topic` fonte como `text` .</span><span class="sxs-lookup"><span data-stu-id="41be9-170">`webUrl` is required when using `topic` source as `text`.</span></span>

#### <a name="request"></a><span data-ttu-id="41be9-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="41be9-171">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="41be9-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="41be9-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification_4"
}
-->
``` http
POST https://graph.microsoft.com/beta/users/{userId}/teamwork/sendActivityNotification
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
    "templateParameters": [
        {
            "name": "deploymentId",
            "value": "6788662"
        }
    ]
}
```
# <a name="javascript"></a>[<span data-ttu-id="41be9-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="41be9-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/team-sendactivitynotification-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="41be9-174">C#</span><span class="sxs-lookup"><span data-stu-id="41be9-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/team-sendactivitynotification-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="41be9-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="41be9-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/team-sendactivitynotification-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="41be9-176">Java</span><span class="sxs-lookup"><span data-stu-id="41be9-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/team-sendactivitynotification-4-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="41be9-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="41be9-177">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```
