---
title: 'Range: LastRow'
description: .
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 9351acf4210324cbf1e2a4b68772ad021728917f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35459094"
---
# <a name="range-lastrow"></a><span data-ttu-id="39b10-103">Range: LastRow</span><span class="sxs-lookup"><span data-stu-id="39b10-103">Range: LastRow</span></span>

<span data-ttu-id="39b10-p101">Obtém a última linha do intervalo. Por exemplo, a última linha de "B2:D5" é "B5:D5".</span><span class="sxs-lookup"><span data-stu-id="39b10-p101">Gets the last row within the range. For example, the last row of "B2:D5" is "B5:D5".</span></span>
## <a name="permissions"></a><span data-ttu-id="39b10-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="39b10-106">Permissions</span></span>
<span data-ttu-id="39b10-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39b10-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39b10-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="39b10-109">Permission type</span></span>      | <span data-ttu-id="39b10-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="39b10-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="39b10-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="39b10-111">Delegated (work or school account)</span></span> | <span data-ttu-id="39b10-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="39b10-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="39b10-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="39b10-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39b10-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="39b10-114">Not supported.</span></span>    |
|<span data-ttu-id="39b10-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="39b10-115">Application</span></span> | <span data-ttu-id="39b10-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="39b10-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="39b10-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="39b10-117">HTTP request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="39b10-118">HTTP</span><span class="sxs-lookup"><span data-stu-id="39b10-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/lastRow
GET /workbook/worksheets/{id|name}/range(address='<address>')/lastRow
GET /workbook/tables/{id|name}/columns/{id|name}/range/lastRow

```
## <a name="request-headers"></a><span data-ttu-id="39b10-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="39b10-119">Request headers</span></span>
| <span data-ttu-id="39b10-120">Nome</span><span class="sxs-lookup"><span data-stu-id="39b10-120">Name</span></span>       | <span data-ttu-id="39b10-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="39b10-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="39b10-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="39b10-122">Authorization</span></span>  | <span data-ttu-id="39b10-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="39b10-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="39b10-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="39b10-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="39b10-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="39b10-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="39b10-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="39b10-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="39b10-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="39b10-129">Response</span></span>

<span data-ttu-id="39b10-130">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="39b10-130">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39b10-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="39b10-131">Example</span></span>
<span data-ttu-id="39b10-132">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="39b10-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="39b10-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="39b10-133">Request</span></span>
<span data-ttu-id="39b10-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="39b10-134">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_lastrow"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/lastRow
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="39b10-135">C#</span><span class="sxs-lookup"><span data-stu-id="39b10-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-lastrow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="39b10-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="39b10-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-lastrow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="39b10-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="39b10-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-lastrow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="39b10-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="39b10-138">Response</span></span>
<span data-ttu-id="39b10-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="39b10-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: LastRow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
