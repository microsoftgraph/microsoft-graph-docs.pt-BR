---
title: 'call: changeScreenSharingRole'
description: Permitir que os aplicativos compartilhem conteúdo de tela com os participantes de uma chamada de grupo.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 5239d0c2929f43d457253268d190c1ae68e87870
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786570"
---
# <a name="call-changescreensharingrole"></a><span data-ttu-id="f4db2-103">call: changeScreenSharingRole</span><span class="sxs-lookup"><span data-stu-id="f4db2-103">call: changeScreenSharingRole</span></span>

<span data-ttu-id="f4db2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4db2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4db2-105">Permitir que os aplicativos compartilhem conteúdo de tela com os participantes de uma chamada de grupo.</span><span class="sxs-lookup"><span data-stu-id="f4db2-105">Allow applications to share screen content with the participants of a group call.</span></span>

> <span data-ttu-id="f4db2-106">**Observação:** Isso só é suportado para chamadas de grupo que usam App-Hosted Mídia.</span><span class="sxs-lookup"><span data-stu-id="f4db2-106">**Note:** This is only supported for group calls that use App-Hosted Media.</span></span>

## <a name="permissions"></a><span data-ttu-id="f4db2-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="f4db2-107">Permissions</span></span>
<span data-ttu-id="f4db2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4db2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f4db2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f4db2-110">Permission type</span></span>                        | <span data-ttu-id="f4db2-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f4db2-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f4db2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f4db2-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="f4db2-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="f4db2-113">Not Supported</span></span>                               |
| <span data-ttu-id="f4db2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f4db2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4db2-115">Não suportado</span><span class="sxs-lookup"><span data-stu-id="f4db2-115">Not Supported</span></span>                               |
| <span data-ttu-id="f4db2-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f4db2-116">Application</span></span>                            | <span data-ttu-id="f4db2-117">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="f4db2-117">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="f4db2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f4db2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/changeScreenSharingRole
POST /communications/calls/{id}/changeScreenSharingRole
```
> <span data-ttu-id="f4db2-119">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="f4db2-119">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="f4db2-120">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="f4db2-120">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f4db2-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f4db2-121">Request headers</span></span>
| <span data-ttu-id="f4db2-122">Nome</span><span class="sxs-lookup"><span data-stu-id="f4db2-122">Name</span></span>          | <span data-ttu-id="f4db2-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4db2-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="f4db2-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f4db2-124">Authorization</span></span> | <span data-ttu-id="f4db2-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f4db2-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f4db2-127">Content-type</span><span class="sxs-lookup"><span data-stu-id="f4db2-127">Content-type</span></span>  | <span data-ttu-id="f4db2-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f4db2-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4db2-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f4db2-130">Request body</span></span>
<span data-ttu-id="f4db2-131">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f4db2-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f4db2-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f4db2-132">Parameter</span></span>      | <span data-ttu-id="f4db2-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4db2-133">Type</span></span>    |<span data-ttu-id="f4db2-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4db2-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f4db2-135">role</span><span class="sxs-lookup"><span data-stu-id="f4db2-135">role</span></span>|<span data-ttu-id="f4db2-136">String</span><span class="sxs-lookup"><span data-stu-id="f4db2-136">String</span></span>|<span data-ttu-id="f4db2-137">Os valores possíveis são: 'visualizador', 'sharer'</span><span class="sxs-lookup"><span data-stu-id="f4db2-137">Possible values are: 'viewer', 'sharer'</span></span>|

## <a name="response"></a><span data-ttu-id="f4db2-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4db2-138">Response</span></span>
<span data-ttu-id="f4db2-139">Se tiver êxito, este método retornará um código de resposta e todos os participantes `202 Accepted` receberão uma atualização de lista.</span><span class="sxs-lookup"><span data-stu-id="f4db2-139">If successful, this method returns a `202 Accepted` response code, and all participants will receive a roster update.</span></span>

## <a name="example"></a><span data-ttu-id="f4db2-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f4db2-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f4db2-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f4db2-141">Request</span></span>
<span data-ttu-id="f4db2-142">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="f4db2-142">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f4db2-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="f4db2-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-changeScreenSharingRole"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/changeScreenSharingRole
Content-Type: application/json
Content-Length: 24

{
  "role": "viewer"
}
```
# <a name="c"></a>[<span data-ttu-id="f4db2-144">C#</span><span class="sxs-lookup"><span data-stu-id="f4db2-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-changescreensharingrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f4db2-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f4db2-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-changescreensharingrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f4db2-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f4db2-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-changescreensharingrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f4db2-147">Java</span><span class="sxs-lookup"><span data-stu-id="f4db2-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-changescreensharingrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f4db2-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4db2-148">Response</span></span>
<span data-ttu-id="f4db2-149">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f4db2-149">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 202 Accepted
```
##### <a name="notification---roster-updated-with-participant-sending-screen-sharing-video"></a><span data-ttu-id="f4db2-150">Notificação - lista atualizada com o participante enviando vídeo de compartilhamento de tela</span><span class="sxs-lookup"><span data-stu-id="f4db2-150">Notification - roster updated with participant sending screen sharing video</span></span>
<span data-ttu-id="f4db2-151">Observe a `direction: sendOnly` propriedade no fluxo de mídia.</span><span class="sxs-lookup"><span data-stu-id="f4db2-151">Note the `direction: sendOnly` property on the media stream.</span></span>

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


