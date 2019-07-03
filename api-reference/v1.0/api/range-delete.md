---
title: 'Range: delete'
description: Exclui as células associadas ao intervalo.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 4c06121d63d45fa4e07e15b2525e7308331cef54
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35449040"
---
# <a name="range-delete"></a><span data-ttu-id="067fc-103">Range: delete</span><span class="sxs-lookup"><span data-stu-id="067fc-103">Range: delete</span></span>

<span data-ttu-id="067fc-104">Exclui as células associadas ao intervalo.</span><span class="sxs-lookup"><span data-stu-id="067fc-104">Deletes the cells associated with the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="067fc-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="067fc-105">Permissions</span></span>
<span data-ttu-id="067fc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="067fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="067fc-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="067fc-108">Permission type</span></span>      | <span data-ttu-id="067fc-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="067fc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="067fc-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="067fc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="067fc-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="067fc-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="067fc-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="067fc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="067fc-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="067fc-113">Not supported.</span></span>    |
|<span data-ttu-id="067fc-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="067fc-114">Application</span></span> | <span data-ttu-id="067fc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="067fc-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="067fc-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="067fc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/delete
POST /workbook/worksheets/{id|name}/range(address='<address>')/delete
POST /workbook/tables/{id|name}/columns/{id|name}/range/delete

```
## <a name="request-headers"></a><span data-ttu-id="067fc-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="067fc-117">Request headers</span></span>
| <span data-ttu-id="067fc-118">Nome</span><span class="sxs-lookup"><span data-stu-id="067fc-118">Name</span></span>       | <span data-ttu-id="067fc-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="067fc-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="067fc-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="067fc-120">Authorization</span></span>  | <span data-ttu-id="067fc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="067fc-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="067fc-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="067fc-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="067fc-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="067fc-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="067fc-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="067fc-126">Request body</span></span>
<span data-ttu-id="067fc-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="067fc-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="067fc-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="067fc-128">Parameter</span></span>    | <span data-ttu-id="067fc-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="067fc-129">Type</span></span>   |<span data-ttu-id="067fc-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="067fc-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="067fc-131">shift</span><span class="sxs-lookup"><span data-stu-id="067fc-131">shift</span></span>|<span data-ttu-id="067fc-132">string</span><span class="sxs-lookup"><span data-stu-id="067fc-132">string</span></span>|<span data-ttu-id="067fc-133">Especifica como deslocar as células.</span><span class="sxs-lookup"><span data-stu-id="067fc-133">Specifies which way to shift the cells.</span></span>  <span data-ttu-id="067fc-134">Os valores possíveis são: `Up`, `Left`.</span><span class="sxs-lookup"><span data-stu-id="067fc-134">The possible values are: `Up`, `Left`.</span></span>|

## <a name="response"></a><span data-ttu-id="067fc-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="067fc-135">Response</span></span>

<span data-ttu-id="067fc-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="067fc-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="067fc-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="067fc-138">Example</span></span>
<span data-ttu-id="067fc-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="067fc-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="067fc-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="067fc-140">Request</span></span>
<span data-ttu-id="067fc-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="067fc-141">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="067fc-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="067fc-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "range_delete"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/delete
Content-type: application/json
Content-length: 28

{
  "shift": "shift-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="067fc-143">C#</span><span class="sxs-lookup"><span data-stu-id="067fc-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="067fc-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="067fc-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="067fc-145">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="067fc-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="067fc-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="067fc-146">Response</span></span>
<span data-ttu-id="067fc-147">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="067fc-147">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
