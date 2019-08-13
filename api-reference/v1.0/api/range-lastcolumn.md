---
title: 'Range: LastColumn'
description: .
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 2660442f59b6d50cb91c81586348d2abb4655fcf
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36375531"
---
# <a name="range-lastcolumn"></a><span data-ttu-id="9b4a3-103">Range: LastColumn</span><span class="sxs-lookup"><span data-stu-id="9b4a3-103">Range: LastColumn</span></span>

<span data-ttu-id="9b4a3-p101">Obtém a última coluna do intervalo. Por exemplo, a última coluna de "B2:D5" é "D2:D5".</span><span class="sxs-lookup"><span data-stu-id="9b4a3-p101">Gets the last column within the range. For example, the last column of "B2:D5" is "D2:D5".</span></span>
## <a name="permissions"></a><span data-ttu-id="9b4a3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9b4a3-106">Permissions</span></span>
<span data-ttu-id="9b4a3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b4a3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b4a3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9b4a3-109">Permission type</span></span>      | <span data-ttu-id="9b4a3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9b4a3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9b4a3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9b4a3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9b4a3-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9b4a3-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9b4a3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9b4a3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b4a3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9b4a3-114">Not supported.</span></span>    |
|<span data-ttu-id="9b4a3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9b4a3-115">Application</span></span> | <span data-ttu-id="9b4a3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9b4a3-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9b4a3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9b4a3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/lastColumn
GET /workbook/worksheets/{id|name}/range(address='<address>')/lastColumn
GET /workbook/tables/{id|name}/columns/{id|name}/range/lastColumn

```
## <a name="request-headers"></a><span data-ttu-id="9b4a3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9b4a3-118">Request headers</span></span>
| <span data-ttu-id="9b4a3-119">Nome</span><span class="sxs-lookup"><span data-stu-id="9b4a3-119">Name</span></span>       | <span data-ttu-id="9b4a3-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b4a3-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9b4a3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9b4a3-121">Authorization</span></span>  | <span data-ttu-id="9b4a3-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9b4a3-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9b4a3-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9b4a3-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="9b4a3-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="9b4a3-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b4a3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9b4a3-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="9b4a3-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b4a3-128">Response</span></span>

<span data-ttu-id="9b4a3-129">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9b4a3-129">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b4a3-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9b4a3-130">Example</span></span>
<span data-ttu-id="9b4a3-131">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="9b4a3-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9b4a3-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9b4a3-132">Request</span></span>
<span data-ttu-id="9b4a3-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9b4a3-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9b4a3-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="9b4a3-134">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_lastcolumn"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/lastColumn
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9b4a3-135">C#</span><span class="sxs-lookup"><span data-stu-id="9b4a3-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-lastcolumn-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9b4a3-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9b4a3-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-lastcolumn-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9b4a3-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="9b4a3-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-lastcolumn-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9b4a3-138">Java</span><span class="sxs-lookup"><span data-stu-id="9b4a3-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-lastcolumn-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9b4a3-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b4a3-139">Response</span></span>
<span data-ttu-id="9b4a3-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9b4a3-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: LastColumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
