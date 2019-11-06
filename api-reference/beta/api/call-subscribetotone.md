---
title: 'Call: subscribeToTone'
description: Assine o DTMF (sinalização de multifrequência de tom dual). Isso permite que você seja notificado quando o usuário pressionar teclas em um ' dialpad '.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 50ff5f41c7637ebe79771db81889e89f982a0d92
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2019
ms.locfileid: "38005934"
---
# <a name="call-subscribetotone"></a><span data-ttu-id="1cf1a-104">Call: subscribeToTone</span><span class="sxs-lookup"><span data-stu-id="1cf1a-104">call: subscribeToTone</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1cf1a-105">Assine o DTMF (sinalização de multifrequência de tom dual).</span><span class="sxs-lookup"><span data-stu-id="1cf1a-105">Subscribe to DTMF (dual-tone multi-frequency signaling).</span></span> <span data-ttu-id="1cf1a-106">Isso permite que você seja notificado quando o usuário pressionar teclas em um "dialpad".</span><span class="sxs-lookup"><span data-stu-id="1cf1a-106">This allows you to be notified when the user presses keys on a "Dialpad".</span></span>

> [!Note]
> <span data-ttu-id="1cf1a-107">A ação **subscribeToTone** é suportada apenas para [chamadas](../resources/call.md) que são iniciadas com o [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span><span class="sxs-lookup"><span data-stu-id="1cf1a-107">The **subscribeToTone** action is supported only for [calls](../resources/call.md) that are initiated with [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1cf1a-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="1cf1a-108">Permissions</span></span>
<span data-ttu-id="1cf1a-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1cf1a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1cf1a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1cf1a-111">Permission type</span></span> | <span data-ttu-id="1cf1a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1cf1a-112">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="1cf1a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1cf1a-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="1cf1a-114">Não suportado</span><span class="sxs-lookup"><span data-stu-id="1cf1a-114">Not Supported</span></span>        |
| <span data-ttu-id="1cf1a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1cf1a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1cf1a-116">Não suportado</span><span class="sxs-lookup"><span data-stu-id="1cf1a-116">Not Supported</span></span>        |
| <span data-ttu-id="1cf1a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1cf1a-117">Application</span></span>     | <span data-ttu-id="1cf1a-118">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="1cf1a-118">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="1cf1a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1cf1a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/subscribeToTone
POST /communications/calls/{id}/subscribeToTone
```
> <span data-ttu-id="1cf1a-120">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="1cf1a-120">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="1cf1a-121">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="1cf1a-121">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1cf1a-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1cf1a-122">Request headers</span></span>
| <span data-ttu-id="1cf1a-123">Nome</span><span class="sxs-lookup"><span data-stu-id="1cf1a-123">Name</span></span>          | <span data-ttu-id="1cf1a-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="1cf1a-124">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="1cf1a-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="1cf1a-125">Authorization</span></span> | <span data-ttu-id="1cf1a-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1cf1a-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1cf1a-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1cf1a-128">Request body</span></span>
<span data-ttu-id="1cf1a-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1cf1a-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1cf1a-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="1cf1a-130">Parameter</span></span>      | <span data-ttu-id="1cf1a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1cf1a-131">Type</span></span>    | <span data-ttu-id="1cf1a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1cf1a-132">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="1cf1a-133">clientContext</span><span class="sxs-lookup"><span data-stu-id="1cf1a-133">clientContext</span></span>  | <span data-ttu-id="1cf1a-134">String</span><span class="sxs-lookup"><span data-stu-id="1cf1a-134">String</span></span>  | <span data-ttu-id="1cf1a-135">Cadeia de caracteres de contexto de cliente exclusivo.</span><span class="sxs-lookup"><span data-stu-id="1cf1a-135">Unique client context string.</span></span> <span data-ttu-id="1cf1a-136">Pode ter um máximo de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="1cf1a-136">Can have a maximum of 256 characters.</span></span> |

## <a name="response"></a><span data-ttu-id="1cf1a-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="1cf1a-137">Response</span></span>
<span data-ttu-id="1cf1a-138">Se bem sucedido, este método retorna um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="1cf1a-138">If successful, this method returns `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1cf1a-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1cf1a-139">Example</span></span>
<span data-ttu-id="1cf1a-140">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="1cf1a-140">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="1cf1a-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1cf1a-141">Request</span></span>
<span data-ttu-id="1cf1a-142">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="1cf1a-142">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="1cf1a-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="1cf1a-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-subscribeToTone"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/subscribeToTone
Content-Type: application/json
Content-Length: 46

{
  "clientContext": "fd1c7836-4d84-4e24-b6aa-23188688cc54"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1cf1a-144">C#</span><span class="sxs-lookup"><span data-stu-id="1cf1a-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-subscribetotone-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1cf1a-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1cf1a-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-subscribetotone-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1cf1a-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1cf1a-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-subscribetotone-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1cf1a-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="1cf1a-147">Response</span></span>

> <span data-ttu-id="1cf1a-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1cf1a-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/communications/calls/421f1100-411f-4a29-8514-dbbb9caff45a/operations/ea91863c-d0a6-4de0-b73a-4c8d63da5d87
Content-Type: application/json
Content-Length: 259

{
  "id": "ea91863c-d0a6-4de0-b73a-4c8d63da5d87",
  "status": "completed",
  "clientContext": "fd1c7836-4d84-4e24-b6aa-23188688cc54",
}
```


##### <a name="notification---tone-notification"></a><span data-ttu-id="1cf1a-150">Notificação de sinal de notificação</span><span class="sxs-lookup"><span data-stu-id="1cf1a-150">Notification - tone notification</span></span>

<span data-ttu-id="1cf1a-151">A notificação contém informações sobre o Tom pressionado no recurso [toneinfo](../resources/toneinfo.md) .</span><span class="sxs-lookup"><span data-stu-id="1cf1a-151">The notification contain information of the tone pressed in the [toneinfo](../resources/toneinfo.md) resource.</span></span>

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
      "resourceUrl": "/communications/calls/421f1100-411f-4a29-8514-dbbb9caff45",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "established",
        "toneInfo": {
          "@odata.type": "#microsoft.graph.toneInfo",
          "sequenceId": 1,
          "tone": "tone1"
        }
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "call: subscribeToTone",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
