---
title: 'Range: LastColumn'
description: .
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 034c589d89570319dd47704a4079f5c4df20d5a8
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055817"
---
# <a name="range-lastcolumn"></a><span data-ttu-id="d7e08-103">Range: LastColumn</span><span class="sxs-lookup"><span data-stu-id="d7e08-103">Range: LastColumn</span></span>

<span data-ttu-id="d7e08-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7e08-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d7e08-p101">Obtém a última coluna do intervalo. Por exemplo, a última coluna de "B2:D5" é "D2:D5".</span><span class="sxs-lookup"><span data-stu-id="d7e08-p101">Gets the last column within the range. For example, the last column of "B2:D5" is "D2:D5".</span></span>
## <a name="permissions"></a><span data-ttu-id="d7e08-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d7e08-107">Permissions</span></span>
<span data-ttu-id="d7e08-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7e08-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7e08-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d7e08-110">Permission type</span></span>      | <span data-ttu-id="d7e08-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d7e08-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7e08-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d7e08-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d7e08-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d7e08-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d7e08-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d7e08-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7e08-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d7e08-115">Not supported.</span></span>    |
|<span data-ttu-id="d7e08-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d7e08-116">Application</span></span> | <span data-ttu-id="d7e08-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d7e08-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d7e08-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d7e08-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/names/{name}/range/lastColumn
GET /me/drive/root:/{item-path}:/workbook/names/{name}/range/lastColumn
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/lastColumn
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/lastColumn
GET /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/lastColumn
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/lastColumn

```
## <a name="request-headers"></a><span data-ttu-id="d7e08-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d7e08-119">Request headers</span></span>
| <span data-ttu-id="d7e08-120">Nome</span><span class="sxs-lookup"><span data-stu-id="d7e08-120">Name</span></span>       | <span data-ttu-id="d7e08-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7e08-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d7e08-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d7e08-122">Authorization</span></span>  | <span data-ttu-id="d7e08-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d7e08-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d7e08-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d7e08-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="d7e08-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="d7e08-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7e08-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d7e08-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="d7e08-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7e08-129">Response</span></span>

<span data-ttu-id="d7e08-130">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d7e08-130">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7e08-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d7e08-131">Example</span></span>
<span data-ttu-id="d7e08-132">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="d7e08-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d7e08-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d7e08-133">Request</span></span>
<span data-ttu-id="d7e08-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d7e08-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d7e08-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="d7e08-135">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_lastcolumn"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/lastColumn
```
# <a name="c"></a>[<span data-ttu-id="d7e08-136">C#</span><span class="sxs-lookup"><span data-stu-id="d7e08-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-lastcolumn-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d7e08-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d7e08-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-lastcolumn-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d7e08-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d7e08-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-lastcolumn-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d7e08-139">Java</span><span class="sxs-lookup"><span data-stu-id="d7e08-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-lastcolumn-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d7e08-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7e08-140">Response</span></span>
<span data-ttu-id="d7e08-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d7e08-141">Here is an example of the response.</span></span> <span data-ttu-id="d7e08-142">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d7e08-142">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: LastColumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

