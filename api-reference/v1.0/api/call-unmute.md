---
title: 'call: unmute'
description: Permitir que o aplicativo se desmute sozinho.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 392f8af0e53c54d3c4f17f2db7837295eb7039e7
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52783635"
---
# <a name="call-unmute"></a><span data-ttu-id="18967-103">call: unmute</span><span class="sxs-lookup"><span data-stu-id="18967-103">call: unmute</span></span>

<span data-ttu-id="18967-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18967-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="18967-105">Permitir que o aplicativo se desmute sozinho.</span><span class="sxs-lookup"><span data-stu-id="18967-105">Allow the application to unmute itself.</span></span>

<span data-ttu-id="18967-106">Esse é um servidor sem deslocamento, o que significa que o servidor começará a enviar pacotes de áudio para esse participante para outros participantes novamente.</span><span class="sxs-lookup"><span data-stu-id="18967-106">This is a server unmute, meaning that the server will start sending audio packets for this participant to other participants again.</span></span>

<span data-ttu-id="18967-107">Para obter mais informações sobre como lidar com operações sem deslocamento, consulte [unmuteParticipantOperation](../resources/unmuteParticipantoperation.md).</span><span class="sxs-lookup"><span data-stu-id="18967-107">For more information about how to handle unmute operations, see [unmuteParticipantOperation](../resources/unmuteParticipantoperation.md).</span></span>

> <span data-ttu-id="18967-108">**Observação:** Esse método só tem suporte para chamadas de grupo.</span><span class="sxs-lookup"><span data-stu-id="18967-108">**Note:** This method is only supported for group calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="18967-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="18967-109">Permissions</span></span>

| <span data-ttu-id="18967-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="18967-110">Permission type</span></span>                        | <span data-ttu-id="18967-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="18967-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="18967-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="18967-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="18967-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="18967-113">Not supported.</span></span>                               |
| <span data-ttu-id="18967-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="18967-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18967-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="18967-115">Not supported.</span></span>                               |
| <span data-ttu-id="18967-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="18967-116">Application</span></span>                            | <span data-ttu-id="18967-117">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="18967-117">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="18967-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="18967-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/unmute
```

## <a name="request-headers"></a><span data-ttu-id="18967-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="18967-119">Request headers</span></span>
| <span data-ttu-id="18967-120">Nome</span><span class="sxs-lookup"><span data-stu-id="18967-120">Name</span></span>          | <span data-ttu-id="18967-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="18967-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="18967-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="18967-122">Authorization</span></span> | <span data-ttu-id="18967-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="18967-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="18967-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="18967-125">Content-type</span></span> | <span data-ttu-id="18967-p102">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="18967-p102">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="18967-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="18967-128">Request body</span></span>
<span data-ttu-id="18967-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="18967-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="18967-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="18967-130">Parameter</span></span>      | <span data-ttu-id="18967-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="18967-131">Type</span></span>    |<span data-ttu-id="18967-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="18967-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="18967-133">clientContext</span><span class="sxs-lookup"><span data-stu-id="18967-133">clientContext</span></span>|<span data-ttu-id="18967-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18967-134">String</span></span>|<span data-ttu-id="18967-135">Cadeia de caracteres de contexto de cliente exclusiva.</span><span class="sxs-lookup"><span data-stu-id="18967-135">Unique Client Context string.</span></span> <span data-ttu-id="18967-136">O limite máximo é 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="18967-136">Max limit is 256 chars.</span></span>|

## <a name="response"></a><span data-ttu-id="18967-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="18967-137">Response</span></span>
<span data-ttu-id="18967-138">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto unmuteParticipantOperation](../resources/unmuteParticipantoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="18967-138">If successful, this method returns a `200 OK` response code and a [unmuteParticipantOperation](../resources/unmuteParticipantoperation.md) object in the response body.</span></span>

><span data-ttu-id="18967-139">**Observação:** Quando essa API retornar uma resposta bem-sucedida, todos os participantes receberão uma atualização de lista.</span><span class="sxs-lookup"><span data-stu-id="18967-139">**Note:** When this API returns a successful response, all participants will receive a roster update.</span></span>

## <a name="example"></a><span data-ttu-id="18967-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="18967-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="18967-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="18967-141">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="18967-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="18967-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-unmute"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/unmute
Content-Type: application/json
Content-Length: 46

{
  "clientContext": "clientContext-value"
}
```
# <a name="c"></a>[<span data-ttu-id="18967-143">C#</span><span class="sxs-lookup"><span data-stu-id="18967-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-unmute-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="18967-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="18967-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-unmute-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="18967-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="18967-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-unmute-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="18967-146">Java</span><span class="sxs-lookup"><span data-stu-id="18967-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-unmute-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="18967-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="18967-147">Response</span></span>

> <span data-ttu-id="18967-148">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="18967-148">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unmuteParticipantOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/v1.0/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
Content-Type: application/json
Content-Length: 259

{
  "@odata.type": "#microsoft.graph.unmuteParticipantOperation",
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#unmuteParticipantOperation",
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "completed",
  "clientContext": "clientContext-value"
}
```

##### <a name="notification---roster-updated-with-participant-unmuted"></a><span data-ttu-id="18967-149">Notificação - lista atualizada com o participante sem deslocamento</span><span class="sxs-lookup"><span data-stu-id="18967-149">Notification - roster updated with participant unmuted</span></span>
<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json

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
          "isMuted": false, // will be set to false on unmute
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
  "description": "call: unmute",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

