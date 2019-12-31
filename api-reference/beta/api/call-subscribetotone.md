---
title: 'Call: subscribeToTone'
description: Assine o DTMF (sinalização de multifrequência de tom dual). Isso permite que você seja notificado quando o usuário pressionar teclas em um ' dialpad '.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 4aade47d641cbeb129b199858956f144e2d4bd0d
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40912745"
---
# <a name="call-subscribetotone"></a><span data-ttu-id="dc959-104">Call: subscribeToTone</span><span class="sxs-lookup"><span data-stu-id="dc959-104">call: subscribeToTone</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc959-105">Assine o DTMF (sinalização de multifrequência de tom dual).</span><span class="sxs-lookup"><span data-stu-id="dc959-105">Subscribe to DTMF (dual-tone multi-frequency signaling).</span></span> <span data-ttu-id="dc959-106">Isso permite que você seja notificado quando o usuário pressionar teclas em um "dialpad".</span><span class="sxs-lookup"><span data-stu-id="dc959-106">This allows you to be notified when the user presses keys on a "Dialpad".</span></span>

> [!Note]
> <span data-ttu-id="dc959-107">A ação **subscribeToTone** é suportada apenas para [chamadas](../resources/call.md) que são iniciadas com o [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span><span class="sxs-lookup"><span data-stu-id="dc959-107">The **subscribeToTone** action is supported only for [calls](../resources/call.md) that are initiated with [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="dc959-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="dc959-108">Permissions</span></span>
<span data-ttu-id="dc959-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc959-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dc959-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dc959-111">Permission type</span></span> | <span data-ttu-id="dc959-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dc959-112">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="dc959-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dc959-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="dc959-114">Não suportado</span><span class="sxs-lookup"><span data-stu-id="dc959-114">Not Supported</span></span>        |
| <span data-ttu-id="dc959-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dc959-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc959-116">Não suportado</span><span class="sxs-lookup"><span data-stu-id="dc959-116">Not Supported</span></span>        |
| <span data-ttu-id="dc959-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dc959-117">Application</span></span>     | <span data-ttu-id="dc959-118">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="dc959-118">Calls.AccessMedia.All</span></span>                       |

><span data-ttu-id="dc959-119">**Observação:** Qualquer dado de Tom fornecido pode não ser persistente.</span><span class="sxs-lookup"><span data-stu-id="dc959-119">**Note:** Any tone data provided may not be persisted.</span></span> <span data-ttu-id="dc959-120">Certifique-se de que você está em conformidade com as leis e regulamentos de sua área em relação à proteção de dados e à confidencialidade das comunicações.</span><span class="sxs-lookup"><span data-stu-id="dc959-120">Make sure you are compliant with the laws and regulations of your area regarding data protection and confidentiality of communications.</span></span> <span data-ttu-id="dc959-121">Confira os [Termos de Uso](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) e converse com sua assessoria jurídica para saber mais.</span><span class="sxs-lookup"><span data-stu-id="dc959-121">Please see the [Terms of Use](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) and consult with your legal counsel for more information.</span></span>
## <a name="http-request"></a><span data-ttu-id="dc959-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dc959-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/subscribeToTone
POST /communications/calls/{id}/subscribeToTone
```
> <span data-ttu-id="dc959-123">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="dc959-123">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="dc959-124">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="dc959-124">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dc959-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dc959-125">Request headers</span></span>
| <span data-ttu-id="dc959-126">Nome</span><span class="sxs-lookup"><span data-stu-id="dc959-126">Name</span></span>          | <span data-ttu-id="dc959-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc959-127">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="dc959-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="dc959-128">Authorization</span></span> | <span data-ttu-id="dc959-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dc959-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dc959-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dc959-131">Request body</span></span>
<span data-ttu-id="dc959-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dc959-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="dc959-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="dc959-133">Parameter</span></span>      | <span data-ttu-id="dc959-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="dc959-134">Type</span></span>    | <span data-ttu-id="dc959-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc959-135">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="dc959-136">clientContext</span><span class="sxs-lookup"><span data-stu-id="dc959-136">clientContext</span></span>  | <span data-ttu-id="dc959-137">String</span><span class="sxs-lookup"><span data-stu-id="dc959-137">String</span></span>  | <span data-ttu-id="dc959-138">Cadeia de caracteres de contexto de cliente exclusivo.</span><span class="sxs-lookup"><span data-stu-id="dc959-138">Unique client context string.</span></span> <span data-ttu-id="dc959-139">Pode ter um máximo de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="dc959-139">Can have a maximum of 256 characters.</span></span> |

## <a name="response"></a><span data-ttu-id="dc959-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc959-140">Response</span></span>
<span data-ttu-id="dc959-141">Se bem sucedido, este método retorna um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="dc959-141">If successful, this method returns `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="dc959-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dc959-142">Example</span></span>
<span data-ttu-id="dc959-143">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="dc959-143">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="dc959-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dc959-144">Request</span></span>
<span data-ttu-id="dc959-145">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="dc959-145">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="dc959-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="dc959-146">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="dc959-147">C#</span><span class="sxs-lookup"><span data-stu-id="dc959-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-subscribetotone-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dc959-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dc959-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-subscribetotone-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dc959-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dc959-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-subscribetotone-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="dc959-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc959-150">Response</span></span>

> <span data-ttu-id="dc959-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dc959-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


##### <a name="notification---tone-notification"></a><span data-ttu-id="dc959-153">Notificação de sinal de notificação</span><span class="sxs-lookup"><span data-stu-id="dc959-153">Notification - tone notification</span></span>

<span data-ttu-id="dc959-154">A notificação contém informações sobre o Tom pressionado no recurso [toneinfo](../resources/toneinfo.md) .</span><span class="sxs-lookup"><span data-stu-id="dc959-154">The notification contain information of the tone pressed in the [toneinfo](../resources/toneinfo.md) resource.</span></span>

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
