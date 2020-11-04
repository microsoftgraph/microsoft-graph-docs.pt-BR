---
title: 'Table: TotalRowRange'
description: Obtém o objeto de intervalo associado à linha de totais da tabela.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 5f28adba4a869d0c2ca1cbe756db4cacd75ee258
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904673"
---
# <a name="table-totalrowrange"></a><span data-ttu-id="c71f7-103">Table: TotalRowRange</span><span class="sxs-lookup"><span data-stu-id="c71f7-103">Table: TotalRowRange</span></span>

<span data-ttu-id="c71f7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c71f7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c71f7-105">Obtém o objeto de intervalo associado à linha de totais da tabela.</span><span class="sxs-lookup"><span data-stu-id="c71f7-105">Gets the range object associated with totals row of the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="c71f7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c71f7-106">Permissions</span></span>
<span data-ttu-id="c71f7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c71f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c71f7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c71f7-109">Permission type</span></span>      | <span data-ttu-id="c71f7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c71f7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c71f7-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c71f7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c71f7-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c71f7-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c71f7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c71f7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c71f7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c71f7-114">Not supported.</span></span>    |
|<span data-ttu-id="c71f7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c71f7-115">Application</span></span> | <span data-ttu-id="c71f7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c71f7-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c71f7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c71f7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/totalRowRange
GET /workbook/worksheets/{id|name}/tables/{id|name}/totalRowRange

```
## <a name="request-headers"></a><span data-ttu-id="c71f7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c71f7-118">Request headers</span></span>
| <span data-ttu-id="c71f7-119">Nome</span><span class="sxs-lookup"><span data-stu-id="c71f7-119">Name</span></span>       | <span data-ttu-id="c71f7-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="c71f7-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c71f7-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c71f7-121">Authorization</span></span>  | <span data-ttu-id="c71f7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c71f7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c71f7-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c71f7-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="c71f7-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="c71f7-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c71f7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c71f7-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="c71f7-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c71f7-128">Response</span></span>

<span data-ttu-id="c71f7-129">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c71f7-129">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c71f7-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c71f7-130">Example</span></span>
<span data-ttu-id="c71f7-131">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="c71f7-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c71f7-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c71f7-132">Request</span></span>
<span data-ttu-id="c71f7-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c71f7-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c71f7-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="c71f7-134">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "table_totalrowrange",
  "idempotent": true
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/totalRowRange
```
# <a name="c"></a>[<span data-ttu-id="c71f7-135">C#</span><span class="sxs-lookup"><span data-stu-id="c71f7-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/table-totalrowrange-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c71f7-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c71f7-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/table-totalrowrange-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c71f7-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c71f7-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/table-totalrowrange-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c71f7-138">Java</span><span class="sxs-lookup"><span data-stu-id="c71f7-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/table-totalrowrange-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c71f7-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="c71f7-139">Response</span></span>
<span data-ttu-id="c71f7-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c71f7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Table: TotalRowRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

