---
title: 'workbookRange: visibleView'
description: Uma das seguintes permissões é necessária para chamar essa API. Para saber mais, incluindo como escolher permissões, confira Permissões.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: b613f66e4da8b27753beca46580e866a432734ee
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50577475"
---
# <a name="workbookrange-visibleview"></a><span data-ttu-id="a2be1-104">workbookRange: visibleView</span><span class="sxs-lookup"><span data-stu-id="a2be1-104">workbookRange: visibleView</span></span>

<span data-ttu-id="a2be1-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2be1-105">Namespace: microsoft.graph</span></span>


## <a name="permissions"></a><span data-ttu-id="a2be1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a2be1-106">Permissions</span></span>
<span data-ttu-id="a2be1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2be1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2be1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a2be1-109">Permission type</span></span>      | <span data-ttu-id="a2be1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a2be1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a2be1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a2be1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a2be1-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a2be1-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a2be1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a2be1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2be1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a2be1-114">Not supported.</span></span>    |
|<span data-ttu-id="a2be1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a2be1-115">Application</span></span> | <span data-ttu-id="a2be1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a2be1-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a2be1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a2be1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets/{id}/range(address={address})/visibleView
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id}/range(address={address})/visibleView
```
## <a name="request-headers"></a><span data-ttu-id="a2be1-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a2be1-118">Request headers</span></span>
| <span data-ttu-id="a2be1-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a2be1-119">Name</span></span>       | <span data-ttu-id="a2be1-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2be1-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a2be1-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a2be1-121">Authorization</span></span>  | <span data-ttu-id="a2be1-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a2be1-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a2be1-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a2be1-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="a2be1-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="a2be1-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2be1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a2be1-127">Request body</span></span>

### <a name="response"></a><span data-ttu-id="a2be1-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2be1-128">Response</span></span>
<span data-ttu-id="a2be1-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRangeView](../resources/workbookrangeview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a2be1-129">If successful, this method returns `200 OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2be1-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a2be1-130">Example</span></span>
<span data-ttu-id="a2be1-131">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="a2be1-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a2be1-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a2be1-132">Request</span></span>
<span data-ttu-id="a2be1-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a2be1-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a2be1-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="a2be1-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "workbookrange_visibleview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView
```
# <a name="c"></a>[<span data-ttu-id="a2be1-135">C#</span><span class="sxs-lookup"><span data-stu-id="a2be1-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrange-visibleview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a2be1-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a2be1-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrange-visibleview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a2be1-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a2be1-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrange-visibleview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a2be1-138">Java</span><span class="sxs-lookup"><span data-stu-id="a2be1-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookrange-visibleview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a2be1-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2be1-139">Response</span></span>
<span data-ttu-id="a2be1-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a2be1-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

