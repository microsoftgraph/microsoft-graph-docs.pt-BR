---
title: 'TableColumn: Range'
description: Obtém o objeto de intervalo associado a toda a coluna.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 96e62c43acc5e8d323da689bad49fb29e535b927
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35456642"
---
# <a name="tablecolumn-range"></a><span data-ttu-id="e854f-103">TableColumn: Range</span><span class="sxs-lookup"><span data-stu-id="e854f-103">TableColumn: Range</span></span>

<span data-ttu-id="e854f-104">Obtém o objeto de intervalo associado a toda a coluna.</span><span class="sxs-lookup"><span data-stu-id="e854f-104">Gets the range object associated with the entire column.</span></span>
## <a name="permissions"></a><span data-ttu-id="e854f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e854f-105">Permissions</span></span>
<span data-ttu-id="e854f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e854f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e854f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e854f-108">Permission type</span></span>      | <span data-ttu-id="e854f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e854f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e854f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e854f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e854f-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e854f-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e854f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e854f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e854f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e854f-113">Not supported.</span></span>    |
|<span data-ttu-id="e854f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e854f-114">Application</span></span> | <span data-ttu-id="e854f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e854f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e854f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e854f-116">HTTP request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e854f-117">HTTP</span><span class="sxs-lookup"><span data-stu-id="e854f-117">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/range
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/range

```
## <a name="request-headers"></a><span data-ttu-id="e854f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e854f-118">Request headers</span></span>
| <span data-ttu-id="e854f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e854f-119">Name</span></span>       | <span data-ttu-id="e854f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e854f-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e854f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e854f-121">Authorization</span></span>  | <span data-ttu-id="e854f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e854f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e854f-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e854f-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="e854f-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="e854f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e854f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e854f-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="e854f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e854f-128">Response</span></span>

<span data-ttu-id="e854f-129">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e854f-129">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e854f-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e854f-130">Example</span></span>
<span data-ttu-id="e854f-131">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="e854f-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e854f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e854f-132">Request</span></span>
<span data-ttu-id="e854f-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e854f-133">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "tablecolumn_range",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e854f-134">C#</span><span class="sxs-lookup"><span data-stu-id="e854f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablecolumn-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e854f-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="e854f-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablecolumn-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e854f-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="e854f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablecolumn-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e854f-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="e854f-137">Response</span></span>
<span data-ttu-id="e854f-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e854f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "TableColumn: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
