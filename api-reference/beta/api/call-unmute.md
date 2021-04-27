---
title: 'call: unmute'
description: Permitir que o aplicativo se desmute sozinho.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 1e995e17bfd98b26ae4680c1215a56d231e0116c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047599"
---
# <a name="call-unmute"></a><span data-ttu-id="e2565-103">call: unmute</span><span class="sxs-lookup"><span data-stu-id="e2565-103">call: unmute</span></span>

<span data-ttu-id="e2565-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2565-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2565-105">Permitir que o aplicativo se desmute sozinho.</span><span class="sxs-lookup"><span data-stu-id="e2565-105">Allow the application to unmute itself.</span></span>

<span data-ttu-id="e2565-106">Esse é um servidor sem deslocamento, o que significa que o servidor começará a enviar pacotes de áudio para esse participante para outros participantes novamente.</span><span class="sxs-lookup"><span data-stu-id="e2565-106">This is a server unmute, meaning that the server will start sending audio packets for this participant to other participants again.</span></span>

<span data-ttu-id="e2565-107">Para obter mais informações sobre como lidar com operações sem deslocamento, consulte [unmuteParticipantOperation](../resources/unmuteParticipantoperation.md).</span><span class="sxs-lookup"><span data-stu-id="e2565-107">For more information about how to handle unmute operations, see [unmuteParticipantOperation](../resources/unmuteParticipantoperation.md).</span></span>

> <span data-ttu-id="e2565-108">**Observação:** Esse método só tem suporte para chamadas de grupo.</span><span class="sxs-lookup"><span data-stu-id="e2565-108">**Note:** This method is only supported for group calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="e2565-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="e2565-109">Permissions</span></span>

| <span data-ttu-id="e2565-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e2565-110">Permission type</span></span>                        | <span data-ttu-id="e2565-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e2565-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e2565-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e2565-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="e2565-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e2565-113">Not supported.</span></span>                               |
| <span data-ttu-id="e2565-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e2565-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2565-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e2565-115">Not supported.</span></span>                               |
| <span data-ttu-id="e2565-116">Application</span><span class="sxs-lookup"><span data-stu-id="e2565-116">Application</span></span>                            | <span data-ttu-id="e2565-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e2565-117">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="e2565-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e2565-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/unmute
POST /communications/calls/{id}/unmute
```
> <span data-ttu-id="e2565-119">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="e2565-119">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="e2565-120">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="e2565-120">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e2565-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e2565-121">Request headers</span></span>
| <span data-ttu-id="e2565-122">Nome</span><span class="sxs-lookup"><span data-stu-id="e2565-122">Name</span></span>          | <span data-ttu-id="e2565-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2565-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="e2565-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e2565-124">Authorization</span></span> | <span data-ttu-id="e2565-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e2565-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e2565-127">Content-type</span><span class="sxs-lookup"><span data-stu-id="e2565-127">Content-type</span></span> | <span data-ttu-id="e2565-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e2565-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2565-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e2565-130">Request body</span></span>
<span data-ttu-id="e2565-131">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e2565-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e2565-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e2565-132">Parameter</span></span>      | <span data-ttu-id="e2565-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="e2565-133">Type</span></span>    |<span data-ttu-id="e2565-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2565-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e2565-135">clientContext</span><span class="sxs-lookup"><span data-stu-id="e2565-135">clientContext</span></span>|<span data-ttu-id="e2565-136">String</span><span class="sxs-lookup"><span data-stu-id="e2565-136">String</span></span>|<span data-ttu-id="e2565-137">O contexto do cliente.</span><span class="sxs-lookup"><span data-stu-id="e2565-137">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="e2565-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2565-138">Response</span></span>
<span data-ttu-id="e2565-139">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto unmuteParticipantOperation](../resources/unmuteParticipantoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e2565-139">If successful, this method returns a `200 OK` response code and a [unmuteParticipantOperation](../resources/unmuteParticipantoperation.md) object in the response body.</span></span>

><span data-ttu-id="e2565-140">**Observação:** Quando essa API retornar uma resposta bem-sucedida, todos os participantes receberão uma atualização de lista.</span><span class="sxs-lookup"><span data-stu-id="e2565-140">**Note:** When this API returns a successful response, all participants will receive a roster update.</span></span>

## <a name="example"></a><span data-ttu-id="e2565-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e2565-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e2565-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2565-142">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e2565-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="e2565-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-unmute"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/unmute
Content-Type: application/json
Content-Length: 46

{
  "clientContext": "clientContext-value"
}
```
# <a name="c"></a>[<span data-ttu-id="e2565-144">C#</span><span class="sxs-lookup"><span data-stu-id="e2565-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-unmute-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e2565-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e2565-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-unmute-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e2565-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e2565-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-unmute-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e2565-147">Java</span><span class="sxs-lookup"><span data-stu-id="e2565-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-unmute-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e2565-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2565-148">Response</span></span>

> <span data-ttu-id="e2565-149">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e2565-149">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unmuteParticipantOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
Content-Type: application/json
Content-Length: 259
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.unmuteParticipantOperation",
  "truncated": true
}-->
```json
{
  "@odata.type": "#microsoft.graph.unmuteParticipantOperation",
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#unmuteParticipantOperation",
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "completed",
  "clientContext": "clientContext-value"
}
```

##### <a name="notification---roster-updated-with-participant-unmuted"></a><span data-ttu-id="e2565-150">Notificação - lista atualizada com o participante sem deslocamento</span><span class="sxs-lookup"><span data-stu-id="e2565-150">Notification - roster updated with participant unmuted</span></span>

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


