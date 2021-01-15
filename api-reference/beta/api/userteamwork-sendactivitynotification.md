---
title: 'userTeamwork: sendActivityNotification'
description: Envie uma notificação de feed de atividades para um usuário.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3dfc3858e51d227bd270bbe783636a4b23c17362
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873126"
---
# <a name="userteamwork-sendactivitynotification"></a><span data-ttu-id="b27be-103">userTeamwork: sendActivityNotification</span><span class="sxs-lookup"><span data-stu-id="b27be-103">userTeamwork: sendActivityNotification</span></span>
<span data-ttu-id="b27be-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b27be-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b27be-105">Envie uma notificação de feed de atividades para um usuário.</span><span class="sxs-lookup"><span data-stu-id="b27be-105">Send an activity feed notification to a user.</span></span> <span data-ttu-id="b27be-106">Para obter mais detalhes sobre como enviar notificações e os requisitos para fazer isso, confira [o envio de notificações de atividades do Teams.](/graph/teams-send-activityfeednotifications)</span><span class="sxs-lookup"><span data-stu-id="b27be-106">For more details about sending notifications and the requirements for doing so, see [sending Teams activity notifications](/graph/teams-send-activityfeednotifications).</span></span>

## <a name="permissions"></a><span data-ttu-id="b27be-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="b27be-107">Permissions</span></span>
<span data-ttu-id="b27be-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b27be-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b27be-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b27be-110">Permission type</span></span>|<span data-ttu-id="b27be-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b27be-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b27be-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b27be-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b27be-113">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="b27be-113">TeamsActivity.Send</span></span>|
|<span data-ttu-id="b27be-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b27be-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b27be-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b27be-115">Not Supported.</span></span>|
|<span data-ttu-id="b27be-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b27be-116">Application</span></span>|<span data-ttu-id="b27be-117">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="b27be-117">TeamsActivity.Send</span></span>|

