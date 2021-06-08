---
title: 'call: mute'
description: Permite que o aplicativo se silencie.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 016fbd3dbad85dfaf9eb0b09d840532ce27a1c01
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52784924"
---
# <a name="call-mute"></a><span data-ttu-id="345c0-103">call: mute</span><span class="sxs-lookup"><span data-stu-id="345c0-103">call: mute</span></span>

<span data-ttu-id="345c0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="345c0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="345c0-105">Permite que o aplicativo se silencie.</span><span class="sxs-lookup"><span data-stu-id="345c0-105">Allows the application to mute itself.</span></span>

<span data-ttu-id="345c0-106">Esse é um servidor mudo, o que significa que o servidor soltará todos os pacotes de áudio para esse participante, mesmo que o participante continue a transmitir áudio.</span><span class="sxs-lookup"><span data-stu-id="345c0-106">This is a server mute, meaning that the server will drop all audio packets for this participant, even if the participant continues to stream audio.</span></span>

<span data-ttu-id="345c0-107">Para obter mais detalhes sobre como lidar com operações de mudo, consulte [muteParticipantOperation](../resources/muteparticipantoperation.md)</span><span class="sxs-lookup"><span data-stu-id="345c0-107">For more details about how to handle mute operations, see [muteParticipantOperation](../resources/muteparticipantoperation.md)</span></span>

> <span data-ttu-id="345c0-108">**Observação:** Esse método só tem suporte para chamadas de grupo.</span><span class="sxs-lookup"><span data-stu-id="345c0-108">**Note:** This method is only supported for group calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="345c0-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="345c0-109">Permissions</span></span>
<span data-ttu-id="345c0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="345c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="345c0-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="345c0-112">Permission type</span></span>                        | <span data-ttu-id="345c0-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="345c0-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="345c0-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="345c0-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="345c0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="345c0-115">Not Supported.</span></span>                               |
| <span data-ttu-id="345c0-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="345c0-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="345c0-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="345c0-117">Not Supported.</span></span>                               |
| <span data-ttu-id="345c0-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="345c0-118">Application</span></span>                            | <span data-ttu-id="345c0-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="345c0-119">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="345c0-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="345c0-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/mute
```

## <a name="request-headers"></a><span data-ttu-id="345c0-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="345c0-121">Request headers</span></span>
| <span data-ttu-id="345c0-122">Nome</span><span class="sxs-lookup"><span data-stu-id="345c0-122">Name</span></span>          | <span data-ttu-id="345c0-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="345c0-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="345c0-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="345c0-124">Authorization</span></span> | <span data-ttu-id="345c0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="345c0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="345c0-127">Content-type</span><span class="sxs-lookup"><span data-stu-id="345c0-127">Content-type</span></span> | <span data-ttu-id="345c0-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="345c0-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="345c0-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="345c0-130">Request body</span></span>
<span data-ttu-id="345c0-131">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="345c0-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="345c0-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="345c0-132">Parameter</span></span>      | <span data-ttu-id="345c0-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="345c0-133">Type</span></span>    |<span data-ttu-id="345c0-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="345c0-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="345c0-135">clientContext</span><span class="sxs-lookup"><span data-stu-id="345c0-135">clientContext</span></span>|<span data-ttu-id="345c0-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="345c0-136">String</span></span>|<span data-ttu-id="345c0-137">Cadeia de caracteres de contexto de cliente exclusiva.</span><span class="sxs-lookup"><span data-stu-id="345c0-137">Unique Client Context string.</span></span> <span data-ttu-id="345c0-138">O limite máximo é 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="345c0-138">Max limit is 256 chars.</span></span>|

## <a name="response"></a><span data-ttu-id="345c0-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="345c0-139">Response</span></span>
<span data-ttu-id="345c0-140">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto muteParticipantOperation](../resources/muteParticipantoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="345c0-140">If successful, this method returns a `200 OK` response code and a [muteParticipantOperation](../resources/muteParticipantoperation.md) object in the response body.</span></span>

> <span data-ttu-id="345c0-141">**Observação:** Depois que essa operação retornar uma resposta bem-sucedida, todos os participantes receberão uma atualização de lista</span><span class="sxs-lookup"><span data-stu-id="345c0-141">**Note:** After this operation returns a successful response, all participants will receive a roster update</span></span>

## <a name="example"></a><span data-ttu-id="345c0-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="345c0-142">Example</span></span>
<span data-ttu-id="345c0-143">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="345c0-143">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="345c0-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="345c0-144">Request</span></span>
<span data-ttu-id="345c0-145">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="345c0-145">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="345c0-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="345c0-146">HTTP</span></span>](#tab/http)
<!-- { 
  "blockType": "request", 
  "name": "call-mute" 
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/mute
Content-Type: application/json

{
  "clientContext": "clientContext-value"
}
```

# <a name="c"></a>[<span data-ttu-id="345c0-147">C#</span><span class="sxs-lookup"><span data-stu-id="345c0-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-mute-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="345c0-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="345c0-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-mute-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="345c0-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="345c0-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-mute-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="345c0-150">Java</span><span class="sxs-lookup"><span data-stu-id="345c0-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-mute-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="345c0-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="345c0-151">Response</span></span>

> <span data-ttu-id="345c0-152">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="345c0-152">**Note:** The response object shown here might be shortened for readability.</span></span> 
 
<!-- { 
  "blockType": "response", 
  "truncated": true, 
  "@odata.type": "microsoft.graph.muteParticipantOperation" 
} --> 
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/v1.0/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
Content-Type: application/json
Content-Length: 259

{
  "@odata.type": "#microsoft.graph.muteParticipantOperation",
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#muteParticipantOperation",
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "completed",
  "clientContext": "clientContext-value"
}
```

##### <a name="notification---roster-updated-with-participant-muted"></a><span data-ttu-id="345c0-153">Notificação - lista atualizada com o participante em mudo</span><span class="sxs-lookup"><span data-stu-id="345c0-153">Notification - roster updated with participant muted</span></span>

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

