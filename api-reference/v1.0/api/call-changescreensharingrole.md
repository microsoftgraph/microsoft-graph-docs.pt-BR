---
title: 'Call: changeScreenSharingRole'
description: Permitir que os aplicativos compartilhem conteúdo de tela com os participantes de uma chamada de grupo.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: b6620eb941ef2b3a18bb15f756263c09388df84d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47966374"
---
# <a name="call-changescreensharingrole"></a><span data-ttu-id="260ed-103">Call: changeScreenSharingRole</span><span class="sxs-lookup"><span data-stu-id="260ed-103">call: changeScreenSharingRole</span></span>

<span data-ttu-id="260ed-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="260ed-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="260ed-105">Permitir que os aplicativos compartilhem conteúdo de tela com os participantes de uma chamada de grupo.</span><span class="sxs-lookup"><span data-stu-id="260ed-105">Allow applications to share screen content with the participants of a group call.</span></span>

> <span data-ttu-id="260ed-106">**Observação:** Isso só é suportado para chamadas de grupo que usam mídia hospedada em aplicativos.</span><span class="sxs-lookup"><span data-stu-id="260ed-106">**Note:** This is only supported for group calls that use App-Hosted Media.</span></span>

## <a name="permissions"></a><span data-ttu-id="260ed-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="260ed-107">Permissions</span></span>
<span data-ttu-id="260ed-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="260ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="260ed-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="260ed-110">Permission type</span></span>                        | <span data-ttu-id="260ed-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="260ed-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="260ed-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="260ed-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="260ed-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="260ed-113">Not Supported</span></span>                               |
| <span data-ttu-id="260ed-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="260ed-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="260ed-115">Não suportado</span><span class="sxs-lookup"><span data-stu-id="260ed-115">Not Supported</span></span>                               |
| <span data-ttu-id="260ed-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="260ed-116">Application</span></span>                            | <span data-ttu-id="260ed-117">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="260ed-117">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="260ed-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="260ed-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/changeScreenSharingRole
```

## <a name="request-headers"></a><span data-ttu-id="260ed-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="260ed-119">Request headers</span></span>
| <span data-ttu-id="260ed-120">Nome</span><span class="sxs-lookup"><span data-stu-id="260ed-120">Name</span></span>          | <span data-ttu-id="260ed-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="260ed-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="260ed-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="260ed-122">Authorization</span></span> | <span data-ttu-id="260ed-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="260ed-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="260ed-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="260ed-125">Content-type</span></span>  | <span data-ttu-id="260ed-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="260ed-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="260ed-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="260ed-128">Request body</span></span>
<span data-ttu-id="260ed-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="260ed-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="260ed-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="260ed-130">Parameter</span></span>      | <span data-ttu-id="260ed-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="260ed-131">Type</span></span>    |<span data-ttu-id="260ed-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="260ed-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="260ed-133">role</span><span class="sxs-lookup"><span data-stu-id="260ed-133">role</span></span>|<span data-ttu-id="260ed-134">String</span><span class="sxs-lookup"><span data-stu-id="260ed-134">String</span></span>|<span data-ttu-id="260ed-135">Os valores possíveis são: ' Visualizador ', ' participante '</span><span class="sxs-lookup"><span data-stu-id="260ed-135">Possible values are: 'viewer', 'sharer'</span></span>|

## <a name="response"></a><span data-ttu-id="260ed-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="260ed-136">Response</span></span>
<span data-ttu-id="260ed-137">Se tiver êxito, este método retornará um `202 Accepted` código de resposta e todos os participantes receberão uma atualização de lista.</span><span class="sxs-lookup"><span data-stu-id="260ed-137">If successful, this method returns a `202 Accepted` response code, and all participants will receive a roster update.</span></span>

## <a name="example"></a><span data-ttu-id="260ed-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="260ed-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="260ed-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="260ed-139">Request</span></span>
<span data-ttu-id="260ed-140">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="260ed-140">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="260ed-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="260ed-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-changeScreenSharingRole"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls/{id}/changeScreenSharingRole
Content-Type: application/json
Content-Length: 24

{
  "role": "viewer"
}
```
# <a name="c"></a>[<span data-ttu-id="260ed-142">C#</span><span class="sxs-lookup"><span data-stu-id="260ed-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-changescreensharingrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="260ed-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="260ed-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-changescreensharingrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="260ed-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="260ed-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-changescreensharingrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="260ed-145">Java</span><span class="sxs-lookup"><span data-stu-id="260ed-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-changescreensharingrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="260ed-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="260ed-146">Response</span></span>
<span data-ttu-id="260ed-147">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="260ed-147">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```
##### <a name="notification---roster-updated-with-participant-sending-screen-sharing-video"></a><span data-ttu-id="260ed-148">Lista de notificação atualizada com o participante enviando vídeo de compartilhamento de tela</span><span class="sxs-lookup"><span data-stu-id="260ed-148">Notification - roster updated with participant sending screen sharing video</span></span>
<span data-ttu-id="260ed-149">Observe a `direction: sendOnly` propriedade no fluxo de mídia.</span><span class="sxs-lookup"><span data-stu-id="260ed-149">Note the `direction: sendOnly` property on the media stream.</span></span>

```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "updated",
      "resourceUrl": "/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/participants",
      "resourceData": [
        {
          "@odata.type": "#microsoft.graph.participant",
          "id": "2765eb15-01f8-47c6-b12b-c32111a4a86f",
          "info": {
            "identity": {
              "user": {
                "displayName": "Bob",
                "id": "5810cede-f3cc-42eb-b2c1-e9bd5d53ec96"
              }
            },
            "region": "westus",
            "languageId": "en-US"
          },
          "mediaStreams": [
            {
              "mediaType": "videoBasedScreenSharing",
              "label": "applicationsharing-video",
              "sourceId": "1",
              "direction": "sendOnly"
            }
          ],
          "isMuted": false,
          "isInLobby": false
        }
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "call: changeScreenSharingRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

