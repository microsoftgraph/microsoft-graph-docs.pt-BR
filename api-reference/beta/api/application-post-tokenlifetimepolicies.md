---
title: Atribiur tokenLifetimePolicy
description: Atribua um tokenLifetimePolicy a um aplicativo ou entidade de serviço.
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 1356714b5a54775ad304e6f32a063b2be7235954
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129069"
---
# <a name="assign-tokenlifetimepolicy"></a><span data-ttu-id="a9638-103">Atribiur tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="a9638-103">Assign tokenLifetimePolicy</span></span>

<span data-ttu-id="a9638-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9638-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9638-105">Atribua [um tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) a [um aplicativo](../resources/application.md) ou [servicePrincipal](../resources/servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="a9638-105">Assign a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) to an [application](../resources/application.md) or [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a9638-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a9638-106">Permissions</span></span>

<span data-ttu-id="a9638-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9638-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a9638-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a9638-109">Permission type</span></span>                        | <span data-ttu-id="a9638-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a9638-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a9638-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a9638-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a9638-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9638-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="a9638-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a9638-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9638-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9638-114">Not supported.</span></span> |
| <span data-ttu-id="a9638-115">Application</span><span class="sxs-lookup"><span data-stu-id="a9638-115">Application</span></span>                            | <span data-ttu-id="a9638-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9638-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a9638-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a9638-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/tokenLifetimePolicies/$ref
POST /servicePrincipals/{id}/tokenLifetimePolicies/$ref
```

## <a name="request-headers"></a><span data-ttu-id="a9638-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a9638-118">Request headers</span></span>

| <span data-ttu-id="a9638-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a9638-119">Name</span></span>          | <span data-ttu-id="a9638-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9638-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a9638-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a9638-121">Authorization</span></span> | <span data-ttu-id="a9638-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="a9638-122">Bearer {token}</span></span> |
| <span data-ttu-id="a9638-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a9638-123">Content-Type</span></span> | <span data-ttu-id="a9638-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a9638-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="a9638-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a9638-125">Request body</span></span>

<span data-ttu-id="a9638-126">No corpo da solicitação, fornece o identificador do objeto [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) (usando uma propriedade) que deve ser atribuído ao aplicativo ou entidade `@odata.id` de serviço.</span><span class="sxs-lookup"><span data-stu-id="a9638-126">In the request body, supply the identifier of the [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object (using an `@odata.id` property) that should be assigned to the application or service principal.</span></span>

## <a name="response"></a><span data-ttu-id="a9638-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9638-127">Response</span></span>

<span data-ttu-id="a9638-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a9638-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a9638-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a9638-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a9638-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9638-131">Request</span></span>

<span data-ttu-id="a9638-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a9638-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a9638-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a9638-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_tokenlifetimepolicy_from_application"
}-->

```http
POST https://graph.microsoft.com/beta/applications/{id}/tokenLifetimePolicies
Content-Type: application/json

{
  "@odata.id":"https://graph.microsoft.com/beta/policies/tokenLifetimePolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"
}
```
# <a name="javascript"></a>[<span data-ttu-id="a9638-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a9638-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-tokenlifetimepolicy-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="a9638-135">C#</span><span class="sxs-lookup"><span data-stu-id="a9638-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-tokenlifetimepolicy-from-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a9638-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a9638-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-tokenlifetimepolicy-from-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a9638-137">Java</span><span class="sxs-lookup"><span data-stu-id="a9638-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-tokenlifetimepolicy-from-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a9638-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9638-138">Response</span></span>

<span data-ttu-id="a9638-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a9638-139">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Assign tokenLifetimePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



