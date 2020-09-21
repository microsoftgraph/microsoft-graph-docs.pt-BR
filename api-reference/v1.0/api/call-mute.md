---
title: 'chamada: sem áudio'
description: Permite que o aplicativo se desative.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: c80228d654f41742eed2f96b9e18ac9bfd6ca4d8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47966265"
---
# <a name="call-mute"></a><span data-ttu-id="b22dd-103">chamada: sem áudio</span><span class="sxs-lookup"><span data-stu-id="b22dd-103">call: mute</span></span>

<span data-ttu-id="b22dd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b22dd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b22dd-105">Permite que o aplicativo se desative.</span><span class="sxs-lookup"><span data-stu-id="b22dd-105">Allows the application to mute itself.</span></span>

<span data-ttu-id="b22dd-106">Este é um servidor sem som, o que significa que o servidor irá descartar todos os pacotes de áudio desse participante, mesmo que o participante continue a transmitir áudio.</span><span class="sxs-lookup"><span data-stu-id="b22dd-106">This is a server mute, meaning that the server will drop all audio packets for this participant, even if the participant continues to stream audio.</span></span>

<span data-ttu-id="b22dd-107">Para obter mais detalhes sobre como lidar com operações sem som, consulte [muteParticipantOperation](../resources/muteparticipantoperation.md)</span><span class="sxs-lookup"><span data-stu-id="b22dd-107">For more details about how to handle mute operations, see [muteParticipantOperation](../resources/muteparticipantoperation.md)</span></span>

> <span data-ttu-id="b22dd-108">**Observação:** Este método só tem suporte para chamadas de grupo.</span><span class="sxs-lookup"><span data-stu-id="b22dd-108">**Note:** This method is only supported for group calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="b22dd-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="b22dd-109">Permissions</span></span>
<span data-ttu-id="b22dd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b22dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b22dd-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b22dd-112">Permission type</span></span>                        | <span data-ttu-id="b22dd-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b22dd-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b22dd-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b22dd-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="b22dd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b22dd-115">Not Supported.</span></span>                               |
| <span data-ttu-id="b22dd-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b22dd-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b22dd-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b22dd-117">Not Supported.</span></span>                               |
| <span data-ttu-id="b22dd-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b22dd-118">Application</span></span>                            | <span data-ttu-id="b22dd-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b22dd-119">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="b22dd-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b22dd-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/mute
```

## <a name="request-headers"></a><span data-ttu-id="b22dd-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b22dd-121">Request headers</span></span>
| <span data-ttu-id="b22dd-122">Nome</span><span class="sxs-lookup"><span data-stu-id="b22dd-122">Name</span></span>          | <span data-ttu-id="b22dd-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="b22dd-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="b22dd-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="b22dd-124">Authorization</span></span> | <span data-ttu-id="b22dd-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b22dd-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b22dd-127">Content-type</span><span class="sxs-lookup"><span data-stu-id="b22dd-127">Content-type</span></span> | <span data-ttu-id="b22dd-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b22dd-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b22dd-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b22dd-130">Request body</span></span>
<span data-ttu-id="b22dd-131">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b22dd-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b22dd-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b22dd-132">Parameter</span></span>      | <span data-ttu-id="b22dd-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="b22dd-133">Type</span></span>    |<span data-ttu-id="b22dd-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="b22dd-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b22dd-135">clientContext</span><span class="sxs-lookup"><span data-stu-id="b22dd-135">clientContext</span></span>|<span data-ttu-id="b22dd-136">String</span><span class="sxs-lookup"><span data-stu-id="b22dd-136">String</span></span>|<span data-ttu-id="b22dd-137">Cadeia de caracteres de contexto de cliente exclusivo.</span><span class="sxs-lookup"><span data-stu-id="b22dd-137">Unique Client Context string.</span></span> <span data-ttu-id="b22dd-138">O limite máximo é de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="b22dd-138">Max limit is 256 chars.</span></span>|

## <a name="response"></a><span data-ttu-id="b22dd-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="b22dd-139">Response</span></span>
<span data-ttu-id="b22dd-140">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [muteParticipantOperation](../resources/muteParticipantoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b22dd-140">If successful, this method returns a `200 OK` response code and a [muteParticipantOperation](../resources/muteParticipantoperation.md) object in the response body.</span></span>

> <span data-ttu-id="b22dd-141">**Observação:** Depois que essa operação retornar uma resposta bem-sucedida, todos os participantes receberão uma atualização de lista</span><span class="sxs-lookup"><span data-stu-id="b22dd-141">**Note:** After this operation returns a successful response, all participants will receive a roster update</span></span>

## <a name="example"></a><span data-ttu-id="b22dd-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b22dd-142">Example</span></span>
<span data-ttu-id="b22dd-143">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="b22dd-143">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="b22dd-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b22dd-144">Request</span></span>
<span data-ttu-id="b22dd-145">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="b22dd-145">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b22dd-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="b22dd-146">HTTP</span></span>](#tab/http)
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

# <a name="c"></a>[<span data-ttu-id="b22dd-147">C#</span><span class="sxs-lookup"><span data-stu-id="b22dd-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-mute-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b22dd-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b22dd-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-mute-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b22dd-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b22dd-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-mute-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b22dd-150">Java</span><span class="sxs-lookup"><span data-stu-id="b22dd-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-mute-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b22dd-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="b22dd-151">Response</span></span>

> <span data-ttu-id="b22dd-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b22dd-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span> 
 
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
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.muteParticipantOperation",
  "truncated": true
}-->
```json
{
  "@odata.type": "#microsoft.graph.muteParticipantOperation",
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#muteParticipantOperation",
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "completed",
  "clientContext": "clientContext-value"
}
```

##### <a name="notification---roster-updated-with-participant-muted"></a><span data-ttu-id="b22dd-154">Lista de notificação atualizada com o participante sem som</span><span class="sxs-lookup"><span data-stu-id="b22dd-154">Notification - roster updated with participant muted</span></span>

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