## <a name="http-request"></a><span data-ttu-id="b27be-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b27be-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{userId}/teamwork/sendActivityNotification
```

## <a name="request-headers"></a><span data-ttu-id="b27be-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b27be-119">Request headers</span></span>
|<span data-ttu-id="b27be-120">Nome</span><span class="sxs-lookup"><span data-stu-id="b27be-120">Name</span></span>|<span data-ttu-id="b27be-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="b27be-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b27be-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b27be-122">Authorization</span></span>|<span data-ttu-id="b27be-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b27be-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b27be-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b27be-125">Content-Type</span></span>|<span data-ttu-id="b27be-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b27be-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b27be-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b27be-128">Request body</span></span>
<span data-ttu-id="b27be-129">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="b27be-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b27be-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="b27be-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b27be-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b27be-131">Parameter</span></span>|<span data-ttu-id="b27be-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="b27be-132">Type</span></span>|<span data-ttu-id="b27be-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="b27be-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b27be-134">topic</span><span class="sxs-lookup"><span data-stu-id="b27be-134">topic</span></span>|[<span data-ttu-id="b27be-135">teamworkActivityTopic</span><span class="sxs-lookup"><span data-stu-id="b27be-135">teamworkActivityTopic</span></span>](../resources/teamworkactivitytopic.md)|<span data-ttu-id="b27be-136">Tópico da notificação.</span><span class="sxs-lookup"><span data-stu-id="b27be-136">Topic of the notification.</span></span> <span data-ttu-id="b27be-137">Especifica o recurso que está sendo falado.</span><span class="sxs-lookup"><span data-stu-id="b27be-137">Specifies the resource being talked about.</span></span>|
|<span data-ttu-id="b27be-138">activityType</span><span class="sxs-lookup"><span data-stu-id="b27be-138">activityType</span></span>|<span data-ttu-id="b27be-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b27be-139">String</span></span>|<span data-ttu-id="b27be-140">Tipo de atividade.</span><span class="sxs-lookup"><span data-stu-id="b27be-140">Activity type.</span></span> <span data-ttu-id="b27be-141">Isso deve ser declarado no manifesto do [aplicativo Teams.](/microsoftteams/platform/overview)</span><span class="sxs-lookup"><span data-stu-id="b27be-141">This must be declared in the [Teams app manifest](/microsoftteams/platform/overview).</span></span>|
|<span data-ttu-id="b27be-142">chainId</span><span class="sxs-lookup"><span data-stu-id="b27be-142">chainId</span></span>|<span data-ttu-id="b27be-143">Int64</span><span class="sxs-lookup"><span data-stu-id="b27be-143">Int64</span></span>|<span data-ttu-id="b27be-144">Opcional.</span><span class="sxs-lookup"><span data-stu-id="b27be-144">Optional.</span></span> <span data-ttu-id="b27be-145">Usado para substituir uma notificação anterior.</span><span class="sxs-lookup"><span data-stu-id="b27be-145">Used to override a previous notification.</span></span> <span data-ttu-id="b27be-146">Use o mesmo `chainId` em solicitações subsequentes para substituir a notificação anterior.</span><span class="sxs-lookup"><span data-stu-id="b27be-146">Use the same `chainId` in subsequent requests to override the previous notification.</span></span>|
|<span data-ttu-id="b27be-147">previewText</span><span class="sxs-lookup"><span data-stu-id="b27be-147">previewText</span></span>|[<span data-ttu-id="b27be-148">itemBody</span><span class="sxs-lookup"><span data-stu-id="b27be-148">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="b27be-149">Texto de visualização para a notificação.</span><span class="sxs-lookup"><span data-stu-id="b27be-149">Preview text for the notification.</span></span> <span data-ttu-id="b27be-150">O Microsoft Teams mostrará apenas os primeiros 150 caracteres.</span><span class="sxs-lookup"><span data-stu-id="b27be-150">Microsoft Teams will only show first 150 characters.</span></span>|
|<span data-ttu-id="b27be-151">templateParameters</span><span class="sxs-lookup"><span data-stu-id="b27be-151">templateParameters</span></span>|<span data-ttu-id="b27be-152">Coleção [keyValuePair](../resources/keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="b27be-152">[keyValuePair](../resources/keyvaluepair.md) collection</span></span>|<span data-ttu-id="b27be-153">Valores para variáveis de modelo definidos na entrada do feed de atividades correspondente no `activityType` manifesto do aplicativo do [Teams.](/microsoftteams/platform/overview)</span><span class="sxs-lookup"><span data-stu-id="b27be-153">Values for template variables defined in the activity feed entry corresponding to `activityType` in [Teams app manifest](/microsoftteams/platform/overview).</span></span>|

<span data-ttu-id="b27be-154">Os seguintes recursos são suportados ao definir `source` o valor da propriedade **de** tópico `entityUrl` como:</span><span class="sxs-lookup"><span data-stu-id="b27be-154">The following resources are supported when setting the `source` value of the **topic** property to `entityUrl`:</span></span>

- [<span data-ttu-id="b27be-155">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="b27be-155">teamsAppInstallation</span></span>](../resources/teamsappinstallation.md)
- [<span data-ttu-id="b27be-156">teamsCatalogApp</span><span class="sxs-lookup"><span data-stu-id="b27be-156">teamsCatalogApp</span></span>](../resources/teamscatalogapp.md)

## <a name="response"></a><span data-ttu-id="b27be-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="b27be-157">Response</span></span>

<span data-ttu-id="b27be-158">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b27be-158">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="b27be-159">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b27be-159">Examples</span></span>

### <a name="example-1-send-notification-to-a-user-for-a-task-created"></a><span data-ttu-id="b27be-160">Exemplo 1: Enviar notificação a um usuário para uma tarefa criada</span><span class="sxs-lookup"><span data-stu-id="b27be-160">Example 1: Send notification to a user for a task created</span></span>

#### <a name="request"></a><span data-ttu-id="b27be-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b27be-161">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b27be-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="b27be-162">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b27be-163">C#</span><span class="sxs-lookup"><span data-stu-id="b27be-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/userteamwork-sendactivitynotification-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b27be-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b27be-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/userteamwork-sendactivitynotification-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b27be-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b27be-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/userteamwork-sendactivitynotification-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b27be-166">Java</span><span class="sxs-lookup"><span data-stu-id="b27be-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/userteamwork-sendactivitynotification-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b27be-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="b27be-167">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-notify-a-user-about-an-event-using-custom-topic"></a><span data-ttu-id="b27be-168">Exemplo 2: Notificar um usuário sobre um evento usando um tópico personalizado</span><span class="sxs-lookup"><span data-stu-id="b27be-168">Example 2: Notify a user about an event using custom topic</span></span>

<span data-ttu-id="b27be-169">Se você deseja vincular um aspecto que não é representado pelo Microsoft Graph ou deseja personalizar o nome, você pode definir a origem do para e passar um valor personalizado `topic` `text` para ele.</span><span class="sxs-lookup"><span data-stu-id="b27be-169">If you want to link an aspect that is not represented by Microsoft Graph, or you want to customize the name, you can set the source of the `topic` to `text` and pass in a custom value for it.</span></span> <span data-ttu-id="b27be-170">`webUrl` é necessário ao usar a `topic` fonte como `text` .</span><span class="sxs-lookup"><span data-stu-id="b27be-170">`webUrl` is required when using `topic` source as `text`.</span></span>

#### <a name="request"></a><span data-ttu-id="b27be-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b27be-171">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b27be-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="b27be-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification"
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
# <a name="javascript"></a>[<span data-ttu-id="b27be-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b27be-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/team-sendactivitynotification-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="b27be-174">C#</span><span class="sxs-lookup"><span data-stu-id="b27be-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/team-sendactivitynotification-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b27be-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b27be-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/team-sendactivitynotification-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b27be-176">Java</span><span class="sxs-lookup"><span data-stu-id="b27be-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/team-sendactivitynotification-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b27be-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="b27be-177">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```
