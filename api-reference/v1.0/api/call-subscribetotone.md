---
title: 'call: subscribeToTone'
description: Inscreva-se em DTMF (sinalização multifrequência de tom duplo). Isso permite que você seja notificado quando o usuário pressionar teclas em um "Dialpad".
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: bca2ba67be2f62f87c84390a5a1bc3a2799e9498
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051596"
---
# <a name="call-subscribetotone"></a><span data-ttu-id="4dbfd-104">call: subscribeToTone</span><span class="sxs-lookup"><span data-stu-id="4dbfd-104">call: subscribeToTone</span></span>

<span data-ttu-id="4dbfd-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4dbfd-105">Namespace: microsoft.graph</span></span>


<span data-ttu-id="4dbfd-106">Inscreva-se em DTMF (sinalização multifrequência de tom duplo).</span><span class="sxs-lookup"><span data-stu-id="4dbfd-106">Subscribe to DTMF (dual-tone multi-frequency signaling).</span></span> <span data-ttu-id="4dbfd-107">Isso permite que você seja notificado quando o usuário pressionar teclas em um "dialpad".</span><span class="sxs-lookup"><span data-stu-id="4dbfd-107">This allows you to be notified when the user presses keys on a "dialpad".</span></span>

> [!Note]
> <span data-ttu-id="4dbfd-108">A **ação subscribeToTone** só tem suporte para [chamadas](../resources/call.md) iniciadas com [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span><span class="sxs-lookup"><span data-stu-id="4dbfd-108">The **subscribeToTone** action is supported only for [calls](../resources/call.md) that are initiated with [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4dbfd-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="4dbfd-109">Permissions</span></span>
<span data-ttu-id="4dbfd-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4dbfd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4dbfd-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4dbfd-112">Permission type</span></span> | <span data-ttu-id="4dbfd-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4dbfd-113">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="4dbfd-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4dbfd-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="4dbfd-115">Não suportado</span><span class="sxs-lookup"><span data-stu-id="4dbfd-115">Not Supported</span></span>        |
| <span data-ttu-id="4dbfd-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4dbfd-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4dbfd-117">Não suportado</span><span class="sxs-lookup"><span data-stu-id="4dbfd-117">Not Supported</span></span>        |
| <span data-ttu-id="4dbfd-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4dbfd-118">Application</span></span>     | <span data-ttu-id="4dbfd-119">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="4dbfd-119">Calls.AccessMedia.All</span></span>                       |

><span data-ttu-id="4dbfd-120">**Observação:** Os dados de tom fornecidos podem não ser persistentes.</span><span class="sxs-lookup"><span data-stu-id="4dbfd-120">**Note:** Any tone data provided may not be persisted.</span></span> <span data-ttu-id="4dbfd-121">Certifique-se de estar em conformidade com as leis e regulamentos de sua área em relação à proteção de dados e à confidencialidade das comunicações.</span><span class="sxs-lookup"><span data-stu-id="4dbfd-121">Make sure you are compliant with the laws and regulations of your area regarding data protection and confidentiality of communications.</span></span> <span data-ttu-id="4dbfd-122">Confira os [Termos de Uso](/legal/microsoft-apis/terms-of-use) e converse com sua assessoria jurídica para saber mais.</span><span class="sxs-lookup"><span data-stu-id="4dbfd-122">Please see the [Terms of Use](/legal/microsoft-apis/terms-of-use) and consult with your legal counsel for more information.</span></span>

## <a name="http-request"></a><span data-ttu-id="4dbfd-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4dbfd-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/subscribeToTone
```

## <a name="request-headers"></a><span data-ttu-id="4dbfd-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4dbfd-124">Request headers</span></span>
| <span data-ttu-id="4dbfd-125">Nome</span><span class="sxs-lookup"><span data-stu-id="4dbfd-125">Name</span></span>          | <span data-ttu-id="4dbfd-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="4dbfd-126">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="4dbfd-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="4dbfd-127">Authorization</span></span> | <span data-ttu-id="4dbfd-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4dbfd-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4dbfd-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4dbfd-130">Request body</span></span>
<span data-ttu-id="4dbfd-131">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4dbfd-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4dbfd-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="4dbfd-132">Parameter</span></span>      | <span data-ttu-id="4dbfd-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="4dbfd-133">Type</span></span>    | <span data-ttu-id="4dbfd-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="4dbfd-134">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="4dbfd-135">clientContext</span><span class="sxs-lookup"><span data-stu-id="4dbfd-135">clientContext</span></span>  | <span data-ttu-id="4dbfd-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4dbfd-136">String</span></span>  | <span data-ttu-id="4dbfd-137">Cadeia de caracteres de contexto de cliente exclusiva.</span><span class="sxs-lookup"><span data-stu-id="4dbfd-137">Unique client context string.</span></span> <span data-ttu-id="4dbfd-138">Pode ter no máximo 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="4dbfd-138">Can have a maximum of 256 characters.</span></span> |

## <a name="response"></a><span data-ttu-id="4dbfd-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="4dbfd-139">Response</span></span>
<span data-ttu-id="4dbfd-140">Se bem sucedido, este método retorna um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="4dbfd-140">If successful, this method returns `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4dbfd-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4dbfd-141">Example</span></span>
<span data-ttu-id="4dbfd-142">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="4dbfd-142">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="4dbfd-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4dbfd-143">Request</span></span>
<span data-ttu-id="4dbfd-144">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="4dbfd-144">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4dbfd-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="4dbfd-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-subscribeToTone"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls/{id}/subscribeToTone
Content-Type: application/json
Content-Length: 46

{
  "clientContext": "fd1c7836-4d84-4e24-b6aa-23188688cc54"
}
```
# <a name="c"></a>[<span data-ttu-id="4dbfd-146">C#</span><span class="sxs-lookup"><span data-stu-id="4dbfd-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-subscribetotone-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4dbfd-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4dbfd-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-subscribetotone-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4dbfd-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4dbfd-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-subscribetotone-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4dbfd-149">Java</span><span class="sxs-lookup"><span data-stu-id="4dbfd-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-subscribetotone-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4dbfd-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="4dbfd-150">Response</span></span>

> <span data-ttu-id="4dbfd-151">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4dbfd-151">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "name": "call-subscribeToTone",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscribeToToneOperation"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Location: https://graph.microsoft.com/v1.0/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5

{
  "@odata.type": "#microsoft.graph.subscribeToToneOperation",
  "clientContext": "clientContext-value",
  "id": "0fe0623f-d628-42ed-b4bd-8ac290072cc5",
  "status": "completed"
}
```


##### <a name="notification---tone-notification"></a><span data-ttu-id="4dbfd-152">Notificação - notificação de tom</span><span class="sxs-lookup"><span data-stu-id="4dbfd-152">Notification - tone notification</span></span>

<span data-ttu-id="4dbfd-153">A notificação contém informações do tom pressionado no [recurso toneinfo.](../resources/toneinfo.md)</span><span class="sxs-lookup"><span data-stu-id="4dbfd-153">The notification contain information of the tone pressed in the [toneinfo](../resources/toneinfo.md) resource.</span></span>

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
