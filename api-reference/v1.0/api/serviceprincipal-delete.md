---
title: Excluir servicePrincipal
description: Exclua o servicePrincipalName.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 3aeec8e560535eec0108331b04f3f0dda18133cd
ms.sourcegitcommit: 4a37678913c98f62b8174de6ca03908b9af864bd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/28/2020
ms.locfileid: "47296501"
---
# <a name="delete-serviceprincipal"></a><span data-ttu-id="845a3-103">Excluir servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="845a3-103">Delete servicePrincipal</span></span>

<span data-ttu-id="845a3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="845a3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="845a3-105">Excluir um objeto [servicePrincipalName](../resources/serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="845a3-105">Delete a [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="845a3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="845a3-106">Permissions</span></span>
<span data-ttu-id="845a3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="845a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="845a3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="845a3-109">Permission type</span></span>      | <span data-ttu-id="845a3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="845a3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="845a3-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="845a3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="845a3-112">Application. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="845a3-112">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="845a3-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="845a3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="845a3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="845a3-114">Not supported.</span></span>    |
|<span data-ttu-id="845a3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="845a3-115">Application</span></span> | <span data-ttu-id="845a3-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="845a3-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="845a3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="845a3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}
```
## <a name="request-headers"></a><span data-ttu-id="845a3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="845a3-118">Request headers</span></span>
| <span data-ttu-id="845a3-119">Nome</span><span class="sxs-lookup"><span data-stu-id="845a3-119">Name</span></span>       | <span data-ttu-id="845a3-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="845a3-120">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="845a3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="845a3-121">Authorization</span></span> | <span data-ttu-id="845a3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="845a3-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="845a3-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="845a3-124">Content-type</span></span> | <span data-ttu-id="845a3-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="845a3-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="845a3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="845a3-127">Request body</span></span>
<span data-ttu-id="845a3-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="845a3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="845a3-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="845a3-129">Response</span></span>

<span data-ttu-id="845a3-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="845a3-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="845a3-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="845a3-132">Examples</span></span>
### <a name="request"></a><span data-ttu-id="845a3-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="845a3-133">Request</span></span>
<span data-ttu-id="845a3-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="845a3-134">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="845a3-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="845a3-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_serviceprincipal"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/servicePrincipals/{id}
```
# <a name="c"></a>[<span data-ttu-id="845a3-136">C#</span><span class="sxs-lookup"><span data-stu-id="845a3-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="845a3-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="845a3-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="845a3-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="845a3-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="845a3-139">Java</span><span class="sxs-lookup"><span data-stu-id="845a3-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="845a3-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="845a3-140">Response</span></span>
<span data-ttu-id="845a3-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="845a3-141">Here is an example of the response.</span></span> 
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
