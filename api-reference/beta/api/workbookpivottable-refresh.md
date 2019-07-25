---
title: 'workbookPivotTable: atualizar'
description: Atualiza a Tabela Dinâmica.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: ff537d8a00f3893a78fb6fbd0c19ad9deac3ae8e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35866442"
---
# <a name="workbookpivottable-refresh"></a><span data-ttu-id="33f3f-103">workbookPivotTable: atualizar</span><span class="sxs-lookup"><span data-stu-id="33f3f-103">workbookPivotTable: refresh</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33f3f-104">Atualiza a Tabela Dinâmica.</span><span class="sxs-lookup"><span data-stu-id="33f3f-104">Refreshes the PivotTable.</span></span>


## <a name="permissions"></a><span data-ttu-id="33f3f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="33f3f-105">Permissions</span></span>
<span data-ttu-id="33f3f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33f3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="33f3f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="33f3f-108">Permission type</span></span>      | <span data-ttu-id="33f3f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="33f3f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="33f3f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="33f3f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="33f3f-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="33f3f-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="33f3f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="33f3f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33f3f-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="33f3f-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="33f3f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="33f3f-114">Application</span></span> | <span data-ttu-id="33f3f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="33f3f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="33f3f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="33f3f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/pivotTables/{id}/refresh
```
## <a name="request-headers"></a><span data-ttu-id="33f3f-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="33f3f-117">Request headers</span></span>
| <span data-ttu-id="33f3f-118">Nome</span><span class="sxs-lookup"><span data-stu-id="33f3f-118">Name</span></span>       | <span data-ttu-id="33f3f-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="33f3f-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="33f3f-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="33f3f-120">Authorization</span></span>  | <span data-ttu-id="33f3f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="33f3f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="33f3f-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="33f3f-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="33f3f-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="33f3f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="33f3f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="33f3f-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="33f3f-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="33f3f-127">Response</span></span>

<span data-ttu-id="33f3f-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="33f3f-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33f3f-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="33f3f-130">Example</span></span>
<span data-ttu-id="33f3f-131">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="33f3f-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="33f3f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="33f3f-132">Request</span></span>
<span data-ttu-id="33f3f-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="33f3f-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="33f3f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="33f3f-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refresh"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/pivotTables/{id}/refresh
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="33f3f-135">C#</span><span class="sxs-lookup"><span data-stu-id="33f3f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookpivottable-refresh-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="33f3f-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="33f3f-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookpivottable-refresh-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="33f3f-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="33f3f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookpivottable-refresh-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="33f3f-138">Java</span><span class="sxs-lookup"><span data-stu-id="33f3f-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookpivottable-refresh-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="33f3f-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="33f3f-139">Response</span></span>
<span data-ttu-id="33f3f-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="33f3f-140">Here is an example of the response.</span></span>
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
