---
title: 'workbookTable: range'
description: Obtém o objeto de intervalo associado a toda a tabela.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 23112ea6e9bd594dc12db2b4e68faf5826587460
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50575081"
---
# <a name="workbooktable-range"></a><span data-ttu-id="911b1-103">workbookTable: range</span><span class="sxs-lookup"><span data-stu-id="911b1-103">workbookTable: range</span></span>

<span data-ttu-id="911b1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="911b1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="911b1-105">Obter o objeto range associado à tabela inteira.</span><span class="sxs-lookup"><span data-stu-id="911b1-105">Get the range object associated with the entire table.</span></span>
## <a name="permissions"></a><span data-ttu-id="911b1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="911b1-106">Permissions</span></span>
<span data-ttu-id="911b1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="911b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="911b1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="911b1-109">Permission type</span></span>      | <span data-ttu-id="911b1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="911b1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="911b1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="911b1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="911b1-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="911b1-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="911b1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="911b1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="911b1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="911b1-114">Not supported.</span></span>    |
|<span data-ttu-id="911b1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="911b1-115">Application</span></span> | <span data-ttu-id="911b1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="911b1-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="911b1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="911b1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/tables/{id|name}/range
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/range
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/range
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/range

```
## <a name="request-headers"></a><span data-ttu-id="911b1-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="911b1-118">Request headers</span></span>
| <span data-ttu-id="911b1-119">Nome</span><span class="sxs-lookup"><span data-stu-id="911b1-119">Name</span></span>       | <span data-ttu-id="911b1-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="911b1-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="911b1-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="911b1-121">Authorization</span></span>  | <span data-ttu-id="911b1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="911b1-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="911b1-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="911b1-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="911b1-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="911b1-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="911b1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="911b1-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="911b1-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="911b1-128">Response</span></span>

<span data-ttu-id="911b1-129">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [workbookRange](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="911b1-129">If successful, this method returns a `200 OK` response code and a [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="911b1-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="911b1-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="911b1-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="911b1-131">Request</span></span>
<span data-ttu-id="911b1-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="911b1-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="911b1-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="911b1-133">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "table_range",
  "idempotent": true
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/range
```
# <a name="c"></a>[<span data-ttu-id="911b1-134">C#</span><span class="sxs-lookup"><span data-stu-id="911b1-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/table-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="911b1-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="911b1-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/table-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="911b1-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="911b1-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/table-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="911b1-137">Java</span><span class="sxs-lookup"><span data-stu-id="911b1-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/table-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="911b1-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="911b1-138">Response</span></span>
<span data-ttu-id="911b1-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="911b1-139">The following is an example of the response.</span></span> 

><span data-ttu-id="911b1-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="911b1-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

