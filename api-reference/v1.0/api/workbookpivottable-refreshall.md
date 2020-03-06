---
title: 'workbookPivotTable: refreshAll'
description: Atualiza a tabela dinâmica dentro de uma determinada planilha.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: adc5da1c3b1334e593e6f7ef3affa8c711aece98
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508769"
---
# <a name="workbookpivottable-refreshall"></a><span data-ttu-id="830c8-103">workbookPivotTable: refreshAll</span><span class="sxs-lookup"><span data-stu-id="830c8-103">workbookPivotTable: refreshAll</span></span>

<span data-ttu-id="830c8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="830c8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="830c8-105">Atualiza a tabela dinâmica dentro de uma determinada planilha.</span><span class="sxs-lookup"><span data-stu-id="830c8-105">Refreshes the PivotTable within a given worksheet.</span></span>

## <a name="permissions"></a><span data-ttu-id="830c8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="830c8-106">Permissions</span></span>
<span data-ttu-id="830c8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="830c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="830c8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="830c8-109">Permission type</span></span>      | <span data-ttu-id="830c8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="830c8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="830c8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="830c8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="830c8-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="830c8-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="830c8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="830c8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="830c8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="830c8-114">Not supported.</span></span>    |
|<span data-ttu-id="830c8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="830c8-115">Application</span></span> | <span data-ttu-id="830c8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="830c8-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="830c8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="830c8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll

```
## <a name="request-headers"></a><span data-ttu-id="830c8-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="830c8-118">Request headers</span></span>
| <span data-ttu-id="830c8-119">Nome</span><span class="sxs-lookup"><span data-stu-id="830c8-119">Name</span></span>       | <span data-ttu-id="830c8-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="830c8-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="830c8-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="830c8-121">Authorization</span></span>  | <span data-ttu-id="830c8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="830c8-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="830c8-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="830c8-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="830c8-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="830c8-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="830c8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="830c8-127">Request body</span></span>

### <a name="response"></a><span data-ttu-id="830c8-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="830c8-128">Response</span></span>
<span data-ttu-id="830c8-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="830c8-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="830c8-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="830c8-131">Example</span></span>
<span data-ttu-id="830c8-132">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="830c8-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="830c8-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="830c8-133">Request</span></span>
<span data-ttu-id="830c8-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="830c8-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="830c8-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="830c8-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refreshall"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll
```
# <a name="c"></a>[<span data-ttu-id="830c8-136">C#</span><span class="sxs-lookup"><span data-stu-id="830c8-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookpivottable-refreshall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="830c8-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="830c8-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookpivottable-refreshall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="830c8-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="830c8-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookpivottable-refreshall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="830c8-139">Java</span><span class="sxs-lookup"><span data-stu-id="830c8-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookpivottable-refreshall-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="830c8-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="830c8-140">Response</span></span>
<span data-ttu-id="830c8-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="830c8-141">Here is an example of the response.</span></span>
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
