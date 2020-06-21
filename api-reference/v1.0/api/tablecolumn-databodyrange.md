---
title: 'TableColumn: DataBodyRange'
description: Obtém o objeto de intervalo associado ao corpo de dados da coluna.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: dfa72e3b0fc6698b2df0bafc9ae5e7d0c79b9c47
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44788777"
---
# <a name="tablecolumn-databodyrange"></a><span data-ttu-id="f0a19-103">TableColumn: DataBodyRange</span><span class="sxs-lookup"><span data-stu-id="f0a19-103">TableColumn: DataBodyRange</span></span>

<span data-ttu-id="f0a19-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0a19-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f0a19-105">Obtém o objeto de intervalo associado ao corpo de dados da coluna.</span><span class="sxs-lookup"><span data-stu-id="f0a19-105">Gets the range object associated with the data body of the column.</span></span>
## <a name="permissions"></a><span data-ttu-id="f0a19-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f0a19-106">Permissions</span></span>
<span data-ttu-id="f0a19-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="f0a19-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="f0a19-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0a19-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0a19-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f0a19-109">Permission type</span></span>      | <span data-ttu-id="f0a19-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f0a19-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f0a19-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f0a19-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f0a19-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f0a19-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f0a19-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f0a19-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0a19-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f0a19-114">Not supported.</span></span>    |
|<span data-ttu-id="f0a19-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f0a19-115">Application</span></span> | <span data-ttu-id="f0a19-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f0a19-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f0a19-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f0a19-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/columns/{id|name}/dataBodyRange
GET /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/dataBodyRange

```
## <a name="request-headers"></a><span data-ttu-id="f0a19-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f0a19-118">Request headers</span></span>
| <span data-ttu-id="f0a19-119">Nome</span><span class="sxs-lookup"><span data-stu-id="f0a19-119">Name</span></span>       | <span data-ttu-id="f0a19-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0a19-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f0a19-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f0a19-121">Authorization</span></span>  | <span data-ttu-id="f0a19-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="f0a19-122">Bearer {token}.</span></span> <span data-ttu-id="f0a19-123">Required.</span><span class="sxs-lookup"><span data-stu-id="f0a19-123">Required.</span></span> |
| <span data-ttu-id="f0a19-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f0a19-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="f0a19-125">Workbook session Id that determines if changes are persisted or not.</span><span class="sxs-lookup"><span data-stu-id="f0a19-125">Workbook session Id that determines if changes are persisted or not.</span></span> <span data-ttu-id="f0a19-126">Optional.</span><span class="sxs-lookup"><span data-stu-id="f0a19-126">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0a19-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f0a19-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="f0a19-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0a19-128">Response</span></span>

<span data-ttu-id="f0a19-129">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f0a19-129">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0a19-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f0a19-130">Example</span></span>
<span data-ttu-id="f0a19-131">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="f0a19-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f0a19-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f0a19-132">Request</span></span>
<span data-ttu-id="f0a19-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f0a19-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f0a19-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="f0a19-134">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "tablecolumn_databodyrange",
  "idempotent": true
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/dataBodyRange
```
# <a name="c"></a>[<span data-ttu-id="f0a19-135">C#</span><span class="sxs-lookup"><span data-stu-id="f0a19-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablecolumn-databodyrange-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f0a19-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f0a19-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablecolumn-databodyrange-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f0a19-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f0a19-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablecolumn-databodyrange-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f0a19-138">Java</span><span class="sxs-lookup"><span data-stu-id="f0a19-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tablecolumn-databodyrange-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f0a19-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0a19-139">Response</span></span>
<span data-ttu-id="f0a19-140">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="f0a19-140">Here is an example of the response.</span></span> <span data-ttu-id="f0a19-141">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="f0a19-141">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f0a19-142">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="f0a19-142">All of the properties will be returned from an actual call.</span></span>
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
  "description": "TableColumn: DataBodyRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
