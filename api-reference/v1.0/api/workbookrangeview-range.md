---
title: 'workbookRangeView: intervalo'
description: Retorne o intervalo associado com o recurso rangeView.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 225d57611fc95abf7fc305294f41e36dbb58f251
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049356"
---
# <a name="workbookrangeview-range"></a><span data-ttu-id="70525-103">workbookRangeView: intervalo</span><span class="sxs-lookup"><span data-stu-id="70525-103">workbookRangeView: range</span></span>

<span data-ttu-id="70525-104">Namespace: microsoft.graph Retornar o intervalo associado ao recurso rangeView.</span><span class="sxs-lookup"><span data-stu-id="70525-104">Namespace: microsoft.graph Return the range associated with the rangeView resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="70525-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="70525-105">Permissions</span></span>
<span data-ttu-id="70525-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70525-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="70525-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="70525-108">Permission type</span></span>      | <span data-ttu-id="70525-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="70525-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="70525-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="70525-110">Delegated (work or school account)</span></span> | <span data-ttu-id="70525-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="70525-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="70525-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="70525-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70525-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="70525-113">Not supported.</span></span>    |
|<span data-ttu-id="70525-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="70525-114">Application</span></span> | <span data-ttu-id="70525-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="70525-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="70525-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="70525-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets/{id}/range(address={address})/visibleView/range
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id}/range(address={address})/visibleView/range

```
## <a name="request-headers"></a><span data-ttu-id="70525-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="70525-117">Request headers</span></span>
| <span data-ttu-id="70525-118">Nome</span><span class="sxs-lookup"><span data-stu-id="70525-118">Name</span></span>       | <span data-ttu-id="70525-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="70525-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="70525-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="70525-120">Authorization</span></span>  | <span data-ttu-id="70525-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="70525-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="70525-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="70525-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="70525-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="70525-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="70525-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="70525-126">Request body</span></span>

### <a name="response"></a><span data-ttu-id="70525-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="70525-127">Response</span></span>
<span data-ttu-id="70525-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="70525-128">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70525-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="70525-129">Example</span></span>
<span data-ttu-id="70525-130">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="70525-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="70525-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="70525-131">Request</span></span>
<span data-ttu-id="70525-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="70525-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="70525-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="70525-133">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrangeview_range"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView/range
```
# <a name="c"></a>[<span data-ttu-id="70525-134">C#</span><span class="sxs-lookup"><span data-stu-id="70525-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrangeview-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="70525-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="70525-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrangeview-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="70525-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="70525-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrangeview-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="70525-137">Java</span><span class="sxs-lookup"><span data-stu-id="70525-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookrangeview-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="70525-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="70525-138">Response</span></span>
<span data-ttu-id="70525-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="70525-139">Here is an example of the response.</span></span> <span data-ttu-id="70525-140">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="70525-140">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 157

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnHidden": true,
  "columnIndex": 99
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

