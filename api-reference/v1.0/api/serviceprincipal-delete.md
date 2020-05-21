---
title: Excluir o servicePrincipalName
description: Exclua o servicePrincipalName.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: bb1fc5a41baa29909c95b757208b12d8a1f8783b
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44334201"
---
# <a name="delete-serviceprincipal"></a><span data-ttu-id="c2c92-103">Excluir o servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="c2c92-103">Delete servicePrincipal</span></span>

<span data-ttu-id="c2c92-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2c92-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c2c92-105">Excluir um objeto [servicePrincipalName](../resources/serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="c2c92-105">Delete a [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c2c92-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c2c92-106">Permissions</span></span>
<span data-ttu-id="c2c92-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2c92-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2c92-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c2c92-109">Permission type</span></span>      | <span data-ttu-id="c2c92-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c2c92-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2c92-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c2c92-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c2c92-112">Application. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="c2c92-112">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c2c92-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c2c92-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2c92-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c2c92-114">Not supported.</span></span>    |
|<span data-ttu-id="c2c92-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c2c92-115">Application</span></span> | <span data-ttu-id="c2c92-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2c92-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c2c92-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c2c92-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}

```
## <a name="request-headers"></a><span data-ttu-id="c2c92-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c2c92-118">Request headers</span></span>
| <span data-ttu-id="c2c92-119">Nome</span><span class="sxs-lookup"><span data-stu-id="c2c92-119">Name</span></span>       | <span data-ttu-id="c2c92-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2c92-120">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="c2c92-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c2c92-121">Authorization</span></span> | <span data-ttu-id="c2c92-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c2c92-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c2c92-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="c2c92-124">Content-type</span></span> | <span data-ttu-id="c2c92-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c2c92-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c2c92-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c2c92-127">Request body</span></span>
<span data-ttu-id="c2c92-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c2c92-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2c92-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2c92-129">Response</span></span>

<span data-ttu-id="c2c92-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c2c92-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c2c92-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c2c92-132">Examples</span></span>
### <a name="request"></a><span data-ttu-id="c2c92-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c2c92-133">Request</span></span>
<span data-ttu-id="c2c92-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c2c92-134">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c2c92-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="c2c92-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_serviceprincipal"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/servicePrincipals/{id}
```
# <a name="c"></a>[<span data-ttu-id="c2c92-136">C#</span><span class="sxs-lookup"><span data-stu-id="c2c92-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c2c92-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c2c92-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c2c92-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c2c92-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c2c92-139">Java</span><span class="sxs-lookup"><span data-stu-id="c2c92-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="c2c92-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2c92-140">Response</span></span>
<span data-ttu-id="c2c92-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c2c92-141">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete servicePrincipal",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
