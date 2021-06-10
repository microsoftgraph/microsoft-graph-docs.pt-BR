---
title: 'timeCard: endBreak'
description: Termine a quebra aberta em um cartão de ponto específico.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 61c80ea006ad0def4d9c8f58e36e44ae4caac851
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870574"
---
# <a name="timecard-endbreak"></a><span data-ttu-id="f60b0-103">timeCard: endBreak</span><span class="sxs-lookup"><span data-stu-id="f60b0-103">timeCard: endBreak</span></span>

<span data-ttu-id="f60b0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f60b0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f60b0-105">Termine a quebra aberta em um [cartão de ponto específico.](../resources/timeCard.md)</span><span class="sxs-lookup"><span data-stu-id="f60b0-105">End the open break in a specific [timeCard](../resources/timeCard.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f60b0-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="f60b0-106">Permissions</span></span>

<span data-ttu-id="f60b0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f60b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f60b0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f60b0-109">Permission type</span></span>      | <span data-ttu-id="f60b0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f60b0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f60b0-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f60b0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f60b0-112">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f60b0-112">Schedule.ReadWrite.All</span></span>    |
|<span data-ttu-id="f60b0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f60b0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f60b0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f60b0-114">Not supported.</span></span>    |
|<span data-ttu-id="f60b0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f60b0-115">Application</span></span> | <span data-ttu-id="f60b0-116">Schedule.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="f60b0-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="f60b0-117">\***Importante:** Quando você usa permissões de aplicativo, deve incluir `MS-APP-ACTS-AS` o header na solicitação.</span><span class="sxs-lookup"><span data-stu-id="f60b0-117">\* **Important:** When you use application permissions, you must include the `MS-APP-ACTS-AS` header in the request.</span></span>

## <a name="http-request"></a><span data-ttu-id="f60b0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f60b0-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timecards/{timeCardID}/endBreak
```

## <a name="request-headers"></a><span data-ttu-id="f60b0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f60b0-119">Request headers</span></span>

| <span data-ttu-id="f60b0-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f60b0-120">Header</span></span>       | <span data-ttu-id="f60b0-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f60b0-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f60b0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f60b0-122">Authorization</span></span>  | <span data-ttu-id="f60b0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f60b0-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f60b0-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="f60b0-125">Content-type</span></span> | <span data-ttu-id="f60b0-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f60b0-p103">application/json. Required.</span></span>|
| <span data-ttu-id="f60b0-128">MS-APP-ACTS-AS</span><span class="sxs-lookup"><span data-stu-id="f60b0-128">MS-APP-ACTS-AS</span></span> | <span data-ttu-id="f60b0-129">A ID do usuário em nome do qual o aplicativo está agindo.</span><span class="sxs-lookup"><span data-stu-id="f60b0-129">The ID of the user on behalf of whom the app is acting.</span></span> <span data-ttu-id="f60b0-130">Obrigatório ao usar o escopo de permissão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f60b0-130">Required when you use the application permission scope.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f60b0-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f60b0-131">Request body</span></span>

<span data-ttu-id="f60b0-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f60b0-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f60b0-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f60b0-133">Parameter</span></span>    | <span data-ttu-id="f60b0-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="f60b0-134">Type</span></span>        | <span data-ttu-id="f60b0-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="f60b0-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f60b0-136">atApprovedLocation</span><span class="sxs-lookup"><span data-stu-id="f60b0-136">atApprovedLocation</span></span>| `Edm.boolean ` | <span data-ttu-id="f60b0-137">Indique se essa ação acontece em um local aprovado.</span><span class="sxs-lookup"><span data-stu-id="f60b0-137">Indicate if this action happens at an approved location.</span></span>|
|<span data-ttu-id="f60b0-138">notes</span><span class="sxs-lookup"><span data-stu-id="f60b0-138">notes</span></span>| [<span data-ttu-id="f60b0-139">itemBody</span><span class="sxs-lookup"><span data-stu-id="f60b0-139">itemBody</span></span>](../resources/itembody.md)  |<span data-ttu-id="f60b0-140">Observações durante o término do intervalo.</span><span class="sxs-lookup"><span data-stu-id="f60b0-140">Notes during end of break.</span></span>|

## <a name="response"></a><span data-ttu-id="f60b0-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="f60b0-141">Response</span></span>

<span data-ttu-id="f60b0-142">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f60b0-142">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f60b0-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f60b0-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="f60b0-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f60b0-144">Request</span></span>
<span data-ttu-id="f60b0-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f60b0-145">The following is an example of the request.</span></span> 


# <a name="http"></a>[<span data-ttu-id="f60b0-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="f60b0-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timecard-endbreak"
}-->

```http
POST https://graph.microsoft.com/beta/teams/fd15cad8-80f6-484f-9666-3caf695fbf32/schedule/timeCards/TCK_cc09588d-d9d2-4fa0-85dc-2aa5ef983972/endbreak

{
    "atAprovedLocation": true,
    "notes": {
        "contentType": "text",
        "content": "end break smaple notes"
    }
}
```
# <a name="javascript"></a>[<span data-ttu-id="f60b0-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f60b0-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timecard-endbreak-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f60b0-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f60b0-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timecard-endbreak-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f60b0-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="f60b0-149">Response</span></span>

<span data-ttu-id="f60b0-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f60b0-150">The following is an example of the response.</span></span> 

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
  "description": "End Break",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
