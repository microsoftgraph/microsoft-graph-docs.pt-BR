---
title: 'servicePrincipal: removePassword'
description: Remover uma senha de uma servicePrincipal
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 30f66a540a7a140e6381ff4f4f556b3509a04a3b
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130533"
---
# <a name="serviceprincipal-removepassword"></a><span data-ttu-id="e8c5d-103">servicePrincipal: removePassword</span><span class="sxs-lookup"><span data-stu-id="e8c5d-103">servicePrincipal: removePassword</span></span>

<span data-ttu-id="e8c5d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8c5d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e8c5d-105">Remover uma senha de um [objeto servicePrincipal.](../resources/serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="e8c5d-105">Remove a password from a [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8c5d-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="e8c5d-106">Permissions</span></span>

<span data-ttu-id="e8c5d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8c5d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e8c5d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8c5d-109">Permission type</span></span>                        | <span data-ttu-id="e8c5d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e8c5d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e8c5d-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8c5d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e8c5d-112">Application.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e8c5d-112">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="e8c5d-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8c5d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8c5d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8c5d-114">Not supported.</span></span> |
| <span data-ttu-id="e8c5d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8c5d-115">Application</span></span>                            | <span data-ttu-id="e8c5d-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8c5d-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8c5d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8c5d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/removePassword
```

## <a name="request-headers"></a><span data-ttu-id="e8c5d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e8c5d-118">Request headers</span></span>

| <span data-ttu-id="e8c5d-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e8c5d-119">Name</span></span>           | <span data-ttu-id="e8c5d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8c5d-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="e8c5d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e8c5d-121">Authorization</span></span>  | <span data-ttu-id="e8c5d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8c5d-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e8c5d-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="e8c5d-124">Content-type</span></span>   | <span data-ttu-id="e8c5d-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8c5d-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8c5d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8c5d-127">Request body</span></span>

| <span data-ttu-id="e8c5d-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e8c5d-128">Property</span></span>     | <span data-ttu-id="e8c5d-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="e8c5d-129">Type</span></span>   |<span data-ttu-id="e8c5d-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8c5d-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e8c5d-131">keyId</span><span class="sxs-lookup"><span data-stu-id="e8c5d-131">keyId</span></span> | <span data-ttu-id="e8c5d-132">GUID</span><span class="sxs-lookup"><span data-stu-id="e8c5d-132">GUID</span></span> | <span data-ttu-id="e8c5d-133">O identificador exclusivo da senha.</span><span class="sxs-lookup"><span data-stu-id="e8c5d-133">The unique identifier for the password.</span></span> <span data-ttu-id="e8c5d-134">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8c5d-134">Required.</span></span> |

## <a name="response"></a><span data-ttu-id="e8c5d-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8c5d-135">Response</span></span>

<span data-ttu-id="e8c5d-136">Se tiver êxito, este método retornará um código de resposta `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="e8c5d-136">If successful, this method returns a `204 No content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="e8c5d-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e8c5d-137">Examples</span></span>

<span data-ttu-id="e8c5d-138">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="e8c5d-138">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="e8c5d-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8c5d-139">Request</span></span>

<span data-ttu-id="e8c5d-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e8c5d-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e8c5d-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="e8c5d-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "servicePrincipal_removepassword"
}-->

```http
POST https://graph.microsoft.com/v1.0/servicePrincipals/{id}/removePassword
Content-type: application/json

{
    "keyId": "f0b0b335-1d71-4883-8f98-567911bfdca6"
}
```
# <a name="c"></a>[<span data-ttu-id="e8c5d-142">C#</span><span class="sxs-lookup"><span data-stu-id="e8c5d-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-removepassword-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e8c5d-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e8c5d-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-removepassword-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e8c5d-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e8c5d-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-removepassword-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e8c5d-145">Java</span><span class="sxs-lookup"><span data-stu-id="e8c5d-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-removepassword-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e8c5d-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8c5d-146">Response</span></span>

<span data-ttu-id="e8c5d-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e8c5d-147">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.passwordCredential"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "servicePrincipal: removePassword",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

