---
title: 'TableSort: clear'
description: Limpa a classificação que está na tabela. Essa ação não modifica a ordenação da tabela, mas limpa o estado dos botões do cabeçalho.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: f202c378ddf774fc2bae2400983a598d2f3a8918
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35982505"
---
# <a name="tablesort-clear"></a><span data-ttu-id="30fbb-104">TableSort: clear</span><span class="sxs-lookup"><span data-stu-id="30fbb-104">TableSort: clear</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30fbb-p102">Limpa a classificação que está na tabela. Essa ação não modifica a ordenação da tabela, mas limpa o estado dos botões do cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="30fbb-p102">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>
## <a name="permissions"></a><span data-ttu-id="30fbb-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="30fbb-107">Permissions</span></span>
<span data-ttu-id="30fbb-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30fbb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30fbb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="30fbb-110">Permission type</span></span>      | <span data-ttu-id="30fbb-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="30fbb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="30fbb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="30fbb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="30fbb-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="30fbb-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="30fbb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="30fbb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30fbb-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="30fbb-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="30fbb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="30fbb-116">Application</span></span> | <span data-ttu-id="30fbb-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="30fbb-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="30fbb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="30fbb-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/clear

```
## <a name="request-headers"></a><span data-ttu-id="30fbb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="30fbb-119">Request headers</span></span>
| <span data-ttu-id="30fbb-120">Nome</span><span class="sxs-lookup"><span data-stu-id="30fbb-120">Name</span></span>       | <span data-ttu-id="30fbb-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="30fbb-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="30fbb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="30fbb-122">Authorization</span></span>  | <span data-ttu-id="30fbb-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="30fbb-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="30fbb-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="30fbb-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="30fbb-p105">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="30fbb-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="30fbb-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="30fbb-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="30fbb-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="30fbb-129">Response</span></span>

<span data-ttu-id="30fbb-p106">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="30fbb-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30fbb-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="30fbb-132">Example</span></span>
<span data-ttu-id="30fbb-133">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="30fbb-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="30fbb-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="30fbb-134">Request</span></span>
<span data-ttu-id="30fbb-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="30fbb-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="30fbb-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="30fbb-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tablesort_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/sort/clear
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="30fbb-137">C#</span><span class="sxs-lookup"><span data-stu-id="30fbb-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablesort-clear-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="30fbb-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="30fbb-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablesort-clear-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="30fbb-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="30fbb-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablesort-clear-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="30fbb-140">Java</span><span class="sxs-lookup"><span data-stu-id="30fbb-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tablesort-clear-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="30fbb-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="30fbb-141">Response</span></span>
<span data-ttu-id="30fbb-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="30fbb-142">Here is an example of the response.</span></span> 
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
