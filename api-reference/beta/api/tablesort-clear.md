---
title: 'TableSort: clear'
description: Limpa a classificação que está na tabela. Essa ação não modifica a ordenação da tabela, mas limpa o estado dos botões do cabeçalho.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 7d8db91751092a331b497b8fce29dbcb67d2131d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452635"
---
# <a name="tablesort-clear"></a><span data-ttu-id="49bc6-104">TableSort: clear</span><span class="sxs-lookup"><span data-stu-id="49bc6-104">TableSort: clear</span></span>

<span data-ttu-id="49bc6-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="49bc6-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49bc6-p102">Limpa a classificação que está na tabela. Essa ação não modifica a ordenação da tabela, mas limpa o estado dos botões do cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="49bc6-p102">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>
## <a name="permissions"></a><span data-ttu-id="49bc6-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="49bc6-108">Permissions</span></span>
<span data-ttu-id="49bc6-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49bc6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49bc6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="49bc6-111">Permission type</span></span>      | <span data-ttu-id="49bc6-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="49bc6-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49bc6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="49bc6-113">Delegated (work or school account)</span></span> | <span data-ttu-id="49bc6-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="49bc6-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="49bc6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="49bc6-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49bc6-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="49bc6-116">Files.ReadWrite</span></span>    |
|<span data-ttu-id="49bc6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="49bc6-117">Application</span></span> | <span data-ttu-id="49bc6-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="49bc6-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="49bc6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="49bc6-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/clear

```
## <a name="request-headers"></a><span data-ttu-id="49bc6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="49bc6-120">Request headers</span></span>
| <span data-ttu-id="49bc6-121">Nome</span><span class="sxs-lookup"><span data-stu-id="49bc6-121">Name</span></span>       | <span data-ttu-id="49bc6-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="49bc6-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="49bc6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="49bc6-123">Authorization</span></span>  | <span data-ttu-id="49bc6-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="49bc6-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="49bc6-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="49bc6-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="49bc6-p105">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="49bc6-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="49bc6-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="49bc6-129">Request body</span></span>

## <a name="response"></a><span data-ttu-id="49bc6-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="49bc6-130">Response</span></span>

<span data-ttu-id="49bc6-p106">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="49bc6-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49bc6-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="49bc6-133">Example</span></span>
<span data-ttu-id="49bc6-134">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="49bc6-134">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="49bc6-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="49bc6-135">Request</span></span>
<span data-ttu-id="49bc6-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="49bc6-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="49bc6-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="49bc6-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tablesort_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/sort/clear
```
# <a name="c"></a>[<span data-ttu-id="49bc6-138">C#</span><span class="sxs-lookup"><span data-stu-id="49bc6-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablesort-clear-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="49bc6-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="49bc6-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablesort-clear-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="49bc6-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="49bc6-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablesort-clear-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="49bc6-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="49bc6-141">Response</span></span>
<span data-ttu-id="49bc6-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="49bc6-142">Here is an example of the response.</span></span> 
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
<!--
{
  "type": "#page.annotation",
  "description": "TableSort: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
