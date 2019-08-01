---
title: 'TableSort: clear'
description: Limpa a classificação que está na tabela. Essa ação não modifica a ordenação da tabela, mas limpa o estado dos botões do cabeçalho.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 39cc8f742da7a31edc45d3e0edb172b86e88ab11
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36024292"
---
# <a name="tablesort-clear"></a><span data-ttu-id="7dd2a-104">TableSort: clear</span><span class="sxs-lookup"><span data-stu-id="7dd2a-104">TableSort: clear</span></span>

<span data-ttu-id="7dd2a-p102">Limpa a classificação que está na tabela. Essa ação não modifica a ordenação da tabela, mas limpa o estado dos botões do cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="7dd2a-p102">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>
## <a name="permissions"></a><span data-ttu-id="7dd2a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="7dd2a-107">Permissions</span></span>
<span data-ttu-id="7dd2a-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7dd2a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7dd2a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7dd2a-110">Permission type</span></span>      | <span data-ttu-id="7dd2a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7dd2a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7dd2a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7dd2a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7dd2a-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7dd2a-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7dd2a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7dd2a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7dd2a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7dd2a-115">Not supported.</span></span>    |
|<span data-ttu-id="7dd2a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7dd2a-116">Application</span></span> | <span data-ttu-id="7dd2a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7dd2a-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7dd2a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7dd2a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/clear

```
## <a name="request-headers"></a><span data-ttu-id="7dd2a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7dd2a-119">Request headers</span></span>
| <span data-ttu-id="7dd2a-120">Nome</span><span class="sxs-lookup"><span data-stu-id="7dd2a-120">Name</span></span>       | <span data-ttu-id="7dd2a-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="7dd2a-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7dd2a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7dd2a-122">Authorization</span></span>  | <span data-ttu-id="7dd2a-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7dd2a-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7dd2a-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7dd2a-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="7dd2a-p105">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="7dd2a-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7dd2a-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7dd2a-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="7dd2a-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="7dd2a-129">Response</span></span>

<span data-ttu-id="7dd2a-p106">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7dd2a-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7dd2a-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7dd2a-132">Example</span></span>
<span data-ttu-id="7dd2a-133">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="7dd2a-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7dd2a-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7dd2a-134">Request</span></span>
<span data-ttu-id="7dd2a-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7dd2a-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7dd2a-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="7dd2a-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tablesort_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/clear
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7dd2a-137">C#</span><span class="sxs-lookup"><span data-stu-id="7dd2a-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablesort-clear-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7dd2a-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="7dd2a-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablesort-clear-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7dd2a-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="7dd2a-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablesort-clear-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7dd2a-140">Java</span><span class="sxs-lookup"><span data-stu-id="7dd2a-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tablesort-clear-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7dd2a-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="7dd2a-141">Response</span></span>
<span data-ttu-id="7dd2a-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7dd2a-142">Here is an example of the response.</span></span> 
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
