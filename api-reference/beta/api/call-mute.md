---
title: 'call: mute'
description: Permite que o aplicativo se silencie.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: c681698b34395fda542a96f6a94941a8e3f25a74
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786233"
---
# <a name="call-mute"></a><span data-ttu-id="e65fb-103">call: mute</span><span class="sxs-lookup"><span data-stu-id="e65fb-103">call: mute</span></span>

<span data-ttu-id="e65fb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e65fb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e65fb-105">Permite que o aplicativo se silencie.</span><span class="sxs-lookup"><span data-stu-id="e65fb-105">Allows the application to mute itself.</span></span>

<span data-ttu-id="e65fb-106">Esse é um servidor mudo, o que significa que o servidor soltará todos os pacotes de áudio para esse participante, mesmo que o participante continue a transmitir áudio.</span><span class="sxs-lookup"><span data-stu-id="e65fb-106">This is a server mute, meaning that the server will drop all audio packets for this participant, even if the participant continues to stream audio.</span></span>

<span data-ttu-id="e65fb-107">Para obter mais detalhes sobre como lidar com operações de mudo, consulte [muteParticipantOperation](../resources/muteparticipantoperation.md)</span><span class="sxs-lookup"><span data-stu-id="e65fb-107">For more details about how to handle mute operations, see [muteParticipantOperation](../resources/muteparticipantoperation.md)</span></span>

> <span data-ttu-id="e65fb-108">**Observação:** Esse método só tem suporte para chamadas de grupo.</span><span class="sxs-lookup"><span data-stu-id="e65fb-108">**Note:** This method is only supported for group calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="e65fb-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="e65fb-109">Permissions</span></span>
<span data-ttu-id="e65fb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e65fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e65fb-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e65fb-112">Permission type</span></span>                        | <span data-ttu-id="e65fb-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e65fb-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e65fb-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e65fb-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="e65fb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e65fb-115">Not Supported.</span></span>                               |
| <span data-ttu-id="e65fb-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e65fb-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e65fb-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e65fb-117">Not Supported.</span></span>                               |
| <span data-ttu-id="e65fb-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e65fb-118">Application</span></span>                            | <span data-ttu-id="e65fb-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e65fb-119">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="e65fb-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e65fb-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/mute
POST /communications/calls/{id}/mute
```
> <span data-ttu-id="e65fb-121">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="e65fb-121">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="e65fb-122">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="e65fb-122">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e65fb-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e65fb-123">Request headers</span></span>
| <span data-ttu-id="e65fb-124">Nome</span><span class="sxs-lookup"><span data-stu-id="e65fb-124">Name</span></span>          | <span data-ttu-id="e65fb-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="e65fb-125">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="e65fb-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="e65fb-126">Authorization</span></span> | <span data-ttu-id="e65fb-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e65fb-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e65fb-129">Content-type</span><span class="sxs-lookup"><span data-stu-id="e65fb-129">Content-type</span></span> | <span data-ttu-id="e65fb-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e65fb-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e65fb-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e65fb-132">Request body</span></span>
<span data-ttu-id="e65fb-133">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e65fb-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e65fb-134">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e65fb-134">Parameter</span></span>      | <span data-ttu-id="e65fb-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="e65fb-135">Type</span></span>    |<span data-ttu-id="e65fb-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="e65fb-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e65fb-137">clientContext</span><span class="sxs-lookup"><span data-stu-id="e65fb-137">clientContext</span></span>|<span data-ttu-id="e65fb-138">String</span><span class="sxs-lookup"><span data-stu-id="e65fb-138">String</span></span>|<span data-ttu-id="e65fb-139">O contexto do cliente.</span><span class="sxs-lookup"><span data-stu-id="e65fb-139">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="e65fb-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="e65fb-140">Response</span></span>
<span data-ttu-id="e65fb-141">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto muteParticipantOperation](../resources/muteParticipantoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e65fb-141">If successful, this method returns a `200 OK` response code and a [muteParticipantOperation](../resources/muteParticipantoperation.md) object in the response body.</span></span>

> <span data-ttu-id="e65fb-142">**Observação:** Depois que essa operação retornar uma resposta bem-sucedida, todos os participantes receberão uma atualização de lista</span><span class="sxs-lookup"><span data-stu-id="e65fb-142">**Note:** After this operation returns a successful response, all participants will receive a roster update</span></span>

## <a name="example"></a><span data-ttu-id="e65fb-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e65fb-143">Example</span></span>
<span data-ttu-id="e65fb-144">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="e65fb-144">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="e65fb-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e65fb-145">Request</span></span>
<span data-ttu-id="e65fb-146">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="e65fb-146">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e65fb-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="e65fb-147">HTTP</span></span>](#tab/http)
<!-- { 
  "blockType": "request", 
  "name": "call-mute" 
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/mute
Content-Type: application/json

{
  "clientContext": "clientContext-value"
}
```

# <a name="c"></a>[<span data-ttu-id="e65fb-148">C#</span><span class="sxs-lookup"><span data-stu-id="e65fb-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-mute-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e65fb-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e65fb-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-mute-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e65fb-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e65fb-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-mute-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e65fb-151">Java</span><span class="sxs-lookup"><span data-stu-id="e65fb-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-mute-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e65fb-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="e65fb-152">Response</span></span>

> <span data-ttu-id="e65fb-153">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e65fb-153">**Note:** The response object shown here might be shortened for readability.</span></span> 
 
<!-- { 
  "blockType": "response", 
  "truncated": true, 
  "@odata.type": "microsoft.graph.muteParticipantOperation" 
} --> 
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
Content-Type: application/json
Content-Length: 259

{
  "@odata.type": "#microsoft.graph.muteParticipantOperation",
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#muteParticipantOperation",
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "completed",
  "clientContext": "clientContext-value"
}
```

##### <a name="notification---roster-updated-with-participant-muted"></a><span data-ttu-id="e65fb-154">Notificação - lista atualizada com o participante em mudo</span><span class="sxs-lookup"><span data-stu-id="e65fb-154">Notification - roster updated with participant muted</span></span>

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
              "mediaType": "audio",
              "label": "main-audio",
              "sourceId": "1",
              "direction": "sendReceive"
            }
          ],
          "isMuted": true, // will be set to true on mute
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
  "description": "call: mute",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


