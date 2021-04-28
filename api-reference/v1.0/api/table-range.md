---
title: 'workbookTable: range'
description: Obtém o objeto de intervalo associado a toda a tabela.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: e1b01a3a8df2288084803fb07ba5ccd489844a23
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054396"
---
# <a name="workbooktable-range"></a><span data-ttu-id="22c92-103">workbookTable: range</span><span class="sxs-lookup"><span data-stu-id="22c92-103">workbookTable: range</span></span>

<span data-ttu-id="22c92-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22c92-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="22c92-105">Obter o objeto range associado à tabela inteira.</span><span class="sxs-lookup"><span data-stu-id="22c92-105">Get the range object associated with the entire table.</span></span>
## <a name="permissions"></a><span data-ttu-id="22c92-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="22c92-106">Permissions</span></span>
<span data-ttu-id="22c92-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22c92-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22c92-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="22c92-109">Permission type</span></span>      | <span data-ttu-id="22c92-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="22c92-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="22c92-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="22c92-111">Delegated (work or school account)</span></span> | <span data-ttu-id="22c92-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="22c92-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="22c92-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="22c92-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22c92-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22c92-114">Not supported.</span></span>    |
|<span data-ttu-id="22c92-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="22c92-115">Application</span></span> | <span data-ttu-id="22c92-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22c92-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="22c92-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="22c92-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/tables/{id|name}/range
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/range
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/range
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/range

```
## <a name="request-headers"></a><span data-ttu-id="22c92-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="22c92-118">Request headers</span></span>
| <span data-ttu-id="22c92-119">Nome</span><span class="sxs-lookup"><span data-stu-id="22c92-119">Name</span></span>       | <span data-ttu-id="22c92-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="22c92-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="22c92-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="22c92-121">Authorization</span></span>  | <span data-ttu-id="22c92-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="22c92-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="22c92-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="22c92-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="22c92-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="22c92-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="22c92-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="22c92-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="22c92-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="22c92-128">Response</span></span>

<span data-ttu-id="22c92-129">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [workbookRange](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="22c92-129">If successful, this method returns a `200 OK` response code and a [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22c92-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="22c92-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="22c92-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="22c92-131">Request</span></span>
<span data-ttu-id="22c92-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="22c92-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="22c92-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="22c92-133">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "table_range",
  "idempotent": true
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/range
```
# <a name="c"></a>[<span data-ttu-id="22c92-134">C#</span><span class="sxs-lookup"><span data-stu-id="22c92-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/table-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="22c92-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="22c92-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/table-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="22c92-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="22c92-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/table-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="22c92-137">Java</span><span class="sxs-lookup"><span data-stu-id="22c92-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/table-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="22c92-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="22c92-138">Response</span></span>
<span data-ttu-id="22c92-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="22c92-139">The following is an example of the response.</span></span> 

><span data-ttu-id="22c92-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="22c92-140">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "description": "Table: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

