---
title: 'TableSort: clear'
description: Limpa a classificação que está na tabela. Essa ação não modifica a ordenação da tabela, mas limpa o estado dos botões do cabeçalho.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 2dfac7c82d0ebe06c159e7675b46a96a07daf497
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36316246"
---
# <a name="tablesort-clear"></a><span data-ttu-id="34b57-104">TableSort: clear</span><span class="sxs-lookup"><span data-stu-id="34b57-104">TableSort: clear</span></span>

<span data-ttu-id="34b57-p102">Limpa a classificação que está na tabela. Essa ação não modifica a ordenação da tabela, mas limpa o estado dos botões do cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="34b57-p102">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>
## <a name="permissions"></a><span data-ttu-id="34b57-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="34b57-107">Permissions</span></span>
<span data-ttu-id="34b57-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34b57-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34b57-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="34b57-110">Permission type</span></span>      | <span data-ttu-id="34b57-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="34b57-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="34b57-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="34b57-112">Delegated (work or school account)</span></span> | <span data-ttu-id="34b57-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34b57-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="34b57-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="34b57-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34b57-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34b57-115">Not supported.</span></span>    |
|<span data-ttu-id="34b57-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="34b57-116">Application</span></span> | <span data-ttu-id="34b57-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34b57-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="34b57-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="34b57-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/clear

```
## <a name="request-headers"></a><span data-ttu-id="34b57-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="34b57-119">Request headers</span></span>
| <span data-ttu-id="34b57-120">Nome</span><span class="sxs-lookup"><span data-stu-id="34b57-120">Name</span></span>       | <span data-ttu-id="34b57-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="34b57-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="34b57-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="34b57-122">Authorization</span></span>  | <span data-ttu-id="34b57-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="34b57-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="34b57-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="34b57-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="34b57-p105">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="34b57-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="34b57-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="34b57-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="34b57-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="34b57-129">Response</span></span>

<span data-ttu-id="34b57-p106">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="34b57-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34b57-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="34b57-132">Example</span></span>
<span data-ttu-id="34b57-133">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="34b57-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="34b57-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="34b57-134">Request</span></span>
<span data-ttu-id="34b57-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="34b57-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="34b57-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="34b57-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tablesort_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/clear
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="34b57-137">C#</span><span class="sxs-lookup"><span data-stu-id="34b57-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablesort-clear-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="34b57-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="34b57-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablesort-clear-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="34b57-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="34b57-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablesort-clear-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="34b57-140">Java</span><span class="sxs-lookup"><span data-stu-id="34b57-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tablesort-clear-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="34b57-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="34b57-141">Response</span></span>
<span data-ttu-id="34b57-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="34b57-142">Here is an example of the response.</span></span> 
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
  "description": "TableSort: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
