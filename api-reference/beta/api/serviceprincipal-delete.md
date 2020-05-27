---
title: Excluir o servicePrincipalName
description: Exclua o servicePrincipalName.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: ec422e251f65b3a0ead4a1d22129cfc0c09be3d6
ms.sourcegitcommit: 7a6231aeb570ff45d01b3db3df07a411f9f60fd1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2020
ms.locfileid: "44383417"
---
# <a name="delete-serviceprincipal"></a><span data-ttu-id="417ef-103">Excluir o servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="417ef-103">Delete servicePrincipal</span></span>

<span data-ttu-id="417ef-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="417ef-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="417ef-105">Excluir um objeto [servicePrincipalName](../resources/serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="417ef-105">Delete a [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="417ef-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="417ef-106">Permissions</span></span>
<span data-ttu-id="417ef-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="417ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="417ef-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="417ef-109">Permission type</span></span>      | <span data-ttu-id="417ef-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="417ef-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="417ef-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="417ef-111">Delegated (work or school account)</span></span> | <span data-ttu-id="417ef-112">Application. ReadWrite. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="417ef-112">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="417ef-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="417ef-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="417ef-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="417ef-114">Not supported.</span></span>    |
|<span data-ttu-id="417ef-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="417ef-115">Application</span></span> | <span data-ttu-id="417ef-116">Application. ReadWrite. OwnedBy, Application. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="417ef-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="417ef-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="417ef-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}

```
## <a name="request-headers"></a><span data-ttu-id="417ef-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="417ef-118">Request headers</span></span>
| <span data-ttu-id="417ef-119">Nome</span><span class="sxs-lookup"><span data-stu-id="417ef-119">Name</span></span>       | <span data-ttu-id="417ef-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="417ef-120">Type</span></span> | <span data-ttu-id="417ef-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="417ef-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="417ef-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="417ef-122">Authorization</span></span>  | <span data-ttu-id="417ef-123">string</span><span class="sxs-lookup"><span data-stu-id="417ef-123">string</span></span>  | <span data-ttu-id="417ef-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="417ef-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="417ef-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="417ef-126">Request body</span></span>
<span data-ttu-id="417ef-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="417ef-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="417ef-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="417ef-128">Response</span></span>

<span data-ttu-id="417ef-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="417ef-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="417ef-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="417ef-131">Examples</span></span>
### <a name="request"></a><span data-ttu-id="417ef-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="417ef-132">Request</span></span>
<span data-ttu-id="417ef-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="417ef-133">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="417ef-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="417ef-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_serviceprincipal"
}-->

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}
```
# <a name="c"></a>[<span data-ttu-id="417ef-135">C#</span><span class="sxs-lookup"><span data-stu-id="417ef-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="417ef-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="417ef-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="417ef-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="417ef-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="417ef-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="417ef-138">Response</span></span>
<span data-ttu-id="417ef-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="417ef-139">Here is an example of the response.</span></span> 
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
