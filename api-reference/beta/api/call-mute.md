---
title: 'chamada: sem áudio'
description: Permite que o aplicativo se desative.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: d1c9093f6c86f11588b0758a80fdbe8682d6d216
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2019
ms.locfileid: "38005966"
---
# <a name="call-mute"></a><span data-ttu-id="f5e34-103">chamada: sem áudio</span><span class="sxs-lookup"><span data-stu-id="f5e34-103">call: mute</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5e34-104">Permite que o aplicativo se desative.</span><span class="sxs-lookup"><span data-stu-id="f5e34-104">Allows the application to mute itself.</span></span>

## <a name="permissions"></a><span data-ttu-id="f5e34-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f5e34-105">Permissions</span></span>
<span data-ttu-id="f5e34-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5e34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f5e34-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f5e34-108">Permission type</span></span>                        | <span data-ttu-id="f5e34-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f5e34-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f5e34-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f5e34-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f5e34-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5e34-111">Not Supported.</span></span>                               |
| <span data-ttu-id="f5e34-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f5e34-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5e34-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5e34-113">Not Supported.</span></span>                               |
| <span data-ttu-id="f5e34-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f5e34-114">Application</span></span>                            | <span data-ttu-id="f5e34-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f5e34-115">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="f5e34-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f5e34-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/mute
POST /communications/calls/{id}/mute
```
> <span data-ttu-id="f5e34-117">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="f5e34-117">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="f5e34-118">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="f5e34-118">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f5e34-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f5e34-119">Request headers</span></span>
| <span data-ttu-id="f5e34-120">Nome</span><span class="sxs-lookup"><span data-stu-id="f5e34-120">Name</span></span>          | <span data-ttu-id="f5e34-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5e34-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="f5e34-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f5e34-122">Authorization</span></span> | <span data-ttu-id="f5e34-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f5e34-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f5e34-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f5e34-125">Request body</span></span>
<span data-ttu-id="f5e34-126">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f5e34-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f5e34-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f5e34-127">Parameter</span></span>      | <span data-ttu-id="f5e34-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="f5e34-128">Type</span></span>    |<span data-ttu-id="f5e34-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5e34-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f5e34-130">clientContext</span><span class="sxs-lookup"><span data-stu-id="f5e34-130">clientContext</span></span>|<span data-ttu-id="f5e34-131">String</span><span class="sxs-lookup"><span data-stu-id="f5e34-131">String</span></span>|<span data-ttu-id="f5e34-132">O contexto do cliente.</span><span class="sxs-lookup"><span data-stu-id="f5e34-132">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="f5e34-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5e34-133">Response</span></span>
<span data-ttu-id="f5e34-134">Se bem-sucedido, este método retorna `200 OK` um código de resposta e um objeto [commsOperation](../resources/commsoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f5e34-134">If successful, this method returns `200 OK` response code and a [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5e34-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f5e34-135">Example</span></span>
<span data-ttu-id="f5e34-136">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="f5e34-136">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="f5e34-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5e34-137">Request</span></span>
<span data-ttu-id="f5e34-138">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="f5e34-138">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f5e34-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="f5e34-139">HTTP</span></span>](#tab/http)
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

# <a name="ctabcsharp"></a>[<span data-ttu-id="f5e34-140">C#</span><span class="sxs-lookup"><span data-stu-id="f5e34-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-mute-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f5e34-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f5e34-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-mute-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f5e34-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f5e34-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-mute-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f5e34-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5e34-143">Response</span></span>

> <span data-ttu-id="f5e34-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f5e34-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span> 
 
<!-- { 
  "blockType": "response", 
  "truncated": true, 
  "@odata.type": "microsoft.graph.commsOperation" 
} --> 
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
Content-Type: application/json
Content-Length: 259
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsOperation",
  "truncated": true
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsOperation",
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#commsOperation",
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "completed",
  "clientContext": "clientContext-value"
}
```

##### <a name="notification---roster-updated-with-participant-muted"></a><span data-ttu-id="f5e34-146">Lista de notificação atualizada com o participante sem som</span><span class="sxs-lookup"><span data-stu-id="f5e34-146">Notification - roster updated with participant muted</span></span>

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
