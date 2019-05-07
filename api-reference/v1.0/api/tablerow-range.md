---
title: 'TableRow: Range'
description: Retorna o objeto de intervalo associado a toda a linha.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: da47add9d566be4e9ccca926ecb12f968fefa1bd
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33602484"
---
# <a name="tablerow-range"></a><span data-ttu-id="c2953-103">TableRow: Range</span><span class="sxs-lookup"><span data-stu-id="c2953-103">TableRow: Range</span></span>

<span data-ttu-id="c2953-104">Retorna o objeto de intervalo associado a toda a linha.</span><span class="sxs-lookup"><span data-stu-id="c2953-104">Returns the range object associated with the entire row.</span></span>
## <a name="permissions"></a><span data-ttu-id="c2953-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c2953-105">Permissions</span></span>
<span data-ttu-id="c2953-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2953-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2953-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c2953-108">Permission type</span></span>      | <span data-ttu-id="c2953-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c2953-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2953-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c2953-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c2953-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c2953-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c2953-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c2953-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2953-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c2953-113">Not supported.</span></span>    |
|<span data-ttu-id="c2953-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c2953-114">Application</span></span> | <span data-ttu-id="c2953-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c2953-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c2953-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c2953-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/rows/{index}/range
GET /workbook/worksheets/{id|name}/tables/{id|name}/rows/{index}/range

```
## <a name="request-headers"></a><span data-ttu-id="c2953-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c2953-117">Request headers</span></span>
| <span data-ttu-id="c2953-118">Nome</span><span class="sxs-lookup"><span data-stu-id="c2953-118">Name</span></span>       | <span data-ttu-id="c2953-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2953-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c2953-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="c2953-120">Authorization</span></span>  | <span data-ttu-id="c2953-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c2953-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c2953-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c2953-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="c2953-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="c2953-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2953-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c2953-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="c2953-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2953-127">Response</span></span>

<span data-ttu-id="c2953-128">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c2953-128">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2953-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c2953-129">Example</span></span>
<span data-ttu-id="c2953-130">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="c2953-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c2953-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c2953-131">Request</span></span>
<span data-ttu-id="c2953-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c2953-132">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "tablerow_range"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows/{index}/range
```

##### <a name="response"></a><span data-ttu-id="c2953-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2953-133">Response</span></span>
<span data-ttu-id="c2953-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c2953-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="c2953-137">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="c2953-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c2953-138">Basic</span><span class="sxs-lookup"><span data-stu-id="c2953-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/tablerow_range-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c2953-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c2953-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/tablerow_range-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableRow: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/tablerow-range.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/tablerow-range.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
