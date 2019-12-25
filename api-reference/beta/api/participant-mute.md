---
title: 'participante: sem áudio'
description: Ativar mudo de um participante específico na chamada.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 1c720ce79b4c31b2895e6d953ab0e36cbb2450be
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869322"
---
# <a name="participant-mute"></a><span data-ttu-id="cbabf-103">participante: sem áudio</span><span class="sxs-lookup"><span data-stu-id="cbabf-103">participant: mute</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cbabf-104">Ativar mudo de um participante específico na chamada.</span><span class="sxs-lookup"><span data-stu-id="cbabf-104">Mute a specific participant in the call.</span></span>

<span data-ttu-id="cbabf-105">Este é um servidor sem som, o que significa que o servidor irá descartar todos os pacotes de áudio desse participante, mesmo que o participante continue a transmitir áudio.</span><span class="sxs-lookup"><span data-stu-id="cbabf-105">This is a server mute, meaning that the server will drop all audio packets for this participant, even if the participant continues to stream audio.</span></span>

<span data-ttu-id="cbabf-106">Para obter mais informações sobre como lidar com operações sem som, consulte [muteParticipantOperation](../resources/muteParticipantoperation.md).</span><span class="sxs-lookup"><span data-stu-id="cbabf-106">For more information about how to handle mute operations, see [muteParticipantOperation](../resources/muteParticipantoperation.md).</span></span>

> <span data-ttu-id="cbabf-107">**Observação:** Este método só tem suporte para chamadas de grupo.</span><span class="sxs-lookup"><span data-stu-id="cbabf-107">**Note:** This method is only supported for group calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="cbabf-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="cbabf-108">Permissions</span></span>

| <span data-ttu-id="cbabf-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cbabf-109">Permission type</span></span> | <span data-ttu-id="cbabf-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cbabf-110">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="cbabf-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cbabf-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cbabf-112">Não suportado</span><span class="sxs-lookup"><span data-stu-id="cbabf-112">Not Supported</span></span>        |
| <span data-ttu-id="cbabf-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cbabf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cbabf-114">Não suportado</span><span class="sxs-lookup"><span data-stu-id="cbabf-114">Not Supported</span></span>        |
| <span data-ttu-id="cbabf-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cbabf-115">Application</span></span>     | <span data-ttu-id="cbabf-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cbabf-116">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="cbabf-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cbabf-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/{id}/mute
POST /communications/calls/{id}/participants/{id}/mute
```
> <span data-ttu-id="cbabf-118">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="cbabf-118">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="cbabf-119">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="cbabf-119">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cbabf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cbabf-120">Request headers</span></span>
| <span data-ttu-id="cbabf-121">Nome</span><span class="sxs-lookup"><span data-stu-id="cbabf-121">Name</span></span>          | <span data-ttu-id="cbabf-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="cbabf-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="cbabf-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cbabf-123">Authorization</span></span> | <span data-ttu-id="cbabf-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cbabf-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cbabf-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="cbabf-126">Content-type</span></span>  | <span data-ttu-id="cbabf-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cbabf-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cbabf-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cbabf-129">Request body</span></span>
<span data-ttu-id="cbabf-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cbabf-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="cbabf-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="cbabf-131">Parameter</span></span>      | <span data-ttu-id="cbabf-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="cbabf-132">Type</span></span>    |<span data-ttu-id="cbabf-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="cbabf-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cbabf-134">clientContext</span><span class="sxs-lookup"><span data-stu-id="cbabf-134">clientContext</span></span>|<span data-ttu-id="cbabf-135">String</span><span class="sxs-lookup"><span data-stu-id="cbabf-135">String</span></span>|<span data-ttu-id="cbabf-136">Cadeia de caracteres de contexto de cliente exclusivo.</span><span class="sxs-lookup"><span data-stu-id="cbabf-136">Unique Client Context string.</span></span> <span data-ttu-id="cbabf-137">O limite máximo é de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="cbabf-137">Max limit is 256 chars.</span></span>|

## <a name="response"></a><span data-ttu-id="cbabf-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="cbabf-138">Response</span></span>
<span data-ttu-id="cbabf-139">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [muteParticipantOperation](../resources/muteParticipantoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cbabf-139">If successful, this method returns a `200 OK` response code and a [muteParticipantOperation](../resources/muteParticipantoperation.md) object in the response body.</span></span>

><span data-ttu-id="cbabf-140">**Observação:** Quando essa API retornar uma resposta bem-sucedida, todos os participantes receberão uma atualização de lista.</span><span class="sxs-lookup"><span data-stu-id="cbabf-140">**Note:** When this API returns a successful response, all participants will receive a roster update.</span></span>

## <a name="example---mute-specific-participant"></a><span data-ttu-id="cbabf-141">Exemplo-sem áudio o participante específico</span><span class="sxs-lookup"><span data-stu-id="cbabf-141">Example - Mute specific participant</span></span>
<span data-ttu-id="cbabf-142">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="cbabf-142">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="cbabf-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cbabf-143">Request</span></span>
<span data-ttu-id="cbabf-144">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="cbabf-144">The following example shows the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="cbabf-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="cbabf-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "participant-mute"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/participants/2765eb15-01f8-47c6-b12b-c32111a4a86f/mute
Content-Type: application/json

{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cbabf-146">C#</span><span class="sxs-lookup"><span data-stu-id="cbabf-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-mute-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cbabf-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cbabf-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-mute-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cbabf-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cbabf-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-mute-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="cbabf-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="cbabf-149">Response</span></span>

> <span data-ttu-id="cbabf-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cbabf-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span> 


<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.muteParticipantOperation",
  "truncated": true
}-->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.muteParticipantOperation",
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#muteParticipantOperation",
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "completed",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

##### <a name="notification---roster-updated-with-participant-muted"></a><span data-ttu-id="cbabf-152">Lista de notificação atualizada com o participante sem som</span><span class="sxs-lookup"><span data-stu-id="cbabf-152">Notification - roster updated with participant muted</span></span>

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
