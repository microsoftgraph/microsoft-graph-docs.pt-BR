---
title: 'TableSort: clear'
description: Limpa a classificação que está na tabela. Essa ação não modifica a ordenação da tabela, mas limpa o estado dos botões do cabeçalho.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: f6ee185d8d2375409b7e11a9dbfef7e5d8944087
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271789"
---
# <a name="tablesort-clear"></a><span data-ttu-id="f7dde-104">TableSort: clear</span><span class="sxs-lookup"><span data-stu-id="f7dde-104">TableSort: clear</span></span>

<span data-ttu-id="f7dde-p102">Limpa a classificação que está na tabela. Essa ação não modifica a ordenação da tabela, mas limpa o estado dos botões do cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="f7dde-p102">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>
## <a name="permissions"></a><span data-ttu-id="f7dde-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f7dde-107">Permissions</span></span>
<span data-ttu-id="f7dde-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7dde-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7dde-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f7dde-110">Permission type</span></span>      | <span data-ttu-id="f7dde-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f7dde-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7dde-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f7dde-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f7dde-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f7dde-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f7dde-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f7dde-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7dde-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7dde-115">Not supported.</span></span>    |
|<span data-ttu-id="f7dde-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f7dde-116">Application</span></span> | <span data-ttu-id="f7dde-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7dde-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7dde-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f7dde-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/clear

```
## <a name="request-headers"></a><span data-ttu-id="f7dde-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f7dde-119">Request headers</span></span>
| <span data-ttu-id="f7dde-120">Nome</span><span class="sxs-lookup"><span data-stu-id="f7dde-120">Name</span></span>       | <span data-ttu-id="f7dde-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7dde-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f7dde-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f7dde-122">Authorization</span></span>  | <span data-ttu-id="f7dde-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f7dde-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f7dde-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f7dde-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="f7dde-p105">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="f7dde-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7dde-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f7dde-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="f7dde-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7dde-129">Response</span></span>

<span data-ttu-id="f7dde-p106">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f7dde-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7dde-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f7dde-132">Example</span></span>
<span data-ttu-id="f7dde-133">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="f7dde-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f7dde-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f7dde-134">Request</span></span>
<span data-ttu-id="f7dde-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f7dde-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablesort_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/clear
```

##### <a name="response"></a><span data-ttu-id="f7dde-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7dde-136">Response</span></span>
<span data-ttu-id="f7dde-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f7dde-137">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f7dde-138">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="f7dde-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f7dde-139">C#</span><span class="sxs-lookup"><span data-stu-id="f7dde-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/tablesort_clear-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f7dde-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="f7dde-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/tablesort_clear-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="f7dde-141">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="f7dde-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/tablesort_clear-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableSort: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/tablesort-clear.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/tablesort-clear.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/tablesort-clear.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
