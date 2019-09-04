---
title: 'workbookRange: visibleView'
description: Uma das seguintes permissões é necessária para chamar esta API. Para saber mais, incluindo como escolher permissões, confira Permissões.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: c2df35a9c34a69b028bbeb02da04cd9258df72fb
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36728913"
---
# <a name="workbookrange-visibleview"></a><span data-ttu-id="dd903-104">workbookRange: visibleView</span><span class="sxs-lookup"><span data-stu-id="dd903-104">workbookRange: visibleView</span></span>


## <a name="permissions"></a><span data-ttu-id="dd903-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="dd903-105">Permissions</span></span>
<span data-ttu-id="dd903-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd903-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd903-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dd903-108">Permission type</span></span>      | <span data-ttu-id="dd903-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dd903-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dd903-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dd903-110">Delegated (work or school account)</span></span> | <span data-ttu-id="dd903-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dd903-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dd903-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dd903-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd903-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dd903-113">Not supported.</span></span>    |
|<span data-ttu-id="dd903-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dd903-114">Application</span></span> | <span data-ttu-id="dd903-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dd903-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dd903-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dd903-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root/workbook/worksheets/{id}/range(address={address})/visibleView
```
## <a name="request-headers"></a><span data-ttu-id="dd903-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dd903-117">Request headers</span></span>
| <span data-ttu-id="dd903-118">Nome</span><span class="sxs-lookup"><span data-stu-id="dd903-118">Name</span></span>       | <span data-ttu-id="dd903-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd903-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="dd903-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="dd903-120">Authorization</span></span>  | <span data-ttu-id="dd903-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dd903-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dd903-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="dd903-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="dd903-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="dd903-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd903-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dd903-126">Request body</span></span>

### <a name="response"></a><span data-ttu-id="dd903-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd903-127">Response</span></span>
<span data-ttu-id="dd903-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRangeView](../resources/workbookrangeview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dd903-128">If successful, this method returns `200 OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd903-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dd903-129">Example</span></span>
<span data-ttu-id="dd903-130">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="dd903-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="dd903-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dd903-131">Request</span></span>
<span data-ttu-id="dd903-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dd903-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="dd903-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="dd903-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "workbookrange_visibleview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dd903-134">C#</span><span class="sxs-lookup"><span data-stu-id="dd903-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrange-visibleview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dd903-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dd903-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrange-visibleview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dd903-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="dd903-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrange-visibleview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="dd903-137">Java</span><span class="sxs-lookup"><span data-stu-id="dd903-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookrange-visibleview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="dd903-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd903-138">Response</span></span>
<span data-ttu-id="dd903-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dd903-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
