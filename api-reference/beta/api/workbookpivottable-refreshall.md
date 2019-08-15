---
title: 'workbookPivotTable: refreshAll'
description: Atualiza a tabela dinâmica dentro de uma determinada planilha.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: d6b591f3a6dc7a9e18133a1005adf4f5f625c517
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36421593"
---
# <a name="workbookpivottable-refreshall"></a><span data-ttu-id="a2c1d-103">workbookPivotTable: refreshAll</span><span class="sxs-lookup"><span data-stu-id="a2c1d-103">workbookPivotTable: refreshAll</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2c1d-104">Atualiza a tabela dinâmica dentro de uma determinada planilha.</span><span class="sxs-lookup"><span data-stu-id="a2c1d-104">Refreshes the PivotTable within a given worksheet.</span></span>

## <a name="permissions"></a><span data-ttu-id="a2c1d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a2c1d-105">Permissions</span></span>
<span data-ttu-id="a2c1d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2c1d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2c1d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a2c1d-108">Permission type</span></span>      | <span data-ttu-id="a2c1d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a2c1d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a2c1d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a2c1d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a2c1d-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a2c1d-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a2c1d-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a2c1d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2c1d-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a2c1d-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a2c1d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a2c1d-114">Application</span></span> | <span data-ttu-id="a2c1d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a2c1d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a2c1d-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a2c1d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll

```
## <a name="request-headers"></a><span data-ttu-id="a2c1d-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a2c1d-117">Request headers</span></span>
| <span data-ttu-id="a2c1d-118">Nome</span><span class="sxs-lookup"><span data-stu-id="a2c1d-118">Name</span></span>       | <span data-ttu-id="a2c1d-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2c1d-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a2c1d-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="a2c1d-120">Authorization</span></span>  | <span data-ttu-id="a2c1d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a2c1d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a2c1d-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a2c1d-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="a2c1d-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="a2c1d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2c1d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a2c1d-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="a2c1d-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2c1d-127">Response</span></span>

<span data-ttu-id="a2c1d-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a2c1d-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2c1d-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a2c1d-130">Example</span></span>
<span data-ttu-id="a2c1d-131">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="a2c1d-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a2c1d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a2c1d-132">Request</span></span>
<span data-ttu-id="a2c1d-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a2c1d-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a2c1d-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="a2c1d-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refreshall"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a2c1d-135">C#</span><span class="sxs-lookup"><span data-stu-id="a2c1d-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookpivottable-refreshall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a2c1d-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a2c1d-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookpivottable-refreshall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a2c1d-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a2c1d-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookpivottable-refreshall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a2c1d-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2c1d-138">Response</span></span>
<span data-ttu-id="a2c1d-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a2c1d-139">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
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
