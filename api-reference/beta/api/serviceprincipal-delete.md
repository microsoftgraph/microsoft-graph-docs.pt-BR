---
title: Excluir servicePrincipal
description: Exclua servicePrincipal.
localization_priority: Normal
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 7066cd3184894f8de1cada2f1936ee1bd343d4a0
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137526"
---
# <a name="delete-serviceprincipal"></a><span data-ttu-id="13359-103">Excluir servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="13359-103">Delete servicePrincipal</span></span>

<span data-ttu-id="13359-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13359-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13359-105">[Exclua um objeto servicePrincipal.](../resources/serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="13359-105">Delete a [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="13359-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="13359-106">Permissions</span></span>
<span data-ttu-id="13359-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13359-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13359-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="13359-109">Permission type</span></span>      | <span data-ttu-id="13359-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="13359-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="13359-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="13359-111">Delegated (work or school account)</span></span> | <span data-ttu-id="13359-112">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="13359-112">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="13359-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="13359-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13359-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13359-114">Not supported.</span></span>    |
|<span data-ttu-id="13359-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="13359-115">Application</span></span> | <span data-ttu-id="13359-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13359-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="13359-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="13359-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}
```
## <a name="request-headers"></a><span data-ttu-id="13359-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="13359-118">Request headers</span></span>
| <span data-ttu-id="13359-119">Nome</span><span class="sxs-lookup"><span data-stu-id="13359-119">Name</span></span>       | <span data-ttu-id="13359-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="13359-120">Type</span></span> | <span data-ttu-id="13359-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="13359-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="13359-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="13359-122">Authorization</span></span>  | <span data-ttu-id="13359-123">string</span><span class="sxs-lookup"><span data-stu-id="13359-123">string</span></span>  | <span data-ttu-id="13359-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="13359-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="13359-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="13359-126">Request body</span></span>
<span data-ttu-id="13359-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="13359-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13359-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="13359-128">Response</span></span>

<span data-ttu-id="13359-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="13359-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="13359-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="13359-131">Examples</span></span>
### <a name="request"></a><span data-ttu-id="13359-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="13359-132">Request</span></span>
<span data-ttu-id="13359-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="13359-133">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="13359-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="13359-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_serviceprincipal"
}-->

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}
```
# <a name="c"></a>[<span data-ttu-id="13359-135">C#</span><span class="sxs-lookup"><span data-stu-id="13359-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="13359-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="13359-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="13359-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="13359-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="13359-138">Java</span><span class="sxs-lookup"><span data-stu-id="13359-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="13359-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="13359-139">Response</span></span>
<span data-ttu-id="13359-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="13359-140">Here is an example of the response.</span></span> 
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



