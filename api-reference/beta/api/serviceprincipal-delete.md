---
title: Excluir servicePrincipal
description: Exclua o servicePrincipalName.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 54e4fbb4c3a764d4b1933439783e59ab79bda23a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058659"
---
# <a name="delete-serviceprincipal"></a><span data-ttu-id="03a15-103">Excluir servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="03a15-103">Delete servicePrincipal</span></span>

<span data-ttu-id="03a15-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03a15-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03a15-105">Excluir um objeto [servicePrincipalName](../resources/serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="03a15-105">Delete a [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="03a15-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="03a15-106">Permissions</span></span>
<span data-ttu-id="03a15-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03a15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03a15-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="03a15-109">Permission type</span></span>      | <span data-ttu-id="03a15-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="03a15-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="03a15-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="03a15-111">Delegated (work or school account)</span></span> | <span data-ttu-id="03a15-112">Application. ReadWrite. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="03a15-112">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="03a15-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="03a15-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03a15-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="03a15-114">Not supported.</span></span>    |
|<span data-ttu-id="03a15-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="03a15-115">Application</span></span> | <span data-ttu-id="03a15-116">Application. ReadWrite. OwnedBy, Application. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="03a15-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="03a15-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="03a15-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}
```
## <a name="request-headers"></a><span data-ttu-id="03a15-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="03a15-118">Request headers</span></span>
| <span data-ttu-id="03a15-119">Nome</span><span class="sxs-lookup"><span data-stu-id="03a15-119">Name</span></span>       | <span data-ttu-id="03a15-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="03a15-120">Type</span></span> | <span data-ttu-id="03a15-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="03a15-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="03a15-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="03a15-122">Authorization</span></span>  | <span data-ttu-id="03a15-123">string</span><span class="sxs-lookup"><span data-stu-id="03a15-123">string</span></span>  | <span data-ttu-id="03a15-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="03a15-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="03a15-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="03a15-126">Request body</span></span>
<span data-ttu-id="03a15-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="03a15-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="03a15-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="03a15-128">Response</span></span>

<span data-ttu-id="03a15-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="03a15-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="03a15-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="03a15-131">Examples</span></span>
### <a name="request"></a><span data-ttu-id="03a15-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="03a15-132">Request</span></span>
<span data-ttu-id="03a15-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="03a15-133">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="03a15-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="03a15-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_serviceprincipal"
}-->

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}
```
# <a name="c"></a>[<span data-ttu-id="03a15-135">C#</span><span class="sxs-lookup"><span data-stu-id="03a15-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="03a15-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="03a15-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="03a15-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="03a15-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="03a15-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="03a15-138">Response</span></span>
<span data-ttu-id="03a15-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="03a15-139">Here is an example of the response.</span></span> 
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


