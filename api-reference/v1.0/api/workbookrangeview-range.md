---
title: 'workbookRangeView: intervalo'
description: Retorne o intervalo associado com o recurso rangeView.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 71c2a27326d67adf25268717af5e927ac6f88570
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36026304"
---
# <a name="workbookrangeview-range"></a><span data-ttu-id="eab36-103">workbookRangeView: intervalo</span><span class="sxs-lookup"><span data-stu-id="eab36-103">workbookRangeView: range</span></span>
<span data-ttu-id="eab36-104">Retorne o intervalo associado com o recurso rangeView.</span><span class="sxs-lookup"><span data-stu-id="eab36-104">Return the range associated with the rangeView resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="eab36-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="eab36-105">Permissions</span></span>
<span data-ttu-id="eab36-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eab36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="eab36-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eab36-108">Permission type</span></span>      | <span data-ttu-id="eab36-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eab36-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eab36-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eab36-110">Delegated (work or school account)</span></span> | <span data-ttu-id="eab36-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eab36-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="eab36-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eab36-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eab36-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eab36-113">Not supported.</span></span>    |
|<span data-ttu-id="eab36-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eab36-114">Application</span></span> | <span data-ttu-id="eab36-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eab36-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="eab36-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eab36-116">HTTP request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="eab36-117">HTTP</span><span class="sxs-lookup"><span data-stu-id="eab36-117">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(address={address})/visibleView/range

```
## <a name="request-headers"></a><span data-ttu-id="eab36-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eab36-118">Request headers</span></span>
| <span data-ttu-id="eab36-119">Nome</span><span class="sxs-lookup"><span data-stu-id="eab36-119">Name</span></span>       | <span data-ttu-id="eab36-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="eab36-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="eab36-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="eab36-121">Authorization</span></span>  | <span data-ttu-id="eab36-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eab36-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="eab36-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="eab36-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="eab36-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="eab36-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="eab36-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eab36-127">Request body</span></span>

### <a name="response"></a><span data-ttu-id="eab36-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="eab36-128">Response</span></span>
<span data-ttu-id="eab36-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eab36-129">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eab36-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eab36-130">Example</span></span>
<span data-ttu-id="eab36-131">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="eab36-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="eab36-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eab36-132">Request</span></span>
<span data-ttu-id="eab36-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eab36-133">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrangeview_range"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView/range
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="eab36-134">C#</span><span class="sxs-lookup"><span data-stu-id="eab36-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrangeview-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="eab36-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="eab36-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrangeview-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="eab36-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="eab36-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrangeview-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="eab36-137">Java</span><span class="sxs-lookup"><span data-stu-id="eab36-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookrangeview-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="eab36-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="eab36-138">Response</span></span>
<span data-ttu-id="eab36-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eab36-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
