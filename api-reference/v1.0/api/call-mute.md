---
title: 'chamada: sem áudio'
description: Permite que o aplicativo se desative.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 8dfa1b4d0cda515dfe6e5ae6303bcbdccd7c231a
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865725"
---
# <a name="call-mute"></a><span data-ttu-id="70feb-103">chamada: sem áudio</span><span class="sxs-lookup"><span data-stu-id="70feb-103">call: mute</span></span>

<span data-ttu-id="70feb-104">Permite que o aplicativo se desative.</span><span class="sxs-lookup"><span data-stu-id="70feb-104">Allows the application to mute itself.</span></span>

<span data-ttu-id="70feb-105">Este é um servidor sem som, o que significa que o servidor irá descartar todos os pacotes de áudio desse participante, mesmo que o participante continue a transmitir áudio.</span><span class="sxs-lookup"><span data-stu-id="70feb-105">This is a server mute, meaning that the server will drop all audio packets for this participant, even if the participant continues to stream audio.</span></span>

<span data-ttu-id="70feb-106">Para obter mais detalhes sobre como lidar com operações sem som, consulte [muteParticipantOperation](../resources/muteparticipantoperation.md)</span><span class="sxs-lookup"><span data-stu-id="70feb-106">For more details about how to handle mute operations, see [muteParticipantOperation](../resources/muteparticipantoperation.md)</span></span>

> <span data-ttu-id="70feb-107">**Observação:** Este método só tem suporte para chamadas de grupo.</span><span class="sxs-lookup"><span data-stu-id="70feb-107">**Note:** This method is only supported for group calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="70feb-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="70feb-108">Permissions</span></span>
<span data-ttu-id="70feb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70feb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="70feb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="70feb-111">Permission type</span></span>                        | <span data-ttu-id="70feb-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="70feb-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="70feb-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="70feb-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="70feb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="70feb-114">Not Supported.</span></span>                               |
| <span data-ttu-id="70feb-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="70feb-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70feb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="70feb-116">Not Supported.</span></span>                               |
| <span data-ttu-id="70feb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="70feb-117">Application</span></span>                            | <span data-ttu-id="70feb-118">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="70feb-118">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="70feb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="70feb-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/mute
```

## <a name="request-headers"></a><span data-ttu-id="70feb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="70feb-120">Request headers</span></span>
| <span data-ttu-id="70feb-121">Nome</span><span class="sxs-lookup"><span data-stu-id="70feb-121">Name</span></span>          | <span data-ttu-id="70feb-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="70feb-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="70feb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="70feb-123">Authorization</span></span> | <span data-ttu-id="70feb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="70feb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="70feb-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="70feb-126">Content-type</span></span> | <span data-ttu-id="70feb-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="70feb-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="70feb-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="70feb-129">Request body</span></span>
<span data-ttu-id="70feb-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="70feb-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="70feb-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="70feb-131">Parameter</span></span>      | <span data-ttu-id="70feb-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="70feb-132">Type</span></span>    |<span data-ttu-id="70feb-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="70feb-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="70feb-134">clientContext</span><span class="sxs-lookup"><span data-stu-id="70feb-134">clientContext</span></span>|<span data-ttu-id="70feb-135">String</span><span class="sxs-lookup"><span data-stu-id="70feb-135">String</span></span>|<span data-ttu-id="70feb-136">Cadeia de caracteres de contexto de cliente exclusivo.</span><span class="sxs-lookup"><span data-stu-id="70feb-136">Unique Client Context string.</span></span> <span data-ttu-id="70feb-137">O limite máximo é de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="70feb-137">Max limit is 256 chars.</span></span>|

## <a name="response"></a><span data-ttu-id="70feb-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="70feb-138">Response</span></span>
<span data-ttu-id="70feb-139">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [muteParticipantOperation](../resources/muteParticipantoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="70feb-139">If successful, this method returns a `200 OK` response code and a [muteParticipantOperation](../resources/muteParticipantoperation.md) object in the response body.</span></span>

> <span data-ttu-id="70feb-140">**Observação:** Depois que essa operação retornar uma resposta bem-sucedida, todos os participantes receberão uma atualização de lista</span><span class="sxs-lookup"><span data-stu-id="70feb-140">**Note:** After this operation returns a successful response, all participants will receive a roster update</span></span>

## <a name="example"></a><span data-ttu-id="70feb-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="70feb-141">Example</span></span>
<span data-ttu-id="70feb-142">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="70feb-142">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="70feb-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="70feb-143">Request</span></span>
<span data-ttu-id="70feb-144">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="70feb-144">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="70feb-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="70feb-145">HTTP</span></span>](#tab/http)
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

# <a name="ctabcsharp"></a>[<span data-ttu-id="70feb-146">C#</span><span class="sxs-lookup"><span data-stu-id="70feb-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-mute-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="70feb-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="70feb-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-mute-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="70feb-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="70feb-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-mute-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="70feb-149">Java</span><span class="sxs-lookup"><span data-stu-id="70feb-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-mute-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="70feb-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="70feb-150">Response</span></span>

> <span data-ttu-id="70feb-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="70feb-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span> 
 
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

##### <a name="notification---roster-updated-with-participant-muted"></a><span data-ttu-id="70feb-153">Lista de notificação atualizada com o participante sem som</span><span class="sxs-lookup"><span data-stu-id="70feb-153">Notification - roster updated with participant muted</span></span>

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
