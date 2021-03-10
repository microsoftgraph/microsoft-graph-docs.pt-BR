---
title: 'workbookPivotTable: atualizar'
description: Atualiza a Tabela Dinâmica.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: fbbeb36dbd78538e1a23a3d007f355205450a90e
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50577643"
---
# <a name="workbookpivottable-refresh"></a><span data-ttu-id="05838-103">workbookPivotTable: atualizar</span><span class="sxs-lookup"><span data-stu-id="05838-103">workbookPivotTable: refresh</span></span>

<span data-ttu-id="05838-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05838-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="05838-105">Atualiza a Tabela Dinâmica.</span><span class="sxs-lookup"><span data-stu-id="05838-105">Refreshes the PivotTable.</span></span>


## <a name="permissions"></a><span data-ttu-id="05838-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="05838-106">Permissions</span></span>
<span data-ttu-id="05838-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05838-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="05838-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="05838-109">Permission type</span></span>      | <span data-ttu-id="05838-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="05838-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="05838-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="05838-111">Delegated (work or school account)</span></span> | <span data-ttu-id="05838-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="05838-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="05838-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="05838-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="05838-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="05838-114">Not supported.</span></span>    |
|<span data-ttu-id="05838-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="05838-115">Application</span></span> | <span data-ttu-id="05838-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="05838-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="05838-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="05838-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/worksheets/{id}/pivotTables/{id}/refresh
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id}/pivotTables/{id}/refresh
```
## <a name="request-headers"></a><span data-ttu-id="05838-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="05838-118">Request headers</span></span>
| <span data-ttu-id="05838-119">Nome</span><span class="sxs-lookup"><span data-stu-id="05838-119">Name</span></span>       | <span data-ttu-id="05838-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="05838-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="05838-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="05838-121">Authorization</span></span>  | <span data-ttu-id="05838-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="05838-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="05838-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="05838-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="05838-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="05838-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="05838-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="05838-127">Request body</span></span>

### <a name="response"></a><span data-ttu-id="05838-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="05838-128">Response</span></span>
<span data-ttu-id="05838-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="05838-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05838-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="05838-131">Example</span></span>
<span data-ttu-id="05838-132">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="05838-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="05838-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="05838-133">Request</span></span>
<span data-ttu-id="05838-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="05838-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="05838-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="05838-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refresh"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/pivotTables/{id}/refresh
```
# <a name="c"></a>[<span data-ttu-id="05838-136">C#</span><span class="sxs-lookup"><span data-stu-id="05838-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookpivottable-refresh-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="05838-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="05838-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookpivottable-refresh-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="05838-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="05838-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookpivottable-refresh-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="05838-139">Java</span><span class="sxs-lookup"><span data-stu-id="05838-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookpivottable-refresh-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="05838-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="05838-140">Response</span></span>
<span data-ttu-id="05838-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="05838-141">Here is an example of the response.</span></span>
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

