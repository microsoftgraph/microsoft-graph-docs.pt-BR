---
title: 'Range: delete'
description: Exclui as células associadas ao intervalo.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 82bf226d76a0db2f90d91284095a11419f62b0b0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47978738"
---
# <a name="range-delete"></a><span data-ttu-id="74895-103">Range: delete</span><span class="sxs-lookup"><span data-stu-id="74895-103">Range: delete</span></span>

<span data-ttu-id="74895-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74895-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="74895-105">Exclui as células associadas ao intervalo.</span><span class="sxs-lookup"><span data-stu-id="74895-105">Deletes the cells associated with the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="74895-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="74895-106">Permissions</span></span>
<span data-ttu-id="74895-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74895-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74895-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="74895-109">Permission type</span></span>      | <span data-ttu-id="74895-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="74895-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="74895-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="74895-111">Delegated (work or school account)</span></span> | <span data-ttu-id="74895-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="74895-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="74895-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="74895-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74895-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="74895-114">Not supported.</span></span>    |
|<span data-ttu-id="74895-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="74895-115">Application</span></span> | <span data-ttu-id="74895-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="74895-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="74895-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="74895-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/delete
POST /workbook/worksheets/{id|name}/range(address='<address>')/delete
POST /workbook/tables/{id|name}/columns/{id|name}/range/delete

```
## <a name="request-headers"></a><span data-ttu-id="74895-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="74895-118">Request headers</span></span>
| <span data-ttu-id="74895-119">Nome</span><span class="sxs-lookup"><span data-stu-id="74895-119">Name</span></span>       | <span data-ttu-id="74895-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="74895-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="74895-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="74895-121">Authorization</span></span>  | <span data-ttu-id="74895-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="74895-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="74895-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="74895-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="74895-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="74895-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="74895-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="74895-127">Request body</span></span>
<span data-ttu-id="74895-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="74895-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="74895-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="74895-129">Parameter</span></span>    | <span data-ttu-id="74895-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="74895-130">Type</span></span>   |<span data-ttu-id="74895-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="74895-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="74895-132">shift</span><span class="sxs-lookup"><span data-stu-id="74895-132">shift</span></span>|<span data-ttu-id="74895-133">string</span><span class="sxs-lookup"><span data-stu-id="74895-133">string</span></span>|<span data-ttu-id="74895-134">Especifica como deslocar as células.</span><span class="sxs-lookup"><span data-stu-id="74895-134">Specifies which way to shift the cells.</span></span>  <span data-ttu-id="74895-135">Os valores possíveis são: `Up` , `Left` .</span><span class="sxs-lookup"><span data-stu-id="74895-135">The possible values are: `Up`, `Left`.</span></span>|

## <a name="response"></a><span data-ttu-id="74895-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="74895-136">Response</span></span>

<span data-ttu-id="74895-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="74895-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74895-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="74895-139">Example</span></span>
<span data-ttu-id="74895-140">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="74895-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="74895-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="74895-141">Request</span></span>
<span data-ttu-id="74895-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="74895-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="74895-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="74895-143">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="74895-144">C#</span><span class="sxs-lookup"><span data-stu-id="74895-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="74895-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="74895-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="74895-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="74895-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="74895-147">Java</span><span class="sxs-lookup"><span data-stu-id="74895-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-delete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="74895-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="74895-148">Response</span></span>
<span data-ttu-id="74895-149">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="74895-149">Here is an example of the response.</span></span> 
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

