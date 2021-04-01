---
title: 'userTeamwork: sendActivityNotification'
description: Envie uma notificação de feed de atividade para um usuário.
author: eddie-lee-msft
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 62a8e740b529aa094466ce53f1a2f93317171101
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473989"
---
# <a name="userteamwork-sendactivitynotification"></a><span data-ttu-id="c5c72-103">userTeamwork: sendActivityNotification</span><span class="sxs-lookup"><span data-stu-id="c5c72-103">userTeamwork: sendActivityNotification</span></span>
<span data-ttu-id="c5c72-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5c72-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c5c72-105">Envie uma notificação de feed de atividade para um usuário.</span><span class="sxs-lookup"><span data-stu-id="c5c72-105">Send an activity feed notification to a user.</span></span> <span data-ttu-id="c5c72-106">Para obter mais detalhes sobre como enviar notificações e os requisitos para fazer isso, consulte [sending Teams activity notifications](/graph/teams-send-activityfeednotifications).</span><span class="sxs-lookup"><span data-stu-id="c5c72-106">For more details about sending notifications and the requirements for doing so, see [sending Teams activity notifications](/graph/teams-send-activityfeednotifications).</span></span>

## <a name="permissions"></a><span data-ttu-id="c5c72-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="c5c72-107">Permissions</span></span>
<span data-ttu-id="c5c72-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5c72-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5c72-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c5c72-110">Permission type</span></span>|<span data-ttu-id="c5c72-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c5c72-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5c72-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c5c72-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c5c72-113">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="c5c72-113">TeamsActivity.Send</span></span>|
|<span data-ttu-id="c5c72-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c5c72-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5c72-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5c72-115">Not Supported.</span></span>|
|<span data-ttu-id="c5c72-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c5c72-116">Application</span></span>|<span data-ttu-id="c5c72-117">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="c5c72-117">TeamsActivity.Send</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5c72-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c5c72-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{userId}/teamwork/sendActivityNotification
```

## <a name="request-headers"></a><span data-ttu-id="c5c72-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c5c72-119">Request headers</span></span>
|<span data-ttu-id="c5c72-120">Nome</span><span class="sxs-lookup"><span data-stu-id="c5c72-120">Name</span></span>|<span data-ttu-id="c5c72-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5c72-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c5c72-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c5c72-122">Authorization</span></span>|<span data-ttu-id="c5c72-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c5c72-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c5c72-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c5c72-125">Content-Type</span></span>|<span data-ttu-id="c5c72-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c5c72-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5c72-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c5c72-128">Request body</span></span>
<span data-ttu-id="c5c72-129">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="c5c72-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c5c72-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="c5c72-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c5c72-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c5c72-131">Parameter</span></span>|<span data-ttu-id="c5c72-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="c5c72-132">Type</span></span>|<span data-ttu-id="c5c72-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5c72-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5c72-134">topic</span><span class="sxs-lookup"><span data-stu-id="c5c72-134">topic</span></span>|[<span data-ttu-id="c5c72-135">teamworkActivityTopic</span><span class="sxs-lookup"><span data-stu-id="c5c72-135">teamworkActivityTopic</span></span>](../resources/teamworkactivitytopic.md)|<span data-ttu-id="c5c72-136">Tópico da notificação.</span><span class="sxs-lookup"><span data-stu-id="c5c72-136">Topic of the notification.</span></span> <span data-ttu-id="c5c72-137">Especifica o recurso que está sendo falado.</span><span class="sxs-lookup"><span data-stu-id="c5c72-137">Specifies the resource being talked about.</span></span>|
|<span data-ttu-id="c5c72-138">activityType</span><span class="sxs-lookup"><span data-stu-id="c5c72-138">activityType</span></span>|<span data-ttu-id="c5c72-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c5c72-139">String</span></span>|<span data-ttu-id="c5c72-140">Tipo de atividade.</span><span class="sxs-lookup"><span data-stu-id="c5c72-140">Activity type.</span></span> <span data-ttu-id="c5c72-141">Isso deve ser declarado no manifesto do [aplicativo teams.](/microsoftteams/platform/overview)</span><span class="sxs-lookup"><span data-stu-id="c5c72-141">This must be declared in the [Teams app manifest](/microsoftteams/platform/overview).</span></span>|
|<span data-ttu-id="c5c72-142">chainId</span><span class="sxs-lookup"><span data-stu-id="c5c72-142">chainId</span></span>|<span data-ttu-id="c5c72-143">Int64</span><span class="sxs-lookup"><span data-stu-id="c5c72-143">Int64</span></span>|<span data-ttu-id="c5c72-144">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c5c72-144">Optional.</span></span> <span data-ttu-id="c5c72-145">Usado para substituir uma notificação anterior.</span><span class="sxs-lookup"><span data-stu-id="c5c72-145">Used to override a previous notification.</span></span> <span data-ttu-id="c5c72-146">Use o mesmo `chainId` em solicitações subsequentes para substituir a notificação anterior.</span><span class="sxs-lookup"><span data-stu-id="c5c72-146">Use the same `chainId` in subsequent requests to override the previous notification.</span></span>|
|<span data-ttu-id="c5c72-147">previewText</span><span class="sxs-lookup"><span data-stu-id="c5c72-147">previewText</span></span>|[<span data-ttu-id="c5c72-148">itemBody</span><span class="sxs-lookup"><span data-stu-id="c5c72-148">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="c5c72-149">Visualizar texto para a notificação.</span><span class="sxs-lookup"><span data-stu-id="c5c72-149">Preview text for the notification.</span></span> <span data-ttu-id="c5c72-150">O Microsoft Teams mostrará apenas os primeiros 150 caracteres.</span><span class="sxs-lookup"><span data-stu-id="c5c72-150">Microsoft Teams will only show first 150 characters.</span></span>|
|<span data-ttu-id="c5c72-151">templateParameters</span><span class="sxs-lookup"><span data-stu-id="c5c72-151">templateParameters</span></span>|<span data-ttu-id="c5c72-152">Coleção [keyValuePair](../resources/keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="c5c72-152">[keyValuePair](../resources/keyvaluepair.md) collection</span></span>|<span data-ttu-id="c5c72-153">Valores para variáveis de modelo definidas na entrada de feed de atividade correspondente `activityType` ao manifesto do aplicativo do [Teams.](/microsoftteams/platform/overview)</span><span class="sxs-lookup"><span data-stu-id="c5c72-153">Values for template variables defined in the activity feed entry corresponding to `activityType` in [Teams app manifest](/microsoftteams/platform/overview).</span></span>|

<span data-ttu-id="c5c72-154">Os seguintes recursos são suportados ao definir o `source` valor da propriedade **topic** como `entityUrl` :</span><span class="sxs-lookup"><span data-stu-id="c5c72-154">The following resources are supported when setting the `source` value of the **topic** property to `entityUrl`:</span></span>

- [<span data-ttu-id="c5c72-155">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="c5c72-155">teamsAppInstallation</span></span>](../resources/teamsappinstallation.md)
- [<span data-ttu-id="c5c72-156">teamsCatalogApp</span><span class="sxs-lookup"><span data-stu-id="c5c72-156">teamsCatalogApp</span></span>](../resources/teamscatalogapp.md)

## <a name="response"></a><span data-ttu-id="c5c72-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5c72-157">Response</span></span>

<span data-ttu-id="c5c72-158">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c5c72-158">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="c5c72-159">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c5c72-159">Examples</span></span>

### <a name="example-1-send-notification-to-a-user-for-a-task-created"></a><span data-ttu-id="c5c72-160">Exemplo 1: Enviar notificação a um usuário para uma tarefa criada</span><span class="sxs-lookup"><span data-stu-id="c5c72-160">Example 1: Send notification to a user for a task created</span></span>

#### <a name="request"></a><span data-ttu-id="c5c72-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c5c72-161">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "userteamwork_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/users/{userId}/teamwork/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/v1.0/users/{userId}/teamwork/installedApps/{installationId}"
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


#### <a name="response"></a><span data-ttu-id="c5c72-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5c72-162">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-notify-a-user-about-an-event-using-custom-topic"></a><span data-ttu-id="c5c72-163">Exemplo 2: Notificar um usuário sobre um evento usando tópico personalizado</span><span class="sxs-lookup"><span data-stu-id="c5c72-163">Example 2: Notify a user about an event using custom topic</span></span>

<span data-ttu-id="c5c72-164">Se você deseja vincular um aspecto que não é representado pelo Microsoft Graph ou deseja personalizar o nome, você pode definir a origem do para e passar um valor personalizado `topic` `text` para ele.</span><span class="sxs-lookup"><span data-stu-id="c5c72-164">If you want to link an aspect that is not represented by Microsoft Graph, or you want to customize the name, you can set the source of the `topic` to `text` and pass in a custom value for it.</span></span> <span data-ttu-id="c5c72-165">`webUrl` é necessário ao usar a `topic` fonte como `text` .</span><span class="sxs-lookup"><span data-stu-id="c5c72-165">`webUrl` is required when using `topic` source as `text`.</span></span>

#### <a name="request"></a><span data-ttu-id="c5c72-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c5c72-166">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/users/{userId}/teamwork/sendActivityNotification
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


#### <a name="response"></a><span data-ttu-id="c5c72-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5c72-167">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```
