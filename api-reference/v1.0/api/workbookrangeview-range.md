---
title: 'workbookRangeView: intervalo'
description: Retorne o intervalo associado com o recurso rangeView.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: b01f354cc0ce909108a085a61d200c0517e724c0
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36727331"
---
# <a name="workbookrangeview-range"></a><span data-ttu-id="1f6fb-103">workbookRangeView: intervalo</span><span class="sxs-lookup"><span data-stu-id="1f6fb-103">workbookRangeView: range</span></span>
<span data-ttu-id="1f6fb-104">Retorne o intervalo associado com o recurso rangeView.</span><span class="sxs-lookup"><span data-stu-id="1f6fb-104">Return the range associated with the rangeView resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="1f6fb-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="1f6fb-105">Permissions</span></span>
<span data-ttu-id="1f6fb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f6fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1f6fb-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1f6fb-108">Permission type</span></span>      | <span data-ttu-id="1f6fb-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1f6fb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1f6fb-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1f6fb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1f6fb-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1f6fb-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1f6fb-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1f6fb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f6fb-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1f6fb-113">Not supported.</span></span>    |
|<span data-ttu-id="1f6fb-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1f6fb-114">Application</span></span> | <span data-ttu-id="1f6fb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1f6fb-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1f6fb-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1f6fb-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(address={address})/visibleView/range

```
## <a name="request-headers"></a><span data-ttu-id="1f6fb-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1f6fb-117">Request headers</span></span>
| <span data-ttu-id="1f6fb-118">Nome</span><span class="sxs-lookup"><span data-stu-id="1f6fb-118">Name</span></span>       | <span data-ttu-id="1f6fb-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f6fb-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1f6fb-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="1f6fb-120">Authorization</span></span>  | <span data-ttu-id="1f6fb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1f6fb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1f6fb-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="1f6fb-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="1f6fb-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="1f6fb-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f6fb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1f6fb-126">Request body</span></span>

### <a name="response"></a><span data-ttu-id="1f6fb-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f6fb-127">Response</span></span>
<span data-ttu-id="1f6fb-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1f6fb-128">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f6fb-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1f6fb-129">Example</span></span>
<span data-ttu-id="1f6fb-130">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="1f6fb-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1f6fb-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1f6fb-131">Request</span></span>
<span data-ttu-id="1f6fb-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1f6fb-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1f6fb-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="1f6fb-133">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrangeview_range"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView/range
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1f6fb-134">C#</span><span class="sxs-lookup"><span data-stu-id="1f6fb-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrangeview-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1f6fb-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1f6fb-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrangeview-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1f6fb-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="1f6fb-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrangeview-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1f6fb-137">Java</span><span class="sxs-lookup"><span data-stu-id="1f6fb-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookrangeview-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1f6fb-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f6fb-138">Response</span></span>
<span data-ttu-id="1f6fb-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1f6fb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
