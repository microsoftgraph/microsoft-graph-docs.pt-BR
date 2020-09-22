---
title: 'workbookPivotTable: atualizar'
description: Atualiza a Tabela Dinâmica.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 169ecaf459a43bbe645b5c720472196cfa1718b8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078504"
---
# <a name="workbookpivottable-refresh"></a><span data-ttu-id="a2234-103">workbookPivotTable: atualizar</span><span class="sxs-lookup"><span data-stu-id="a2234-103">workbookPivotTable: refresh</span></span>

<span data-ttu-id="a2234-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2234-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2234-105">Atualiza a Tabela Dinâmica.</span><span class="sxs-lookup"><span data-stu-id="a2234-105">Refreshes the PivotTable.</span></span>


## <a name="permissions"></a><span data-ttu-id="a2234-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a2234-106">Permissions</span></span>
<span data-ttu-id="a2234-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2234-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a2234-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a2234-109">Permission type</span></span>      | <span data-ttu-id="a2234-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a2234-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a2234-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a2234-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a2234-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a2234-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a2234-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a2234-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2234-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a2234-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a2234-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a2234-115">Application</span></span> | <span data-ttu-id="a2234-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a2234-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a2234-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a2234-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/pivotTables/{id}/refresh
```
## <a name="request-headers"></a><span data-ttu-id="a2234-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a2234-118">Request headers</span></span>
| <span data-ttu-id="a2234-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a2234-119">Name</span></span>       | <span data-ttu-id="a2234-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2234-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a2234-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a2234-121">Authorization</span></span>  | <span data-ttu-id="a2234-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a2234-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a2234-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a2234-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="a2234-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="a2234-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2234-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a2234-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="a2234-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2234-128">Response</span></span>

<span data-ttu-id="a2234-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a2234-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2234-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a2234-131">Example</span></span>
<span data-ttu-id="a2234-132">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="a2234-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a2234-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a2234-133">Request</span></span>
<span data-ttu-id="a2234-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a2234-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a2234-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="a2234-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refresh"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/pivotTables/{id}/refresh
```
# <a name="c"></a>[<span data-ttu-id="a2234-136">C#</span><span class="sxs-lookup"><span data-stu-id="a2234-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookpivottable-refresh-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a2234-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a2234-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookpivottable-refresh-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a2234-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a2234-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookpivottable-refresh-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a2234-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2234-139">Response</span></span>
<span data-ttu-id="a2234-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a2234-140">Here is an example of the response.</span></span>
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


