---
title: 'Table: HeaderRowRange'
description: Obtém o objeto de intervalo associado à linha de cabeçalho da tabela.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: b350ea0b6976774bbb6f87e3225240a16bcb47cf
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055726"
---
# <a name="table-headerrowrange"></a><span data-ttu-id="7fb0f-103">Table: HeaderRowRange</span><span class="sxs-lookup"><span data-stu-id="7fb0f-103">Table: HeaderRowRange</span></span>

<span data-ttu-id="7fb0f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7fb0f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7fb0f-105">Obtém o objeto de intervalo associado à linha de cabeçalho da tabela.</span><span class="sxs-lookup"><span data-stu-id="7fb0f-105">Gets the range object associated with header row of the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="7fb0f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7fb0f-106">Permissions</span></span>
<span data-ttu-id="7fb0f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7fb0f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7fb0f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7fb0f-109">Permission type</span></span>      | <span data-ttu-id="7fb0f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7fb0f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7fb0f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7fb0f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7fb0f-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7fb0f-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7fb0f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7fb0f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7fb0f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7fb0f-114">Not supported.</span></span>    |
|<span data-ttu-id="7fb0f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7fb0f-115">Application</span></span> | <span data-ttu-id="7fb0f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7fb0f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7fb0f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7fb0f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/tables/{id|name}/headerRowRange
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/headerRowRange
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/headerRowRange
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/headerRowRange

```
## <a name="request-headers"></a><span data-ttu-id="7fb0f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7fb0f-118">Request headers</span></span>
| <span data-ttu-id="7fb0f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="7fb0f-119">Name</span></span>       | <span data-ttu-id="7fb0f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="7fb0f-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7fb0f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7fb0f-121">Authorization</span></span>  | <span data-ttu-id="7fb0f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7fb0f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7fb0f-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7fb0f-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="7fb0f-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="7fb0f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7fb0f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7fb0f-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="7fb0f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="7fb0f-128">Response</span></span>

<span data-ttu-id="7fb0f-129">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7fb0f-129">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7fb0f-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7fb0f-130">Example</span></span>
<span data-ttu-id="7fb0f-131">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="7fb0f-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7fb0f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7fb0f-132">Request</span></span>
<span data-ttu-id="7fb0f-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7fb0f-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7fb0f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="7fb0f-134">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "table_headerrowrange",
  "idempotent": true
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/headerRowRange
```
# <a name="c"></a>[<span data-ttu-id="7fb0f-135">C#</span><span class="sxs-lookup"><span data-stu-id="7fb0f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/table-headerrowrange-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7fb0f-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7fb0f-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/table-headerrowrange-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7fb0f-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7fb0f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/table-headerrowrange-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7fb0f-138">Java</span><span class="sxs-lookup"><span data-stu-id="7fb0f-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/table-headerrowrange-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7fb0f-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="7fb0f-139">Response</span></span>
<span data-ttu-id="7fb0f-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7fb0f-140">Here is an example of the response.</span></span> <span data-ttu-id="7fb0f-141">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7fb0f-141">Note: The response object shown here might be shortened for readability.</span></span>
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
  "description": "Table: HeaderRowRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

