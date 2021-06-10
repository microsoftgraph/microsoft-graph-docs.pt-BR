---
title: 'timeCard: clockOut'
description: Clock Out para finalizar um cartão de ponto aberto.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f6f3f054bff67a1c9eea966fac8c03c44c00dc8f
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869818"
---
# <a name="timecard-clockout"></a><span data-ttu-id="1e471-103">timeCard: clockOut</span><span class="sxs-lookup"><span data-stu-id="1e471-103">timeCard: clockOut</span></span>

<span data-ttu-id="1e471-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e471-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e471-105">Clock out to end a open [timeCard](../resources/timeCard.md).</span><span class="sxs-lookup"><span data-stu-id="1e471-105">Clock out to end an open [timeCard](../resources/timeCard.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1e471-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="1e471-106">Permissions</span></span>

<span data-ttu-id="1e471-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e471-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e471-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1e471-109">Permission type</span></span>      | <span data-ttu-id="1e471-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1e471-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1e471-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1e471-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1e471-112">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e471-112">Schedule.ReadWrite.All</span></span>    |
|<span data-ttu-id="1e471-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1e471-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e471-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e471-114">Not supported.</span></span>    |
|<span data-ttu-id="1e471-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1e471-115">Application</span></span> | <span data-ttu-id="1e471-116">Schedule.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="1e471-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="1e471-117">\***Importante:** Quando você usa permissões de aplicativo, deve incluir `MS-APP-ACTS-AS` o header na solicitação.</span><span class="sxs-lookup"><span data-stu-id="1e471-117">\* **Important:** When you use application permissions, you must include the `MS-APP-ACTS-AS` header in the request.</span></span>

## <a name="http-request"></a><span data-ttu-id="1e471-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1e471-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timecards/{timeCardID}/clockOut
```

## <a name="request-headers"></a><span data-ttu-id="1e471-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1e471-119">Request headers</span></span>

| <span data-ttu-id="1e471-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1e471-120">Header</span></span>       | <span data-ttu-id="1e471-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1e471-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1e471-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1e471-122">Authorization</span></span>  | <span data-ttu-id="1e471-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1e471-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1e471-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="1e471-125">Content-type</span></span> | <span data-ttu-id="1e471-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1e471-p103">application/json. Required.</span></span>|
| <span data-ttu-id="1e471-128">MS-APP-ACTS-AS</span><span class="sxs-lookup"><span data-stu-id="1e471-128">MS-APP-ACTS-AS</span></span> | <span data-ttu-id="1e471-129">A ID do usuário em nome do qual o aplicativo está agindo.</span><span class="sxs-lookup"><span data-stu-id="1e471-129">The ID of the user on behalf of whom the app is acting.</span></span> <span data-ttu-id="1e471-130">Obrigatório ao usar o escopo de permissão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1e471-130">Required when you use the application permission scope.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1e471-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1e471-131">Request body</span></span>

<span data-ttu-id="1e471-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1e471-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1e471-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="1e471-133">Parameter</span></span>    | <span data-ttu-id="1e471-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="1e471-134">Type</span></span>        | <span data-ttu-id="1e471-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e471-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1e471-136">atApprovedLocation</span><span class="sxs-lookup"><span data-stu-id="1e471-136">atApprovedLocation</span></span>| `Edm.boolean ` | <span data-ttu-id="1e471-137">Indique se essa ação acontece em um local aprovado.</span><span class="sxs-lookup"><span data-stu-id="1e471-137">Indicate if this action happens at an approved location.</span></span>|
|<span data-ttu-id="1e471-138">notes</span><span class="sxs-lookup"><span data-stu-id="1e471-138">notes</span></span>| [<span data-ttu-id="1e471-139">itemBody</span><span class="sxs-lookup"><span data-stu-id="1e471-139">itemBody</span></span>](../resources/itembody.md)  |<span data-ttu-id="1e471-140">Observações para o tempo de saída.</span><span class="sxs-lookup"><span data-stu-id="1e471-140">Notes for the clock out.</span></span> |

## <a name="response"></a><span data-ttu-id="1e471-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e471-141">Response</span></span>

<span data-ttu-id="1e471-142">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1e471-142">If successful, this method returns a `204 No Content` response code.</span></span>


## <a name="example"></a><span data-ttu-id="1e471-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1e471-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="1e471-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1e471-144">Request</span></span>
<span data-ttu-id="1e471-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1e471-145">The following is an example of the request.</span></span> 


# <a name="http"></a>[<span data-ttu-id="1e471-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="1e471-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timecard-clockout"
}-->

```http
POST https://graph.microsoft.com/beta/teams/fd15cad8-80f6-484f-9666-3caf695fbf32/schedule/timeCards/TCK_cc09588d-d9d2-4fa0-85dc-2aa5ef983972/clockout
Content-type: application/json

{
    "atAprovedLocation": true,
    "notes": {
        "contentType": "text",
        "content": "clock out smaple notes"
    }
}
```
# <a name="javascript"></a>[<span data-ttu-id="1e471-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1e471-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timecard-clockout-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1e471-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1e471-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timecard-clockout-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1e471-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e471-149">Response</span></span>

<span data-ttu-id="1e471-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1e471-150">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Clock Out",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
