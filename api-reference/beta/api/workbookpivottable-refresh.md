---
title: 'workbookPivotTable: atualizar'
description: Atualiza a Tabela Dinâmica.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 523aecab7e17330f26142c19bf3df42d4c255c1d
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787706"
---
# <a name="workbookpivottable-refresh"></a><span data-ttu-id="186d0-103">workbookPivotTable: atualizar</span><span class="sxs-lookup"><span data-stu-id="186d0-103">workbookPivotTable: refresh</span></span>

<span data-ttu-id="186d0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="186d0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="186d0-105">Atualiza a Tabela Dinâmica.</span><span class="sxs-lookup"><span data-stu-id="186d0-105">Refreshes the PivotTable.</span></span>


## <a name="permissions"></a><span data-ttu-id="186d0-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="186d0-106">Permissions</span></span>
<span data-ttu-id="186d0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="186d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="186d0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="186d0-109">Permission type</span></span>      | <span data-ttu-id="186d0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="186d0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="186d0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="186d0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="186d0-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="186d0-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="186d0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="186d0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="186d0-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="186d0-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="186d0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="186d0-115">Application</span></span> | <span data-ttu-id="186d0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="186d0-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="186d0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="186d0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/worksheets/{id}/pivotTables/{id}/refresh
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id}/pivotTables/{id}/refresh
```
## <a name="request-headers"></a><span data-ttu-id="186d0-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="186d0-118">Request headers</span></span>
| <span data-ttu-id="186d0-119">Nome</span><span class="sxs-lookup"><span data-stu-id="186d0-119">Name</span></span>       | <span data-ttu-id="186d0-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="186d0-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="186d0-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="186d0-121">Authorization</span></span>  | <span data-ttu-id="186d0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="186d0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="186d0-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="186d0-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="186d0-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="186d0-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="186d0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="186d0-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="186d0-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="186d0-128">Response</span></span>

<span data-ttu-id="186d0-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="186d0-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="186d0-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="186d0-131">Example</span></span>
<span data-ttu-id="186d0-132">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="186d0-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="186d0-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="186d0-133">Request</span></span>
<span data-ttu-id="186d0-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="186d0-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="186d0-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="186d0-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refresh"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/pivotTables/{id}/refresh
```
# <a name="c"></a>[<span data-ttu-id="186d0-136">C#</span><span class="sxs-lookup"><span data-stu-id="186d0-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookpivottable-refresh-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="186d0-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="186d0-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookpivottable-refresh-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="186d0-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="186d0-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookpivottable-refresh-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="186d0-139">Java</span><span class="sxs-lookup"><span data-stu-id="186d0-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookpivottable-refresh-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="186d0-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="186d0-140">Response</span></span>
<span data-ttu-id="186d0-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="186d0-141">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response"
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


