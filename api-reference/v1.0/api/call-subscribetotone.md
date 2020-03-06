---
title: 'Call: subscribeToTone'
description: Assine o DTMF (sinalização de multifrequência de tom dual). Isso permite que você seja notificado quando o usuário pressionar teclas em um ' dialpad '.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 45b2145c002eb17a5bc65f946646ce70bf3872f8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518662"
---
# <a name="call-subscribetotone"></a><span data-ttu-id="4e05f-104">Call: subscribeToTone</span><span class="sxs-lookup"><span data-stu-id="4e05f-104">call: subscribeToTone</span></span>

<span data-ttu-id="4e05f-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e05f-105">Namespace: microsoft.graph</span></span>


<span data-ttu-id="4e05f-106">Assine o DTMF (sinalização de multifrequência de tom dual).</span><span class="sxs-lookup"><span data-stu-id="4e05f-106">Subscribe to DTMF (dual-tone multi-frequency signaling).</span></span> <span data-ttu-id="4e05f-107">Isso permite que você seja notificado quando o usuário pressionar teclas em um "dialpad".</span><span class="sxs-lookup"><span data-stu-id="4e05f-107">This allows you to be notified when the user presses keys on a "dialpad".</span></span>

> [!Note]
> <span data-ttu-id="4e05f-108">A ação **subscribeToTone** é suportada apenas para [chamadas](../resources/call.md) que são iniciadas com o [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span><span class="sxs-lookup"><span data-stu-id="4e05f-108">The **subscribeToTone** action is supported only for [calls](../resources/call.md) that are initiated with [serviceHostedMediaConfig](../resources/servicehostedmediaconfig.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4e05f-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="4e05f-109">Permissions</span></span>
<span data-ttu-id="4e05f-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e05f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4e05f-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4e05f-112">Permission type</span></span> | <span data-ttu-id="4e05f-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4e05f-113">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="4e05f-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4e05f-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="4e05f-115">Não suportado</span><span class="sxs-lookup"><span data-stu-id="4e05f-115">Not Supported</span></span>        |
| <span data-ttu-id="4e05f-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4e05f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e05f-117">Não suportado</span><span class="sxs-lookup"><span data-stu-id="4e05f-117">Not Supported</span></span>        |
| <span data-ttu-id="4e05f-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4e05f-118">Application</span></span>     | <span data-ttu-id="4e05f-119">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="4e05f-119">Calls.AccessMedia.All</span></span>                       |

><span data-ttu-id="4e05f-120">**Observação:** Qualquer dado de Tom fornecido pode não ser persistente.</span><span class="sxs-lookup"><span data-stu-id="4e05f-120">**Note:** Any tone data provided may not be persisted.</span></span> <span data-ttu-id="4e05f-121">Certifique-se de que você está em conformidade com as leis e regulamentos de sua área em relação à proteção de dados e à confidencialidade das comunicações.</span><span class="sxs-lookup"><span data-stu-id="4e05f-121">Make sure you are compliant with the laws and regulations of your area regarding data protection and confidentiality of communications.</span></span> <span data-ttu-id="4e05f-122">Confira os [Termos de Uso](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) e converse com sua assessoria jurídica para saber mais.</span><span class="sxs-lookup"><span data-stu-id="4e05f-122">Please see the [Terms of Use](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) and consult with your legal counsel for more information.</span></span>

## <a name="http-request"></a><span data-ttu-id="4e05f-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4e05f-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/subscribeToTone
```

## <a name="request-headers"></a><span data-ttu-id="4e05f-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4e05f-124">Request headers</span></span>
| <span data-ttu-id="4e05f-125">Nome</span><span class="sxs-lookup"><span data-stu-id="4e05f-125">Name</span></span>          | <span data-ttu-id="4e05f-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e05f-126">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="4e05f-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="4e05f-127">Authorization</span></span> | <span data-ttu-id="4e05f-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4e05f-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4e05f-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4e05f-130">Request body</span></span>
<span data-ttu-id="4e05f-131">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4e05f-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4e05f-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="4e05f-132">Parameter</span></span>      | <span data-ttu-id="4e05f-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="4e05f-133">Type</span></span>    | <span data-ttu-id="4e05f-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e05f-134">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="4e05f-135">clientContext</span><span class="sxs-lookup"><span data-stu-id="4e05f-135">clientContext</span></span>  | <span data-ttu-id="4e05f-136">String</span><span class="sxs-lookup"><span data-stu-id="4e05f-136">String</span></span>  | <span data-ttu-id="4e05f-137">Cadeia de caracteres de contexto de cliente exclusivo.</span><span class="sxs-lookup"><span data-stu-id="4e05f-137">Unique client context string.</span></span> <span data-ttu-id="4e05f-138">Pode ter um máximo de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="4e05f-138">Can have a maximum of 256 characters.</span></span> |

## <a name="response"></a><span data-ttu-id="4e05f-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e05f-139">Response</span></span>
<span data-ttu-id="4e05f-140">Se bem sucedido, este método retorna um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="4e05f-140">If successful, this method returns `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4e05f-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4e05f-141">Example</span></span>
<span data-ttu-id="4e05f-142">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="4e05f-142">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="4e05f-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4e05f-143">Request</span></span>
<span data-ttu-id="4e05f-144">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="4e05f-144">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4e05f-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="4e05f-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="4e05f-146">C#</span><span class="sxs-lookup"><span data-stu-id="4e05f-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-subscribetotone-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4e05f-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4e05f-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-subscribetotone-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4e05f-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4e05f-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-subscribetotone-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4e05f-149">Java</span><span class="sxs-lookup"><span data-stu-id="4e05f-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-subscribetotone-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4e05f-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e05f-150">Response</span></span>

> <span data-ttu-id="4e05f-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4e05f-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


##### <a name="notification---tone-notification"></a><span data-ttu-id="4e05f-153">Notificação de sinal de notificação</span><span class="sxs-lookup"><span data-stu-id="4e05f-153">Notification - tone notification</span></span>

<span data-ttu-id="4e05f-154">A notificação contém informações sobre o Tom pressionado no recurso [toneinfo](../resources/toneinfo.md) .</span><span class="sxs-lookup"><span data-stu-id="4e05f-154">The notification contain information of the tone pressed in the [toneinfo](../resources/toneinfo.md) resource.</span></span>

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
