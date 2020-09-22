---
title: Excluir servicePrincipal
description: Exclua o servicePrincipalName.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 071f767c31b8cee19defc5ccd635d73cce8c0f5f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48044079"
---
# <a name="delete-serviceprincipal"></a><span data-ttu-id="4edf1-103">Excluir servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="4edf1-103">Delete servicePrincipal</span></span>

<span data-ttu-id="4edf1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4edf1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4edf1-105">Excluir um objeto [servicePrincipalName](../resources/serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="4edf1-105">Delete a [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4edf1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4edf1-106">Permissions</span></span>
<span data-ttu-id="4edf1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4edf1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4edf1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4edf1-109">Permission type</span></span>      | <span data-ttu-id="4edf1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4edf1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4edf1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4edf1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4edf1-112">Application. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="4edf1-112">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4edf1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4edf1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4edf1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4edf1-114">Not supported.</span></span>    |
|<span data-ttu-id="4edf1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4edf1-115">Application</span></span> | <span data-ttu-id="4edf1-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4edf1-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4edf1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4edf1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}
```
## <a name="request-headers"></a><span data-ttu-id="4edf1-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4edf1-118">Request headers</span></span>
| <span data-ttu-id="4edf1-119">Nome</span><span class="sxs-lookup"><span data-stu-id="4edf1-119">Name</span></span>       | <span data-ttu-id="4edf1-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="4edf1-120">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="4edf1-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4edf1-121">Authorization</span></span> | <span data-ttu-id="4edf1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4edf1-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4edf1-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="4edf1-124">Content-type</span></span> | <span data-ttu-id="4edf1-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4edf1-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4edf1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4edf1-127">Request body</span></span>
<span data-ttu-id="4edf1-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4edf1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4edf1-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4edf1-129">Response</span></span>

<span data-ttu-id="4edf1-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4edf1-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4edf1-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4edf1-132">Examples</span></span>
### <a name="request"></a><span data-ttu-id="4edf1-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4edf1-133">Request</span></span>
<span data-ttu-id="4edf1-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4edf1-134">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4edf1-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="4edf1-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_serviceprincipal"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/servicePrincipals/{id}
```
# <a name="c"></a>[<span data-ttu-id="4edf1-136">C#</span><span class="sxs-lookup"><span data-stu-id="4edf1-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4edf1-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4edf1-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4edf1-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4edf1-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4edf1-139">Java</span><span class="sxs-lookup"><span data-stu-id="4edf1-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="4edf1-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="4edf1-140">Response</span></span>
<span data-ttu-id="4edf1-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4edf1-141">Here is an example of the response.</span></span> 
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

