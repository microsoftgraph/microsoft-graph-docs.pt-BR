---
title: 'TableColumn: DataBodyRange'
description: Obtém o objeto de intervalo associado ao corpo de dados da coluna.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 0031c29ce4228ad36ef03c0d6aa0b149f09a9785
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35278873"
---
# <a name="tablecolumn-databodyrange"></a><span data-ttu-id="807d6-103">TableColumn: DataBodyRange</span><span class="sxs-lookup"><span data-stu-id="807d6-103">TableColumn: DataBodyRange</span></span>

<span data-ttu-id="807d6-104">Obtém o objeto de intervalo associado ao corpo de dados da coluna.</span><span class="sxs-lookup"><span data-stu-id="807d6-104">Gets the range object associated with the data body of the column.</span></span>
## <a name="permissions"></a><span data-ttu-id="807d6-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="807d6-105">Permissions</span></span>
<span data-ttu-id="807d6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="807d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="807d6-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="807d6-108">Permission type</span></span>      | <span data-ttu-id="807d6-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="807d6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="807d6-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="807d6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="807d6-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="807d6-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="807d6-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="807d6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="807d6-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="807d6-113">Not supported.</span></span>    |
|<span data-ttu-id="807d6-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="807d6-114">Application</span></span> | <span data-ttu-id="807d6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="807d6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="807d6-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="807d6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/dataBodyRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/dataBodyRange

```
## <a name="request-headers"></a><span data-ttu-id="807d6-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="807d6-117">Request headers</span></span>
| <span data-ttu-id="807d6-118">Nome</span><span class="sxs-lookup"><span data-stu-id="807d6-118">Name</span></span>       | <span data-ttu-id="807d6-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="807d6-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="807d6-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="807d6-120">Authorization</span></span>  | <span data-ttu-id="807d6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="807d6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="807d6-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="807d6-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="807d6-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="807d6-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="807d6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="807d6-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="807d6-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="807d6-127">Response</span></span>

<span data-ttu-id="807d6-128">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="807d6-128">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="807d6-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="807d6-129">Example</span></span>
<span data-ttu-id="807d6-130">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="807d6-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="807d6-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="807d6-131">Request</span></span>
<span data-ttu-id="807d6-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="807d6-132">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "tablecolumn_databodyrange",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/dataBodyRange
```

##### <a name="response"></a><span data-ttu-id="807d6-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="807d6-133">Response</span></span>
<span data-ttu-id="807d6-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="807d6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="807d6-137">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="807d6-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="807d6-138">C#</span><span class="sxs-lookup"><span data-stu-id="807d6-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/tablecolumn_databodyrange-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="807d6-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="807d6-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/tablecolumn_databodyrange-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="807d6-140">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="807d6-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/tablecolumn_databodyrange-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableColumn: DataBodyRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/tablecolumn-databodyrange.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/tablecolumn-databodyrange.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/tablecolumn-databodyrange.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
