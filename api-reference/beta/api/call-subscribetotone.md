---
title: 'Call: subscribeToTone'
description: Assine o DTMF (sinalização de multifrequência de tom dual). Isso permite que você seja notificado quando o usuário pressionar teclas em um ' dialpad '.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: aea175602f363477103fba7b6fad785ce4f22c5f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47987292"
---
# <a name="call-subscribetotone"></a><span data-ttu-id="dddc6-104">Call: subscribeToTone</span><span class="sxs-lookup"><span data-stu-id="dddc6-104">call: subscribeToTone</span></span>

<span data-ttu-id="dddc6-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dddc6-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dddc6-106">Assine o DTMF (sinalização de multifrequência de tom dual).</span><span class="sxs-lookup"><span data-stu-id="dddc6-106">Subscribe to DTMF (dual-tone multi-frequency signaling).</span></span> <span data-ttu-id="dddc6-107">Isso permite que você seja notificado quando o usuário pressionar teclas em um "dialpad".</span><span class="sxs-lookup"><span data-stu-id="dddc6-107">This allows you to be notified when the user presses keys on a "Dialpad".</span></span>

> [!Note]
> <span data-ttu-id="dddc6-108">A ação **subscribeToTone** é suportada apenas para [chamadas](../resources/call.md) que são iniciadas com o [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span><span class="sxs-lookup"><span data-stu-id="dddc6-108">The **subscribeToTone** action is supported only for [calls](../resources/call.md) that are initiated with [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="dddc6-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="dddc6-109">Permissions</span></span>
<span data-ttu-id="dddc6-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dddc6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dddc6-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dddc6-112">Permission type</span></span> | <span data-ttu-id="dddc6-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dddc6-113">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="dddc6-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dddc6-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="dddc6-115">Não suportado</span><span class="sxs-lookup"><span data-stu-id="dddc6-115">Not Supported</span></span>        |
| <span data-ttu-id="dddc6-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dddc6-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dddc6-117">Não suportado</span><span class="sxs-lookup"><span data-stu-id="dddc6-117">Not Supported</span></span>        |
| <span data-ttu-id="dddc6-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dddc6-118">Application</span></span>     | <span data-ttu-id="dddc6-119">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="dddc6-119">Calls.AccessMedia.All</span></span>                       |

><span data-ttu-id="dddc6-120">**Observação:** Qualquer dado de Tom fornecido pode não ser persistente.</span><span class="sxs-lookup"><span data-stu-id="dddc6-120">**Note:** Any tone data provided may not be persisted.</span></span> <span data-ttu-id="dddc6-121">Certifique-se de que você está em conformidade com as leis e regulamentos de sua área em relação à proteção de dados e à confidencialidade das comunicações.</span><span class="sxs-lookup"><span data-stu-id="dddc6-121">Make sure you are compliant with the laws and regulations of your area regarding data protection and confidentiality of communications.</span></span> <span data-ttu-id="dddc6-122">Confira os [Termos de Uso](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) e converse com sua assessoria jurídica para saber mais.</span><span class="sxs-lookup"><span data-stu-id="dddc6-122">Please see the [Terms of Use](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) and consult with your legal counsel for more information.</span></span>
## <a name="http-request"></a><span data-ttu-id="dddc6-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dddc6-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/subscribeToTone
POST /communications/calls/{id}/subscribeToTone
```
> <span data-ttu-id="dddc6-124">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="dddc6-124">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="dddc6-125">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="dddc6-125">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dddc6-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dddc6-126">Request headers</span></span>
| <span data-ttu-id="dddc6-127">Nome</span><span class="sxs-lookup"><span data-stu-id="dddc6-127">Name</span></span>          | <span data-ttu-id="dddc6-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="dddc6-128">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="dddc6-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="dddc6-129">Authorization</span></span> | <span data-ttu-id="dddc6-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dddc6-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dddc6-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dddc6-132">Request body</span></span>
<span data-ttu-id="dddc6-133">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dddc6-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="dddc6-134">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="dddc6-134">Parameter</span></span>      | <span data-ttu-id="dddc6-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="dddc6-135">Type</span></span>    | <span data-ttu-id="dddc6-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="dddc6-136">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="dddc6-137">clientContext</span><span class="sxs-lookup"><span data-stu-id="dddc6-137">clientContext</span></span>  | <span data-ttu-id="dddc6-138">String</span><span class="sxs-lookup"><span data-stu-id="dddc6-138">String</span></span>  | <span data-ttu-id="dddc6-139">Cadeia de caracteres de contexto de cliente exclusivo.</span><span class="sxs-lookup"><span data-stu-id="dddc6-139">Unique client context string.</span></span> <span data-ttu-id="dddc6-140">Pode ter um máximo de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="dddc6-140">Can have a maximum of 256 characters.</span></span> |

## <a name="response"></a><span data-ttu-id="dddc6-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="dddc6-141">Response</span></span>
<span data-ttu-id="dddc6-142">Se bem sucedido, este método retorna um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="dddc6-142">If successful, this method returns `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="dddc6-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dddc6-143">Example</span></span>
<span data-ttu-id="dddc6-144">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="dddc6-144">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="dddc6-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dddc6-145">Request</span></span>
<span data-ttu-id="dddc6-146">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="dddc6-146">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="dddc6-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="dddc6-147">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="dddc6-148">C#</span><span class="sxs-lookup"><span data-stu-id="dddc6-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-subscribetotone-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dddc6-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dddc6-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-subscribetotone-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dddc6-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dddc6-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-subscribetotone-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="dddc6-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="dddc6-151">Response</span></span>

> <span data-ttu-id="dddc6-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dddc6-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "call-subscribeToTone",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscribeToToneOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5

{
  "@odata.type": "#microsoft.graph.subscribeToToneOperation",
  "clientContext": "clientContext-value",
  "id": "0fe0623f-d628-42ed-b4bd-8ac290072cc5",
  "resultInfo": null,
  "status": "completed"
}
```


##### <a name="notification---tone-notification"></a><span data-ttu-id="dddc6-154">Notificação de sinal de notificação</span><span class="sxs-lookup"><span data-stu-id="dddc6-154">Notification - tone notification</span></span>

<span data-ttu-id="dddc6-155">A notificação contém informações sobre o Tom pressionado no recurso [toneinfo](../resources/toneinfo.md) .</span><span class="sxs-lookup"><span data-stu-id="dddc6-155">The notification contain information of the tone pressed in the [toneinfo](../resources/toneinfo.md) resource.</span></span>

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
      "resourceUrl": "/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896",
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


