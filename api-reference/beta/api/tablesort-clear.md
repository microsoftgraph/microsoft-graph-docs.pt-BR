---
title: 'TableSort: clear'
description: Limpa a classificação que está na tabela. Essa ação não modifica a ordenação da tabela, mas limpa o estado dos botões do cabeçalho.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 42577eef5fad03b74175f860cb9ea7b6a997d942
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786871"
---
# <a name="tablesort-clear"></a><span data-ttu-id="19eb8-104">TableSort: clear</span><span class="sxs-lookup"><span data-stu-id="19eb8-104">TableSort: clear</span></span>

<span data-ttu-id="19eb8-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19eb8-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19eb8-p102">Limpa a classificação que está na tabela. Essa ação não modifica a ordenação da tabela, mas limpa o estado dos botões do cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="19eb8-p102">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>
## <a name="permissions"></a><span data-ttu-id="19eb8-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="19eb8-108">Permissions</span></span>
<span data-ttu-id="19eb8-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19eb8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19eb8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="19eb8-111">Permission type</span></span>      | <span data-ttu-id="19eb8-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="19eb8-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="19eb8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="19eb8-113">Delegated (work or school account)</span></span> | <span data-ttu-id="19eb8-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19eb8-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="19eb8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="19eb8-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19eb8-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19eb8-116">Files.ReadWrite</span></span>    |
|<span data-ttu-id="19eb8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="19eb8-117">Application</span></span> | <span data-ttu-id="19eb8-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="19eb8-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="19eb8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="19eb8-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/tables/{id|name}/sort/clear
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/sort/clear
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/sort/clear
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/sort/clear

```
## <a name="request-headers"></a><span data-ttu-id="19eb8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="19eb8-120">Request headers</span></span>
| <span data-ttu-id="19eb8-121">Nome</span><span class="sxs-lookup"><span data-stu-id="19eb8-121">Name</span></span>       | <span data-ttu-id="19eb8-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="19eb8-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="19eb8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="19eb8-123">Authorization</span></span>  | <span data-ttu-id="19eb8-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="19eb8-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="19eb8-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="19eb8-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="19eb8-p105">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="19eb8-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="19eb8-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="19eb8-129">Request body</span></span>

## <a name="response"></a><span data-ttu-id="19eb8-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="19eb8-130">Response</span></span>

<span data-ttu-id="19eb8-p106">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="19eb8-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19eb8-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="19eb8-133">Example</span></span>
<span data-ttu-id="19eb8-134">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="19eb8-134">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="19eb8-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="19eb8-135">Request</span></span>
<span data-ttu-id="19eb8-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="19eb8-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="19eb8-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="19eb8-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tablesort_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/sort/clear
```
# <a name="c"></a>[<span data-ttu-id="19eb8-138">C#</span><span class="sxs-lookup"><span data-stu-id="19eb8-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablesort-clear-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="19eb8-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="19eb8-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablesort-clear-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="19eb8-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="19eb8-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablesort-clear-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="19eb8-141">Java</span><span class="sxs-lookup"><span data-stu-id="19eb8-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tablesort-clear-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="19eb8-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="19eb8-142">Response</span></span>
<span data-ttu-id="19eb8-143">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="19eb8-143">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
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


