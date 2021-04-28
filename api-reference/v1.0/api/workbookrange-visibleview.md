---
title: 'workbookRange: visibleView'
description: Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira Permissões.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: cc18dd61d7a1307c11e968a383d3e0ea72a64dc2
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055649"
---
# <a name="workbookrange-visibleview"></a><span data-ttu-id="9a195-104">workbookRange: visibleView</span><span class="sxs-lookup"><span data-stu-id="9a195-104">workbookRange: visibleView</span></span>

<span data-ttu-id="9a195-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a195-105">Namespace: microsoft.graph</span></span>


## <a name="permissions"></a><span data-ttu-id="9a195-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9a195-106">Permissions</span></span>
<span data-ttu-id="9a195-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a195-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a195-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9a195-109">Permission type</span></span>      | <span data-ttu-id="9a195-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9a195-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a195-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9a195-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9a195-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9a195-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9a195-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9a195-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a195-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9a195-114">Not supported.</span></span>    |
|<span data-ttu-id="9a195-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9a195-115">Application</span></span> | <span data-ttu-id="9a195-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9a195-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a195-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9a195-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets/{id}/range(address={address})/visibleView
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id}/range(address={address})/visibleView
```
## <a name="request-headers"></a><span data-ttu-id="9a195-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9a195-118">Request headers</span></span>
| <span data-ttu-id="9a195-119">Nome</span><span class="sxs-lookup"><span data-stu-id="9a195-119">Name</span></span>       | <span data-ttu-id="9a195-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a195-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9a195-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9a195-121">Authorization</span></span>  | <span data-ttu-id="9a195-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9a195-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9a195-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9a195-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="9a195-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="9a195-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a195-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9a195-127">Request body</span></span>

### <a name="response"></a><span data-ttu-id="9a195-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a195-128">Response</span></span>
<span data-ttu-id="9a195-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRangeView](../resources/workbookrangeview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9a195-129">If successful, this method returns `200 OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a195-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9a195-130">Example</span></span>
<span data-ttu-id="9a195-131">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="9a195-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9a195-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9a195-132">Request</span></span>
<span data-ttu-id="9a195-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9a195-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9a195-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="9a195-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "workbookrange_visibleview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView
```
# <a name="c"></a>[<span data-ttu-id="9a195-135">C#</span><span class="sxs-lookup"><span data-stu-id="9a195-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrange-visibleview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9a195-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9a195-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrange-visibleview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9a195-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9a195-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrange-visibleview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9a195-138">Java</span><span class="sxs-lookup"><span data-stu-id="9a195-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookrange-visibleview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9a195-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a195-139">Response</span></span>
<span data-ttu-id="9a195-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9a195-140">Here is an example of the response.</span></span> <span data-ttu-id="9a195-141">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9a195-141">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeView"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 194

{
  "cellAddresses": "cellAddresses-value",
  "columnCount": 99,
  "formulas": "formulas-value",
  "formulasLocal": "formulasLocal-value",
  "formulasR1C1": "formulasR1C1-value",
  "index": 99
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

