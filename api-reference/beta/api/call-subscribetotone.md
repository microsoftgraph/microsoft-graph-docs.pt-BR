---
title: 'Call: subscribeToTone'
description: Assine o DTMF (sinalização de multifrequência de tom dual). Isso permite que você seja notificado quando o usuário pressionar teclas em um ' dialpad '.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: a81c6440d320f74411f1ffefb94a6fea14945b14
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/07/2019
ms.locfileid: "36792522"
---
# <a name="call-subscribetotone"></a><span data-ttu-id="ea92f-104">Call: subscribeToTone</span><span class="sxs-lookup"><span data-stu-id="ea92f-104">call: subscribeToTone</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ea92f-105">Assine o DTMF (sinalização de multifrequência de tom dual).</span><span class="sxs-lookup"><span data-stu-id="ea92f-105">Subscribe to DTMF (dual-tone multi-frequency signaling).</span></span> <span data-ttu-id="ea92f-106">Isso permite que você seja notificado quando o usuário pressionar teclas em um "dialpad".</span><span class="sxs-lookup"><span data-stu-id="ea92f-106">This allows you to be notified when the user presses keys on a "Dialpad".</span></span>

> [!Note]
> <span data-ttu-id="ea92f-107">A ação **subscribeToTone** é suportada apenas para [chamadas](../resources/call.md) que são iniciadas com o [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span><span class="sxs-lookup"><span data-stu-id="ea92f-107">The **subscribeToTone** action is supported only for [calls](../resources/call.md) that are initiated with [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ea92f-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="ea92f-108">Permissions</span></span>
<span data-ttu-id="ea92f-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea92f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ea92f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ea92f-111">Permission type</span></span> | <span data-ttu-id="ea92f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ea92f-112">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="ea92f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ea92f-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="ea92f-114">Não suportado</span><span class="sxs-lookup"><span data-stu-id="ea92f-114">Not Supported</span></span>        |
| <span data-ttu-id="ea92f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ea92f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea92f-116">Não suportado</span><span class="sxs-lookup"><span data-stu-id="ea92f-116">Not Supported</span></span>        |
| <span data-ttu-id="ea92f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ea92f-117">Application</span></span>     | <span data-ttu-id="ea92f-118">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="ea92f-118">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="ea92f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ea92f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/subscribeToTone
```

## <a name="request-headers"></a><span data-ttu-id="ea92f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ea92f-120">Request headers</span></span>
| <span data-ttu-id="ea92f-121">Nome</span><span class="sxs-lookup"><span data-stu-id="ea92f-121">Name</span></span>          | <span data-ttu-id="ea92f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea92f-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="ea92f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ea92f-123">Authorization</span></span> | <span data-ttu-id="ea92f-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ea92f-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ea92f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ea92f-126">Request body</span></span>
<span data-ttu-id="ea92f-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ea92f-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ea92f-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ea92f-128">Parameter</span></span>      | <span data-ttu-id="ea92f-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="ea92f-129">Type</span></span>    | <span data-ttu-id="ea92f-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea92f-130">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="ea92f-131">clientContext</span><span class="sxs-lookup"><span data-stu-id="ea92f-131">clientContext</span></span>  | <span data-ttu-id="ea92f-132">String</span><span class="sxs-lookup"><span data-stu-id="ea92f-132">String</span></span>  | <span data-ttu-id="ea92f-133">Cadeia de caracteres de contexto de cliente exclusivo.</span><span class="sxs-lookup"><span data-stu-id="ea92f-133">Unique client context string.</span></span> <span data-ttu-id="ea92f-134">Pode ter um máximo de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="ea92f-134">Can have a maximum of 256 characters.</span></span> |

## <a name="response"></a><span data-ttu-id="ea92f-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="ea92f-135">Response</span></span>
<span data-ttu-id="ea92f-136">Se bem sucedido, este método retorna um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="ea92f-136">If successful, this method returns `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ea92f-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ea92f-137">Example</span></span>
<span data-ttu-id="ea92f-138">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="ea92f-138">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="ea92f-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ea92f-139">Request</span></span>
<span data-ttu-id="ea92f-140">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="ea92f-140">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ea92f-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="ea92f-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-subscribeToTone"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/subscribeToTone
Content-Type: application/json
Content-Length: 46

{
  "clientContext": "fd1c7836-4d84-4e24-b6aa-23188688cc54"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ea92f-142">C#</span><span class="sxs-lookup"><span data-stu-id="ea92f-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-subscribetotone-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ea92f-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ea92f-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-subscribetotone-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ea92f-144">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="ea92f-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-subscribetotone-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ea92f-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="ea92f-145">Response</span></span>

> <span data-ttu-id="ea92f-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ea92f-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 200 OK

{
  "id": "ea91863c-d0a6-4de0-b73a-4c8d63da5d87",
  "status": "completed",
  "createdDateTime": "2019-07-18T19:52:30Z",
  "lastActionDateTime": "2019-07-18T19:52:31Z",
  "clientContext": "fd1c7836-4d84-4e24-b6aa-23188688cc54",
}
```


##### <a name="notification---tone-notification"></a><span data-ttu-id="ea92f-148">Notificação de sinal de notificação</span><span class="sxs-lookup"><span data-stu-id="ea92f-148">Notification - Tone notification</span></span>

<span data-ttu-id="ea92f-149">A notificação contém informações sobre o Tom pressionado no recurso [toneinfo](../resources/toneinfo.md) .</span><span class="sxs-lookup"><span data-stu-id="ea92f-149">The notification contain information of the tone pressed in the [toneinfo](../resources/toneinfo.md) resource.</span></span>

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [
    {
      "changeType": "updated",
      "resource": "/app/calls/421f1100-411f-4a29-8514-dbbb9caff45",
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
