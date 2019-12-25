---
title: 'Call: subscribeToTone'
description: Assine o DTMF (sinalização de multifrequência de tom dual). Isso permite que você seja notificado quando o usuário pressionar teclas em um ' dialpad '.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 67f77d3413b53d2f26bb60be934a188239bd8234
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871018"
---
# <a name="call-subscribetotone"></a><span data-ttu-id="354cd-104">Call: subscribeToTone</span><span class="sxs-lookup"><span data-stu-id="354cd-104">call: subscribeToTone</span></span>


<span data-ttu-id="354cd-105">Assine o DTMF (sinalização de multifrequência de tom dual).</span><span class="sxs-lookup"><span data-stu-id="354cd-105">Subscribe to DTMF (dual-tone multi-frequency signaling).</span></span> <span data-ttu-id="354cd-106">Isso permite que você seja notificado quando o usuário pressionar teclas em um "dialpad".</span><span class="sxs-lookup"><span data-stu-id="354cd-106">This allows you to be notified when the user presses keys on a "dialpad".</span></span>

> [!Note]
> <span data-ttu-id="354cd-107">A ação **subscribeToTone** é suportada apenas para [chamadas](../resources/call.md) que são iniciadas com o [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span><span class="sxs-lookup"><span data-stu-id="354cd-107">The **subscribeToTone** action is supported only for [calls](../resources/call.md) that are initiated with [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="354cd-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="354cd-108">Permissions</span></span>
<span data-ttu-id="354cd-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="354cd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="354cd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="354cd-111">Permission type</span></span> | <span data-ttu-id="354cd-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="354cd-112">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="354cd-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="354cd-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="354cd-114">Não suportado</span><span class="sxs-lookup"><span data-stu-id="354cd-114">Not Supported</span></span>        |
| <span data-ttu-id="354cd-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="354cd-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="354cd-116">Não suportado</span><span class="sxs-lookup"><span data-stu-id="354cd-116">Not Supported</span></span>        |
| <span data-ttu-id="354cd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="354cd-117">Application</span></span>     | <span data-ttu-id="354cd-118">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="354cd-118">Calls.AccessMedia.All</span></span>                       |

><span data-ttu-id="354cd-119">**Observação:** Qualquer dado de Tom fornecido pode não ser persistente.</span><span class="sxs-lookup"><span data-stu-id="354cd-119">**Note:** Any tone data provided may not be persisted.</span></span> <span data-ttu-id="354cd-120">Certifique-se de que você está em conformidade com as leis e regulamentos de sua área em relação à proteção de dados e à confidencialidade das comunicações.</span><span class="sxs-lookup"><span data-stu-id="354cd-120">Make sure you are compliant with the laws and regulations of your area regarding data protection and confidentiality of communications.</span></span> <span data-ttu-id="354cd-121">Confira os [Termos de Uso](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) e converse com sua assessoria jurídica para saber mais.</span><span class="sxs-lookup"><span data-stu-id="354cd-121">Please see the [Terms of Use](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) and consult with your legal counsel for more information.</span></span>

## <a name="http-request"></a><span data-ttu-id="354cd-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="354cd-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/subscribeToTone
```

## <a name="request-headers"></a><span data-ttu-id="354cd-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="354cd-123">Request headers</span></span>
| <span data-ttu-id="354cd-124">Nome</span><span class="sxs-lookup"><span data-stu-id="354cd-124">Name</span></span>          | <span data-ttu-id="354cd-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="354cd-125">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="354cd-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="354cd-126">Authorization</span></span> | <span data-ttu-id="354cd-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="354cd-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="354cd-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="354cd-129">Request body</span></span>
<span data-ttu-id="354cd-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="354cd-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="354cd-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="354cd-131">Parameter</span></span>      | <span data-ttu-id="354cd-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="354cd-132">Type</span></span>    | <span data-ttu-id="354cd-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="354cd-133">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="354cd-134">clientContext</span><span class="sxs-lookup"><span data-stu-id="354cd-134">clientContext</span></span>  | <span data-ttu-id="354cd-135">String</span><span class="sxs-lookup"><span data-stu-id="354cd-135">String</span></span>  | <span data-ttu-id="354cd-136">Cadeia de caracteres de contexto de cliente exclusivo.</span><span class="sxs-lookup"><span data-stu-id="354cd-136">Unique client context string.</span></span> <span data-ttu-id="354cd-137">Pode ter um máximo de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="354cd-137">Can have a maximum of 256 characters.</span></span> |

## <a name="response"></a><span data-ttu-id="354cd-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="354cd-138">Response</span></span>
<span data-ttu-id="354cd-139">Se bem sucedido, este método retorna um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="354cd-139">If successful, this method returns `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="354cd-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="354cd-140">Example</span></span>
<span data-ttu-id="354cd-141">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="354cd-141">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="354cd-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="354cd-142">Request</span></span>
<span data-ttu-id="354cd-143">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="354cd-143">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="354cd-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="354cd-144">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="354cd-145">C#</span><span class="sxs-lookup"><span data-stu-id="354cd-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-subscribetotone-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="354cd-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="354cd-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-subscribetotone-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="354cd-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="354cd-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-subscribetotone-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="354cd-148">Java</span><span class="sxs-lookup"><span data-stu-id="354cd-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-subscribetotone-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="354cd-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="354cd-149">Response</span></span>

> <span data-ttu-id="354cd-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="354cd-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


##### <a name="notification---tone-notification"></a><span data-ttu-id="354cd-152">Notificação de sinal de notificação</span><span class="sxs-lookup"><span data-stu-id="354cd-152">Notification - tone notification</span></span>

<span data-ttu-id="354cd-153">A notificação contém informações sobre o Tom pressionado no recurso [toneinfo](../resources/toneinfo.md) .</span><span class="sxs-lookup"><span data-stu-id="354cd-153">The notification contain information of the tone pressed in the [toneinfo](../resources/toneinfo.md) resource.</span></span>

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
