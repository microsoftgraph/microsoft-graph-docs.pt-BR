---
title: 'Table: TotalRowRange'
description: Obtém o objeto de intervalo associado à linha de totais da tabela.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: b6c4335d640a54a74683225bc50418c0a0d54ca1
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050840"
---
# <a name="table-totalrowrange"></a><span data-ttu-id="bfb8d-103">Table: TotalRowRange</span><span class="sxs-lookup"><span data-stu-id="bfb8d-103">Table: TotalRowRange</span></span>

<span data-ttu-id="bfb8d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bfb8d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bfb8d-105">Obtém o objeto de intervalo associado à linha de totais da tabela.</span><span class="sxs-lookup"><span data-stu-id="bfb8d-105">Gets the range object associated with totals row of the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="bfb8d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bfb8d-106">Permissions</span></span>
<span data-ttu-id="bfb8d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bfb8d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bfb8d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bfb8d-109">Permission type</span></span>      | <span data-ttu-id="bfb8d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bfb8d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bfb8d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bfb8d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bfb8d-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bfb8d-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bfb8d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bfb8d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bfb8d-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bfb8d-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bfb8d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bfb8d-115">Application</span></span> | <span data-ttu-id="bfb8d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bfb8d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bfb8d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bfb8d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/tables/{id|name}/TotalRowRange
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/TotalRowRange
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/TotalRowRange
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/TotalRowRange

```
## <a name="request-headers"></a><span data-ttu-id="bfb8d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bfb8d-118">Request headers</span></span>
| <span data-ttu-id="bfb8d-119">Nome</span><span class="sxs-lookup"><span data-stu-id="bfb8d-119">Name</span></span>       | <span data-ttu-id="bfb8d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="bfb8d-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="bfb8d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="bfb8d-121">Authorization</span></span>  | <span data-ttu-id="bfb8d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bfb8d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bfb8d-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="bfb8d-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="bfb8d-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="bfb8d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bfb8d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bfb8d-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="bfb8d-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="bfb8d-128">Response</span></span>

<span data-ttu-id="bfb8d-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/workbookrange.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bfb8d-129">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bfb8d-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bfb8d-130">Example</span></span>
<span data-ttu-id="bfb8d-131">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="bfb8d-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="bfb8d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bfb8d-132">Request</span></span>
<span data-ttu-id="bfb8d-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bfb8d-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bfb8d-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="bfb8d-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "table_totalrowrange"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/TotalRowRange
```
# <a name="c"></a>[<span data-ttu-id="bfb8d-135">C#</span><span class="sxs-lookup"><span data-stu-id="bfb8d-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/table-totalrowrange-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bfb8d-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bfb8d-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/table-totalrowrange-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bfb8d-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bfb8d-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/table-totalrowrange-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bfb8d-138">Java</span><span class="sxs-lookup"><span data-stu-id="bfb8d-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/table-totalrowrange-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="bfb8d-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="bfb8d-139">Response</span></span>
<span data-ttu-id="bfb8d-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bfb8d-140">Here is an example of the response.</span></span> <span data-ttu-id="bfb8d-141">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="bfb8d-141">Note: The response object shown here might be shortened for readability.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Table: TotalRowRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


