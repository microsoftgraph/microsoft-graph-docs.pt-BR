---
title: 'workbookRangeView: intervalo'
description: Retorne o intervalo associado com o recurso rangeView.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 197a2e7142836637c3d7156b1c3f1b83313a68ab
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33600619"
---
# <a name="workbookrangeview-range"></a><span data-ttu-id="80cf6-103">workbookRangeView: intervalo</span><span class="sxs-lookup"><span data-stu-id="80cf6-103">workbookRangeView: range</span></span>
<span data-ttu-id="80cf6-104">Retorne o intervalo associado com o recurso rangeView.</span><span class="sxs-lookup"><span data-stu-id="80cf6-104">Return the range associated with the rangeView resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="80cf6-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="80cf6-105">Permissions</span></span>
<span data-ttu-id="80cf6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80cf6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="80cf6-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="80cf6-108">Permission type</span></span>      | <span data-ttu-id="80cf6-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="80cf6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="80cf6-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="80cf6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="80cf6-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="80cf6-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="80cf6-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="80cf6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80cf6-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="80cf6-113">Not supported.</span></span>    |
|<span data-ttu-id="80cf6-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="80cf6-114">Application</span></span> | <span data-ttu-id="80cf6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="80cf6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="80cf6-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="80cf6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(address={address})/visibleView/range

```
## <a name="request-headers"></a><span data-ttu-id="80cf6-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="80cf6-117">Request headers</span></span>
| <span data-ttu-id="80cf6-118">Nome</span><span class="sxs-lookup"><span data-stu-id="80cf6-118">Name</span></span>       | <span data-ttu-id="80cf6-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="80cf6-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="80cf6-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="80cf6-120">Authorization</span></span>  | <span data-ttu-id="80cf6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="80cf6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="80cf6-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="80cf6-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="80cf6-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="80cf6-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="80cf6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="80cf6-126">Request body</span></span>

### <a name="response"></a><span data-ttu-id="80cf6-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="80cf6-127">Response</span></span>
<span data-ttu-id="80cf6-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="80cf6-128">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80cf6-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="80cf6-129">Example</span></span>
<span data-ttu-id="80cf6-130">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="80cf6-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="80cf6-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="80cf6-131">Request</span></span>
<span data-ttu-id="80cf6-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="80cf6-132">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrangeview_range"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView/range
```

##### <a name="response"></a><span data-ttu-id="80cf6-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="80cf6-133">Response</span></span>
<span data-ttu-id="80cf6-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="80cf6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="80cf6-137">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="80cf6-137">SDK sample code</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="80cf6-138">Basic</span><span class="sxs-lookup"><span data-stu-id="80cf6-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/workbookrangeview_range-Cs-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/workbookrangeview-range.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/workbookrangeview-range.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
