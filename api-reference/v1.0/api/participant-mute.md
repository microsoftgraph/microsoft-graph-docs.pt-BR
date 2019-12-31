---
title: 'participante: sem áudio'
description: Ativar mudo de um participante específico na chamada.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 2c65bf06524b883ca4632a6127e50a13e4355054
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913419"
---
# <a name="participant-mute"></a><span data-ttu-id="18284-103">participante: sem áudio</span><span class="sxs-lookup"><span data-stu-id="18284-103">participant: mute</span></span>

<span data-ttu-id="18284-104">Ativar mudo de um participante específico na chamada.</span><span class="sxs-lookup"><span data-stu-id="18284-104">Mute a specific participant in the call.</span></span>

<span data-ttu-id="18284-105">Este é um servidor sem som, o que significa que o servidor irá descartar todos os pacotes de áudio desse participante, mesmo que o participante continue a transmitir áudio.</span><span class="sxs-lookup"><span data-stu-id="18284-105">This is a server mute, meaning that the server will drop all audio packets for this participant, even if the participant continues to stream audio.</span></span>

<span data-ttu-id="18284-106">Para obter mais informações sobre como lidar com operações sem som, consulte [muteParticipantOperation](../resources/muteParticipantoperation.md).</span><span class="sxs-lookup"><span data-stu-id="18284-106">For more information about how to handle mute operations, see [muteParticipantOperation](../resources/muteParticipantoperation.md).</span></span>

> <span data-ttu-id="18284-107">**Observação:** Este método só tem suporte para chamadas de grupo.</span><span class="sxs-lookup"><span data-stu-id="18284-107">**Note:** This method is only supported for group calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="18284-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="18284-108">Permissions</span></span>

| <span data-ttu-id="18284-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="18284-109">Permission type</span></span> | <span data-ttu-id="18284-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="18284-110">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="18284-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="18284-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="18284-112">Não suportado</span><span class="sxs-lookup"><span data-stu-id="18284-112">Not Supported</span></span>        |
| <span data-ttu-id="18284-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="18284-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18284-114">Não suportado</span><span class="sxs-lookup"><span data-stu-id="18284-114">Not Supported</span></span>        |
| <span data-ttu-id="18284-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="18284-115">Application</span></span>     | <span data-ttu-id="18284-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="18284-116">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="18284-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="18284-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/participants/{id}/mute
```

## <a name="request-headers"></a><span data-ttu-id="18284-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="18284-118">Request headers</span></span>
| <span data-ttu-id="18284-119">Nome</span><span class="sxs-lookup"><span data-stu-id="18284-119">Name</span></span>          | <span data-ttu-id="18284-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="18284-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="18284-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="18284-121">Authorization</span></span> | <span data-ttu-id="18284-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="18284-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="18284-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="18284-124">Content-type</span></span>  | <span data-ttu-id="18284-p102">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="18284-p102">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="18284-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="18284-127">Request body</span></span>
<span data-ttu-id="18284-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="18284-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="18284-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="18284-129">Parameter</span></span>      | <span data-ttu-id="18284-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="18284-130">Type</span></span>    |<span data-ttu-id="18284-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="18284-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="18284-132">clientContext</span><span class="sxs-lookup"><span data-stu-id="18284-132">clientContext</span></span>|<span data-ttu-id="18284-133">String</span><span class="sxs-lookup"><span data-stu-id="18284-133">String</span></span>|<span data-ttu-id="18284-134">Cadeia de caracteres de contexto de cliente exclusivo.</span><span class="sxs-lookup"><span data-stu-id="18284-134">Unique Client Context string.</span></span> <span data-ttu-id="18284-135">O limite máximo é de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="18284-135">Max limit is 256 chars.</span></span>|

## <a name="response"></a><span data-ttu-id="18284-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="18284-136">Response</span></span>
<span data-ttu-id="18284-137">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [muteParticipantOperation](../resources/muteParticipantoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="18284-137">If successful, this method returns a `200 OK` response code and a [muteParticipantOperation](../resources/muteParticipantoperation.md) object in the response body.</span></span>

><span data-ttu-id="18284-138">**Observação:** Quando essa API retornar uma resposta bem-sucedida, todos os participantes receberão uma atualização de lista.</span><span class="sxs-lookup"><span data-stu-id="18284-138">**Note:** When this API returns a successful response, all participants will receive a roster update.</span></span>

## <a name="example---mute-specific-participant"></a><span data-ttu-id="18284-139">Exemplo-sem áudio o participante específico</span><span class="sxs-lookup"><span data-stu-id="18284-139">Example - Mute specific participant</span></span>
<span data-ttu-id="18284-140">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="18284-140">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="18284-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="18284-141">Request</span></span>
<span data-ttu-id="18284-142">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="18284-142">The following example shows the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="18284-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="18284-143">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="18284-144">C#</span><span class="sxs-lookup"><span data-stu-id="18284-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-mute-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="18284-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="18284-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-mute-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="18284-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="18284-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-mute-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="18284-147">Java</span><span class="sxs-lookup"><span data-stu-id="18284-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/participant-mute-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="18284-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="18284-148">Response</span></span>

> <span data-ttu-id="18284-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="18284-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span> 


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

##### <a name="notification---roster-updated-with-participant-muted"></a><span data-ttu-id="18284-151">Lista de notificação atualizada com o participante sem som</span><span class="sxs-lookup"><span data-stu-id="18284-151">Notification - roster updated with participant muted</span></span>

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
