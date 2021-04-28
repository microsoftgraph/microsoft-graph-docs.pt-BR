---
title: 'participante: mute'
description: Silencie um participante específico na chamada.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: a74b2ed36831960ba27b48742f91f99333c69efb
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051309"
---
# <a name="participant-mute"></a><span data-ttu-id="59d3d-103">participante: mute</span><span class="sxs-lookup"><span data-stu-id="59d3d-103">participant: mute</span></span>

<span data-ttu-id="59d3d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59d3d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="59d3d-105">Silencie um participante específico na chamada.</span><span class="sxs-lookup"><span data-stu-id="59d3d-105">Mute a specific participant in the call.</span></span>

<span data-ttu-id="59d3d-106">Esse é um servidor mudo, o que significa que o servidor soltará todos os pacotes de áudio para esse participante, mesmo que o participante continue a transmitir áudio.</span><span class="sxs-lookup"><span data-stu-id="59d3d-106">This is a server mute, meaning that the server will drop all audio packets for this participant, even if the participant continues to stream audio.</span></span>

<span data-ttu-id="59d3d-107">Para obter mais informações sobre como lidar com operações de mudo, consulte [muteParticipantOperation](../resources/muteParticipantoperation.md).</span><span class="sxs-lookup"><span data-stu-id="59d3d-107">For more information about how to handle mute operations, see [muteParticipantOperation](../resources/muteParticipantoperation.md).</span></span>

> <span data-ttu-id="59d3d-108">**Observação:** Esse método só tem suporte para chamadas de grupo.</span><span class="sxs-lookup"><span data-stu-id="59d3d-108">**Note:** This method is only supported for group calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="59d3d-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="59d3d-109">Permissions</span></span>

| <span data-ttu-id="59d3d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="59d3d-110">Permission type</span></span> | <span data-ttu-id="59d3d-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="59d3d-111">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="59d3d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="59d3d-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="59d3d-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="59d3d-113">Not Supported</span></span>        |
| <span data-ttu-id="59d3d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="59d3d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59d3d-115">Não suportado</span><span class="sxs-lookup"><span data-stu-id="59d3d-115">Not Supported</span></span>        |
| <span data-ttu-id="59d3d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="59d3d-116">Application</span></span>     | <span data-ttu-id="59d3d-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="59d3d-117">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="59d3d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="59d3d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/participants/{id}/mute
```

## <a name="request-headers"></a><span data-ttu-id="59d3d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="59d3d-119">Request headers</span></span>
| <span data-ttu-id="59d3d-120">Nome</span><span class="sxs-lookup"><span data-stu-id="59d3d-120">Name</span></span>          | <span data-ttu-id="59d3d-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="59d3d-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="59d3d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="59d3d-122">Authorization</span></span> | <span data-ttu-id="59d3d-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59d3d-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="59d3d-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="59d3d-125">Content-type</span></span>  | <span data-ttu-id="59d3d-p102">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59d3d-p102">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="59d3d-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="59d3d-128">Request body</span></span>
<span data-ttu-id="59d3d-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="59d3d-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="59d3d-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="59d3d-130">Parameter</span></span>      | <span data-ttu-id="59d3d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="59d3d-131">Type</span></span>    |<span data-ttu-id="59d3d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="59d3d-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="59d3d-133">clientContext</span><span class="sxs-lookup"><span data-stu-id="59d3d-133">clientContext</span></span>|<span data-ttu-id="59d3d-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59d3d-134">String</span></span>|<span data-ttu-id="59d3d-135">Cadeia de caracteres de contexto de cliente exclusiva.</span><span class="sxs-lookup"><span data-stu-id="59d3d-135">Unique Client Context string.</span></span> <span data-ttu-id="59d3d-136">O limite máximo é 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="59d3d-136">Max limit is 256 chars.</span></span>|

## <a name="response"></a><span data-ttu-id="59d3d-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="59d3d-137">Response</span></span>
<span data-ttu-id="59d3d-138">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto muteParticipantOperation](../resources/muteParticipantoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59d3d-138">If successful, this method returns a `200 OK` response code and a [muteParticipantOperation](../resources/muteParticipantoperation.md) object in the response body.</span></span>

><span data-ttu-id="59d3d-139">**Observação:** Quando essa API retornar uma resposta bem-sucedida, todos os participantes receberão uma atualização de lista.</span><span class="sxs-lookup"><span data-stu-id="59d3d-139">**Note:** When this API returns a successful response, all participants will receive a roster update.</span></span>

## <a name="example---mute-specific-participant"></a><span data-ttu-id="59d3d-140">Exemplo - Mudo de participante específico</span><span class="sxs-lookup"><span data-stu-id="59d3d-140">Example - Mute specific participant</span></span>
<span data-ttu-id="59d3d-141">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="59d3d-141">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="59d3d-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="59d3d-142">Request</span></span>
<span data-ttu-id="59d3d-143">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="59d3d-143">The following example shows the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="59d3d-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="59d3d-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "participant-mute"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/participants/2765eb15-01f8-47c6-b12b-c32111a4a86f/mute
Content-Type: application/json

{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```
# <a name="c"></a>[<span data-ttu-id="59d3d-145">C#</span><span class="sxs-lookup"><span data-stu-id="59d3d-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-mute-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="59d3d-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="59d3d-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-mute-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="59d3d-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="59d3d-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-mute-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="59d3d-148">Java</span><span class="sxs-lookup"><span data-stu-id="59d3d-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/participant-mute-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="59d3d-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="59d3d-149">Response</span></span>

> <span data-ttu-id="59d3d-150">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="59d3d-150">**Note:** The response object shown here might be shortened for readability.</span></span> 


<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.muteParticipantOperation",
  "truncated": true
}-->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/v1.0/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.muteParticipantOperation",
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#muteParticipantOperation",
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "completed",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

##### <a name="notification---roster-updated-with-participant-muted"></a><span data-ttu-id="59d3d-151">Notificação - lista atualizada com o participante em mudo</span><span class="sxs-lookup"><span data-stu-id="59d3d-151">Notification - roster updated with participant muted</span></span>

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
  "description": "participant: mute",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

