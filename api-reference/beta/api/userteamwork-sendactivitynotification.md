---
title: 'Conjunto de equipe: sendActivityNotification'
description: Enviar uma notificação de feed de atividades para um usuário.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 09e9382663140abbd736a7497ce632bacf83b24b
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377487"
---
# <a name="userteamwork-sendactivitynotification"></a><span data-ttu-id="b28fa-103">Conjunto de equipe: sendActivityNotification</span><span class="sxs-lookup"><span data-stu-id="b28fa-103">userTeamwork: sendActivityNotification</span></span>
<span data-ttu-id="b28fa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b28fa-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b28fa-105">Enviar uma notificação de feed de atividades para um usuário.</span><span class="sxs-lookup"><span data-stu-id="b28fa-105">Send an activity feed notification to a user.</span></span> <span data-ttu-id="b28fa-106">Para obter mais detalhes sobre o envio de notificações e os requisitos para fazer isso, consulte [enviando notificações de atividade do teams](/graph/teams-send-activityfeednotifications).</span><span class="sxs-lookup"><span data-stu-id="b28fa-106">For more details about sending notifications and the requirements for doing so, see [sending Teams activity notifications](/graph/teams-send-activityfeednotifications).</span></span>

## <a name="permissions"></a><span data-ttu-id="b28fa-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="b28fa-107">Permissions</span></span>
<span data-ttu-id="b28fa-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b28fa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b28fa-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b28fa-110">Permission type</span></span>|<span data-ttu-id="b28fa-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b28fa-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b28fa-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b28fa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b28fa-113">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="b28fa-113">TeamsActivity.Send</span></span>|
|<span data-ttu-id="b28fa-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b28fa-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b28fa-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b28fa-115">Not Supported.</span></span>|
|<span data-ttu-id="b28fa-116">Application</span><span class="sxs-lookup"><span data-stu-id="b28fa-116">Application</span></span>|<span data-ttu-id="b28fa-117">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="b28fa-117">TeamsActivity.Send</span></span>|

