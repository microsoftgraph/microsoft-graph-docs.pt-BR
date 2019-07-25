---
title: 'Range: clear'
description: Limpa valores de intervalo, formatação, preenchimento, borda, etc.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 910eaedd10f155a9189295158d0f1f2f630af9cd
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35857230"
---
# <a name="range-clear"></a><span data-ttu-id="6226c-103">Range: clear</span><span class="sxs-lookup"><span data-stu-id="6226c-103">Range: clear</span></span>

<span data-ttu-id="6226c-104">Limpa valores de intervalo, formatação, preenchimento, borda, etc.</span><span class="sxs-lookup"><span data-stu-id="6226c-104">Clear range values, format, fill, border, etc.</span></span>
## <a name="permissions"></a><span data-ttu-id="6226c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="6226c-105">Permissions</span></span>
<span data-ttu-id="6226c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6226c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6226c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6226c-108">Permission type</span></span>      | <span data-ttu-id="6226c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6226c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6226c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6226c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6226c-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6226c-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6226c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6226c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6226c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6226c-113">Not supported.</span></span>    |
|<span data-ttu-id="6226c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6226c-114">Application</span></span> | <span data-ttu-id="6226c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6226c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6226c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6226c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/clear
POST /workbook/worksheets/{id|name}/range(address='<address>')/clear
POST /workbook/tables/{id|name}/columns/{id|name}/range/clear

```
## <a name="request-headers"></a><span data-ttu-id="6226c-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6226c-117">Request headers</span></span>
| <span data-ttu-id="6226c-118">Nome</span><span class="sxs-lookup"><span data-stu-id="6226c-118">Name</span></span>       | <span data-ttu-id="6226c-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="6226c-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6226c-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="6226c-120">Authorization</span></span>  | <span data-ttu-id="6226c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6226c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6226c-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="6226c-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="6226c-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="6226c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6226c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6226c-126">Request body</span></span>
<span data-ttu-id="6226c-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6226c-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6226c-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="6226c-128">Parameter</span></span>    | <span data-ttu-id="6226c-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="6226c-129">Type</span></span>   |<span data-ttu-id="6226c-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="6226c-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6226c-131">applyTo</span><span class="sxs-lookup"><span data-stu-id="6226c-131">applyTo</span></span>|<span data-ttu-id="6226c-132">string</span><span class="sxs-lookup"><span data-stu-id="6226c-132">string</span></span>|<span data-ttu-id="6226c-133">Opcional.</span><span class="sxs-lookup"><span data-stu-id="6226c-133">Optional.</span></span> <span data-ttu-id="6226c-134">Determina o tipo de ação clara.</span><span class="sxs-lookup"><span data-stu-id="6226c-134">Determines the type of clear action.</span></span>  <span data-ttu-id="6226c-135">Os valores possíveis são: `All`, `Formats`, `Contents`.</span><span class="sxs-lookup"><span data-stu-id="6226c-135">The possible values are: `All`, `Formats`, `Contents`.</span></span>|

## <a name="response"></a><span data-ttu-id="6226c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="6226c-136">Response</span></span>

<span data-ttu-id="6226c-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6226c-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6226c-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6226c-139">Example</span></span>
<span data-ttu-id="6226c-140">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="6226c-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6226c-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6226c-141">Request</span></span>
<span data-ttu-id="6226c-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6226c-142">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6226c-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="6226c-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "range_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/clear
Content-type: application/json
Content-length: 32

{
  "applyTo": "applyTo-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6226c-144">C#</span><span class="sxs-lookup"><span data-stu-id="6226c-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-clear-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6226c-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="6226c-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-clear-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6226c-146">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="6226c-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-clear-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6226c-147">Java</span><span class="sxs-lookup"><span data-stu-id="6226c-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-clear-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6226c-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="6226c-148">Response</span></span>
<span data-ttu-id="6226c-149">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6226c-149">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
