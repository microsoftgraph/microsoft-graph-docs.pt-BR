---
title: 'workbookPivotTable: refreshAll'
description: Atualiza a tabela dinâmica dentro de uma determinada planilha.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 09373fe51dcd760702c0ad2aa5a6f09ae48f572e
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2019
ms.locfileid: "33961289"
---
# <a name="workbookpivottable-refreshall"></a><span data-ttu-id="b2b7a-103">workbookPivotTable: refreshAll</span><span class="sxs-lookup"><span data-stu-id="b2b7a-103">workbookPivotTable: refreshAll</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2b7a-104">Atualiza a tabela dinâmica dentro de uma determinada planilha.</span><span class="sxs-lookup"><span data-stu-id="b2b7a-104">Refreshes the PivotTable within a given worksheet.</span></span>

## <a name="permissions"></a><span data-ttu-id="b2b7a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b2b7a-105">Permissions</span></span>
<span data-ttu-id="b2b7a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2b7a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2b7a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b2b7a-108">Permission type</span></span>      | <span data-ttu-id="b2b7a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b2b7a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b2b7a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b2b7a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b2b7a-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b2b7a-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b2b7a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b2b7a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b2b7a-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b2b7a-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b2b7a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b2b7a-114">Application</span></span> | <span data-ttu-id="b2b7a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2b7a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b2b7a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b2b7a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll

```
## <a name="request-headers"></a><span data-ttu-id="b2b7a-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b2b7a-117">Request headers</span></span>
| <span data-ttu-id="b2b7a-118">Nome</span><span class="sxs-lookup"><span data-stu-id="b2b7a-118">Name</span></span>       | <span data-ttu-id="b2b7a-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2b7a-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b2b7a-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="b2b7a-120">Authorization</span></span>  | <span data-ttu-id="b2b7a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b2b7a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b2b7a-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b2b7a-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="b2b7a-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="b2b7a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2b7a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b2b7a-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="b2b7a-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2b7a-127">Response</span></span>

<span data-ttu-id="b2b7a-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b2b7a-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2b7a-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b2b7a-130">Example</span></span>
<span data-ttu-id="b2b7a-131">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="b2b7a-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b2b7a-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b2b7a-132">Request</span></span>
<span data-ttu-id="b2b7a-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b2b7a-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refreshall"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll
```

##### <a name="response"></a><span data-ttu-id="b2b7a-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2b7a-134">Response</span></span>
<span data-ttu-id="b2b7a-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b2b7a-135">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="b2b7a-136">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="b2b7a-136">SDK sample code</span></span>
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b2b7a-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="b2b7a-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/workbookpivottable_refreshall-Javascript-snippets.md)]

# <a name="ctabcs"></a>[<span data-ttu-id="b2b7a-138">C#</span><span class="sxs-lookup"><span data-stu-id="b2b7a-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/workbookpivottable_refreshall-Cs-snippets.md)]

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
    "Error: /api-reference/beta/api/workbookpivottable-refreshall.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/workbookpivottable-refreshall.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