## <a name="http-request"></a><span data-ttu-id="b28fa-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b28fa-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{userId}/teamwork/sendActivityNotification
```

## <a name="request-headers"></a><span data-ttu-id="b28fa-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b28fa-119">Request headers</span></span>
|<span data-ttu-id="b28fa-120">Nome</span><span class="sxs-lookup"><span data-stu-id="b28fa-120">Name</span></span>|<span data-ttu-id="b28fa-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="b28fa-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b28fa-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b28fa-122">Authorization</span></span>|<span data-ttu-id="b28fa-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b28fa-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b28fa-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b28fa-125">Content-Type</span></span>|<span data-ttu-id="b28fa-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b28fa-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b28fa-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b28fa-128">Request body</span></span>
<span data-ttu-id="b28fa-129">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="b28fa-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b28fa-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="b28fa-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b28fa-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b28fa-131">Parameter</span></span>|<span data-ttu-id="b28fa-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="b28fa-132">Type</span></span>|<span data-ttu-id="b28fa-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="b28fa-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b28fa-134">topic</span><span class="sxs-lookup"><span data-stu-id="b28fa-134">topic</span></span>|[<span data-ttu-id="b28fa-135">teamworkActivityTopic</span><span class="sxs-lookup"><span data-stu-id="b28fa-135">teamworkActivityTopic</span></span>](../resources/teamworkactivitytopic.md)|<span data-ttu-id="b28fa-136">Tópico da notificação.</span><span class="sxs-lookup"><span data-stu-id="b28fa-136">Topic of the notification.</span></span> <span data-ttu-id="b28fa-137">Especifica o recurso que está sendo falamos.</span><span class="sxs-lookup"><span data-stu-id="b28fa-137">Specifies the resource being talked about.</span></span>|
|<span data-ttu-id="b28fa-138">activityType</span><span class="sxs-lookup"><span data-stu-id="b28fa-138">activityType</span></span>|<span data-ttu-id="b28fa-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b28fa-139">String</span></span>|<span data-ttu-id="b28fa-140">Tipo de atividade.</span><span class="sxs-lookup"><span data-stu-id="b28fa-140">Activity type.</span></span> <span data-ttu-id="b28fa-141">Isso deve ser declarado no [manifesto do aplicativo Teams](/microsoftteams/platform/overview).</span><span class="sxs-lookup"><span data-stu-id="b28fa-141">This must be declared in the [Teams app manifest](/microsoftteams/platform/overview).</span></span>|
|<span data-ttu-id="b28fa-142">chainid</span><span class="sxs-lookup"><span data-stu-id="b28fa-142">chainId</span></span>|<span data-ttu-id="b28fa-143">Int64</span><span class="sxs-lookup"><span data-stu-id="b28fa-143">Int64</span></span>|<span data-ttu-id="b28fa-144">Opcional.</span><span class="sxs-lookup"><span data-stu-id="b28fa-144">Optional.</span></span> <span data-ttu-id="b28fa-145">Usado para substituir uma notificação anterior.</span><span class="sxs-lookup"><span data-stu-id="b28fa-145">Used to override a previous notification.</span></span> <span data-ttu-id="b28fa-146">Use o mesmo `chainId` nas solicitações subsequentes para substituir a notificação anterior.</span><span class="sxs-lookup"><span data-stu-id="b28fa-146">Use the same `chainId` in subsequent requests to override the previous notification.</span></span>|
|<span data-ttu-id="b28fa-147">previewText</span><span class="sxs-lookup"><span data-stu-id="b28fa-147">previewText</span></span>|[<span data-ttu-id="b28fa-148">itemBody</span><span class="sxs-lookup"><span data-stu-id="b28fa-148">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="b28fa-149">Visualizar o texto da notificação.</span><span class="sxs-lookup"><span data-stu-id="b28fa-149">Preview text for the notification.</span></span> <span data-ttu-id="b28fa-150">O Microsoft Teams só mostrará os primeiros 150 caracteres.</span><span class="sxs-lookup"><span data-stu-id="b28fa-150">Microsoft Teams will only show first 150 characters.</span></span>|
|<span data-ttu-id="b28fa-151">TemplateParameters</span><span class="sxs-lookup"><span data-stu-id="b28fa-151">templateParameters</span></span>|<span data-ttu-id="b28fa-152">Coleção [keyValuePair](../resources/keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="b28fa-152">[keyValuePair](../resources/keyvaluepair.md) collection</span></span>|<span data-ttu-id="b28fa-153">Valores para variáveis de modelo definidas na entrada de feed de atividade correspondente ao `activityType` [manifesto do aplicativo Teams](/microsoftteams/platform/overview).</span><span class="sxs-lookup"><span data-stu-id="b28fa-153">Values for template variables defined in the activity feed entry corresponding to `activityType` in [Teams app manifest](/microsoftteams/platform/overview).</span></span>|

<span data-ttu-id="b28fa-154">Os recursos a seguir têm suporte ao definir o `source` valor da propriedade **topic** como `entityUrl` :</span><span class="sxs-lookup"><span data-stu-id="b28fa-154">The following resources are supported when setting the `source` value of the **topic** property to `entityUrl`:</span></span>

- [<span data-ttu-id="b28fa-155">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="b28fa-155">teamsAppInstallation</span></span>](../resources/teamsappinstallation.md)
- [<span data-ttu-id="b28fa-156">teamsCatalogApp</span><span class="sxs-lookup"><span data-stu-id="b28fa-156">teamsCatalogApp</span></span>](../resources/teamscatalogapp.md)

## <a name="response"></a><span data-ttu-id="b28fa-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="b28fa-157">Response</span></span>

<span data-ttu-id="b28fa-158">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b28fa-158">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="b28fa-159">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b28fa-159">Examples</span></span>

### <a name="example-1-send-notification-to-a-user-for-a-task-created"></a><span data-ttu-id="b28fa-160">Exemplo 1: enviar notificação para um usuário para uma tarefa criada</span><span class="sxs-lookup"><span data-stu-id="b28fa-160">Example 1: Send notification to a user for a task created</span></span>

#### <a name="request"></a><span data-ttu-id="b28fa-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b28fa-161">Request</span></span>
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

#### <a name="response"></a><span data-ttu-id="b28fa-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="b28fa-162">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-notify-a-user-about-an-event-using-custom-topic"></a><span data-ttu-id="b28fa-163">Exemplo 2: notificar um usuário sobre um evento usando o tópico personalizado</span><span class="sxs-lookup"><span data-stu-id="b28fa-163">Example 2: Notify a user about an event using custom topic</span></span>

<span data-ttu-id="b28fa-164">Se você deseja vincular um aspecto que não é representado pelo Microsoft Graph ou deseja personalizar o nome, você pode definir a fonte do `topic` para `text` e passar um valor personalizado para ele.</span><span class="sxs-lookup"><span data-stu-id="b28fa-164">If you want to link an aspect that is not represented by Microsoft Graph, or you want to customize the name, you can set the source of the `topic` to `text` and pass in a custom value for it.</span></span> <span data-ttu-id="b28fa-165">`webUrl` é necessário ao usar `topic` source como `text` .</span><span class="sxs-lookup"><span data-stu-id="b28fa-165">`webUrl` is required when using `topic` source as `text`.</span></span>

#### <a name="request"></a><span data-ttu-id="b28fa-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b28fa-166">Request</span></span>
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

#### <a name="response"></a><span data-ttu-id="b28fa-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="b28fa-167">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```
