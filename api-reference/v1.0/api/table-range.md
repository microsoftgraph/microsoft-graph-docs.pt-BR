---
title: 'workbooktable: Range'
description: Obtém o objeto de intervalo associado a toda a tabela.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 086ec5dc0ded09aed75ece8285e69d7ba73be806
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092045"
---
# <a name="workbooktable-range"></a><span data-ttu-id="7fe2d-103">workbooktable: Range</span><span class="sxs-lookup"><span data-stu-id="7fe2d-103">workbookTable: range</span></span>

<span data-ttu-id="7fe2d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7fe2d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7fe2d-105">Obter o objeto de intervalo associado a toda a tabela.</span><span class="sxs-lookup"><span data-stu-id="7fe2d-105">Get the range object associated with the entire table.</span></span>
## <a name="permissions"></a><span data-ttu-id="7fe2d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7fe2d-106">Permissions</span></span>
<span data-ttu-id="7fe2d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7fe2d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7fe2d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7fe2d-109">Permission type</span></span>      | <span data-ttu-id="7fe2d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7fe2d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7fe2d-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7fe2d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7fe2d-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7fe2d-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7fe2d-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7fe2d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7fe2d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7fe2d-114">Not supported.</span></span>    |
|<span data-ttu-id="7fe2d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7fe2d-115">Application</span></span> | <span data-ttu-id="7fe2d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7fe2d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7fe2d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7fe2d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/range
GET /workbook/worksheets/{id|name}/tables/{id|name}/range

```
## <a name="request-headers"></a><span data-ttu-id="7fe2d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7fe2d-118">Request headers</span></span>
| <span data-ttu-id="7fe2d-119">Nome</span><span class="sxs-lookup"><span data-stu-id="7fe2d-119">Name</span></span>       | <span data-ttu-id="7fe2d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="7fe2d-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7fe2d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7fe2d-121">Authorization</span></span>  | <span data-ttu-id="7fe2d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7fe2d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7fe2d-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7fe2d-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="7fe2d-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="7fe2d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7fe2d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7fe2d-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="7fe2d-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="7fe2d-128">Response</span></span>

<span data-ttu-id="7fe2d-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [workbookRange](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7fe2d-129">If successful, this method returns a `200 OK` response code and a [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7fe2d-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7fe2d-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="7fe2d-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7fe2d-131">Request</span></span>
<span data-ttu-id="7fe2d-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7fe2d-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7fe2d-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="7fe2d-133">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "table_range",
  "idempotent": true
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/range
```
# <a name="c"></a>[<span data-ttu-id="7fe2d-134">C#</span><span class="sxs-lookup"><span data-stu-id="7fe2d-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/table-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7fe2d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7fe2d-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/table-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7fe2d-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7fe2d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/table-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7fe2d-137">Java</span><span class="sxs-lookup"><span data-stu-id="7fe2d-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/table-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7fe2d-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="7fe2d-138">Response</span></span>
<span data-ttu-id="7fe2d-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7fe2d-139">The following is an example of the response.</span></span> 

><span data-ttu-id="7fe2d-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7fe2d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

