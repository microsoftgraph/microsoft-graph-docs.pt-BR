---
title: 'workbookPivotTable: refreshAll'
description: Atualiza a tabela dinâmica dentro de uma determinada planilha.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 85099e87d6c92fdb4bdaf304dde431a31c89e225
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35459850"
---
# <a name="workbookpivottable-refreshall"></a><span data-ttu-id="fb996-103">workbookPivotTable: refreshAll</span><span class="sxs-lookup"><span data-stu-id="fb996-103">workbookPivotTable: refreshAll</span></span>

<span data-ttu-id="fb996-104">Atualiza a tabela dinâmica dentro de uma determinada planilha.</span><span class="sxs-lookup"><span data-stu-id="fb996-104">Refreshes the PivotTable within a given worksheet.</span></span>

## <a name="permissions"></a><span data-ttu-id="fb996-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="fb996-105">Permissions</span></span>
<span data-ttu-id="fb996-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb996-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb996-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fb996-108">Permission type</span></span>      | <span data-ttu-id="fb996-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fb996-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fb996-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fb996-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fb996-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fb996-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fb996-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fb996-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb996-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fb996-113">Not supported.</span></span>    |
|<span data-ttu-id="fb996-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fb996-114">Application</span></span> | <span data-ttu-id="fb996-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fb996-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fb996-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fb996-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll

```
## <a name="request-headers"></a><span data-ttu-id="fb996-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fb996-117">Request headers</span></span>
| <span data-ttu-id="fb996-118">Nome</span><span class="sxs-lookup"><span data-stu-id="fb996-118">Name</span></span>       | <span data-ttu-id="fb996-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb996-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fb996-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="fb996-120">Authorization</span></span>  | <span data-ttu-id="fb996-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fb996-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fb996-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="fb996-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="fb996-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="fb996-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb996-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fb996-126">Request body</span></span>

### <a name="response"></a><span data-ttu-id="fb996-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb996-127">Response</span></span>
<span data-ttu-id="fb996-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fb996-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb996-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fb996-130">Example</span></span>
<span data-ttu-id="fb996-131">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="fb996-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fb996-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb996-132">Request</span></span>
<span data-ttu-id="fb996-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fb996-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fb996-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="fb996-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refreshall"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fb996-135">C#</span><span class="sxs-lookup"><span data-stu-id="fb996-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookpivottable-refreshall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fb996-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="fb996-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookpivottable-refreshall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fb996-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="fb996-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookpivottable-refreshall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="fb996-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb996-138">Response</span></span>
<span data-ttu-id="fb996-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fb996-139">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
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
