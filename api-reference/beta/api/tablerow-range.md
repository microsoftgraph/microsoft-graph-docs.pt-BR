---
title: 'TableRow: Range'
description: Retorna o objeto de intervalo associado a toda a linha.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 4d8786cdd812924cc857bdc02df3a557c0baedaf
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637707"
---
# <a name="tablerow-range"></a><span data-ttu-id="0b8c7-103">TableRow: Range</span><span class="sxs-lookup"><span data-stu-id="0b8c7-103">TableRow: Range</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b8c7-104">Retorna o objeto de intervalo associado a toda a linha.</span><span class="sxs-lookup"><span data-stu-id="0b8c7-104">Returns the range object associated with the entire row.</span></span>
## <a name="permissions"></a><span data-ttu-id="0b8c7-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0b8c7-105">Permissions</span></span>
<span data-ttu-id="0b8c7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b8c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b8c7-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0b8c7-108">Permission type</span></span>      | <span data-ttu-id="0b8c7-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0b8c7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b8c7-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0b8c7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0b8c7-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0b8c7-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0b8c7-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0b8c7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b8c7-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0b8c7-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0b8c7-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0b8c7-114">Application</span></span> | <span data-ttu-id="0b8c7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0b8c7-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0b8c7-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0b8c7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/{index}/Range
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/{index}/Range

```
## <a name="request-headers"></a><span data-ttu-id="0b8c7-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0b8c7-117">Request headers</span></span>
| <span data-ttu-id="0b8c7-118">Nome</span><span class="sxs-lookup"><span data-stu-id="0b8c7-118">Name</span></span>       | <span data-ttu-id="0b8c7-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b8c7-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0b8c7-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="0b8c7-120">Authorization</span></span>  | <span data-ttu-id="0b8c7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0b8c7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0b8c7-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0b8c7-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="0b8c7-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="0b8c7-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b8c7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0b8c7-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="0b8c7-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b8c7-127">Response</span></span>

<span data-ttu-id="0b8c7-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/workbookrange.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0b8c7-128">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b8c7-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0b8c7-129">Example</span></span>
<span data-ttu-id="0b8c7-130">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="0b8c7-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0b8c7-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0b8c7-131">Request</span></span>
<span data-ttu-id="0b8c7-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0b8c7-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablerow_range"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows/{index}/Range
```

##### <a name="response"></a><span data-ttu-id="0b8c7-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b8c7-133">Response</span></span>
<span data-ttu-id="0b8c7-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0b8c7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="0b8c7-137">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="0b8c7-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0b8c7-138">Basic</span><span class="sxs-lookup"><span data-stu-id="0b8c7-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/tablerow_range-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0b8c7-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b8c7-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/tablerow_range-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "TableRow: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/tablerow-range.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/tablerow-range.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
