---
title: 'Table: delete'
description: Exclui a tabela.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 378204783e631818777d9bce7ec77ecf801f1184
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777514"
---
# <a name="table-delete"></a><span data-ttu-id="26ad6-103">Table: delete</span><span class="sxs-lookup"><span data-stu-id="26ad6-103">Table: delete</span></span>

<span data-ttu-id="26ad6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26ad6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="26ad6-105">Exclui a tabela.</span><span class="sxs-lookup"><span data-stu-id="26ad6-105">Deletes the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="26ad6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="26ad6-106">Permissions</span></span>
<span data-ttu-id="26ad6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26ad6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26ad6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="26ad6-109">Permission type</span></span>      | <span data-ttu-id="26ad6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="26ad6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="26ad6-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="26ad6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="26ad6-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="26ad6-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="26ad6-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="26ad6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26ad6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="26ad6-114">Not supported.</span></span>    |
|<span data-ttu-id="26ad6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="26ad6-115">Application</span></span> | <span data-ttu-id="26ad6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="26ad6-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="26ad6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="26ad6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/drive/items/{id}/workbook/tables/{id|name}
DELETE /me/drive/root:/{item-path}:/workbook/tables/{id|name}
DELETE /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}
DELETE /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}

```
## <a name="request-headers"></a><span data-ttu-id="26ad6-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="26ad6-118">Request headers</span></span>
| <span data-ttu-id="26ad6-119">Nome</span><span class="sxs-lookup"><span data-stu-id="26ad6-119">Name</span></span>       | <span data-ttu-id="26ad6-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="26ad6-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="26ad6-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="26ad6-121">Authorization</span></span>  | <span data-ttu-id="26ad6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="26ad6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="26ad6-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="26ad6-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="26ad6-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="26ad6-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="26ad6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="26ad6-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="26ad6-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="26ad6-128">Response</span></span>

<span data-ttu-id="26ad6-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="26ad6-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26ad6-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="26ad6-131">Example</span></span>
<span data-ttu-id="26ad6-132">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="26ad6-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="26ad6-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="26ad6-133">Request</span></span>
<span data-ttu-id="26ad6-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="26ad6-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="26ad6-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="26ad6-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "table_delete"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}
```
# <a name="c"></a>[<span data-ttu-id="26ad6-136">C#</span><span class="sxs-lookup"><span data-stu-id="26ad6-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/table-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="26ad6-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="26ad6-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/table-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="26ad6-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="26ad6-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/table-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="26ad6-139">Java</span><span class="sxs-lookup"><span data-stu-id="26ad6-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/table-delete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="26ad6-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="26ad6-140">Response</span></span>
<span data-ttu-id="26ad6-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="26ad6-141">Here is an example of the response.</span></span> 
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
  "description": "Table: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

