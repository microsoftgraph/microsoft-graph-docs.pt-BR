---
title: 'Range: EntireColumn'
description: Obtém um objeto que representa toda a coluna do intervalo.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: ba549d473d1ef922119cb69b670fb063fbc99fb5
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36728402"
---
# <a name="range-entirecolumn"></a><span data-ttu-id="db46d-103">Range: EntireColumn</span><span class="sxs-lookup"><span data-stu-id="db46d-103">Range: EntireColumn</span></span>

<span data-ttu-id="db46d-104">Obtém um objeto que representa toda a coluna do intervalo.</span><span class="sxs-lookup"><span data-stu-id="db46d-104">Gets an object that represents the entire column of the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="db46d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="db46d-105">Permissions</span></span>
<span data-ttu-id="db46d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db46d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db46d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="db46d-108">Permission type</span></span>      | <span data-ttu-id="db46d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="db46d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db46d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="db46d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="db46d-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="db46d-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="db46d-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="db46d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db46d-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="db46d-113">Not supported.</span></span>    |
|<span data-ttu-id="db46d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="db46d-114">Application</span></span> | <span data-ttu-id="db46d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="db46d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="db46d-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="db46d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/entireColumn
GET /workbook/worksheets/{id|name}/range(address='<address>')/entireColumn
GET /workbook/tables/{id|name}/columns/{id|name}/range/entireColumn

```
## <a name="request-headers"></a><span data-ttu-id="db46d-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="db46d-117">Request headers</span></span>
| <span data-ttu-id="db46d-118">Nome</span><span class="sxs-lookup"><span data-stu-id="db46d-118">Name</span></span>       | <span data-ttu-id="db46d-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="db46d-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="db46d-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="db46d-120">Authorization</span></span>  | <span data-ttu-id="db46d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="db46d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="db46d-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="db46d-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="db46d-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="db46d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="db46d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="db46d-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="db46d-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="db46d-127">Response</span></span>

<span data-ttu-id="db46d-128">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="db46d-128">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db46d-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="db46d-129">Example</span></span>
<span data-ttu-id="db46d-130">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="db46d-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="db46d-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="db46d-131">Request</span></span>
<span data-ttu-id="db46d-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="db46d-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="db46d-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="db46d-133">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_entirecolumn"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/entireColumn
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="db46d-134">C#</span><span class="sxs-lookup"><span data-stu-id="db46d-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-entirecolumn-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="db46d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db46d-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-entirecolumn-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="db46d-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="db46d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-entirecolumn-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="db46d-137">Java</span><span class="sxs-lookup"><span data-stu-id="db46d-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-entirecolumn-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="db46d-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="db46d-138">Response</span></span>
<span data-ttu-id="db46d-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="db46d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: EntireColumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
