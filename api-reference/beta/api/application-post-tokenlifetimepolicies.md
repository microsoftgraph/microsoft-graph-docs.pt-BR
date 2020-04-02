---
title: Atribiur tokenLifetimePolicy
description: Atribua um tokenLifetimePolicy a uma entidade de serviço ou aplicativo.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 93cef7b8bf48fc1a2c1b54a11745a3393cb365aa
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2020
ms.locfileid: "43107056"
---
# <a name="assign-tokenlifetimepolicy"></a><span data-ttu-id="ce67d-103">Atribiur tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="ce67d-103">Assign tokenLifetimePolicy</span></span>

<span data-ttu-id="ce67d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce67d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce67d-105">Atribua um [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) a um [aplicativo](../resources/application.md) ou a um [servicePrincipalName](../resources/servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="ce67d-105">Assign a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) to an [application](../resources/application.md) or [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ce67d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ce67d-106">Permissions</span></span>

<span data-ttu-id="ce67d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce67d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ce67d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ce67d-109">Permission type</span></span>                        | <span data-ttu-id="ce67d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ce67d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ce67d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ce67d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ce67d-112">Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="ce67d-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="ce67d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ce67d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce67d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ce67d-114">Not supported.</span></span> |
| <span data-ttu-id="ce67d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ce67d-115">Application</span></span>                            | <span data-ttu-id="ce67d-116">Policy. Read. All e Application. ReadWrite. OwnedBy, Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. OwnedBy, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="ce67d-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce67d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ce67d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/tokenLifetimePolicies/$ref
POST /servicePrincipals/{id}/tokenLifetimePolicies/$ref
```

## <a name="request-headers"></a><span data-ttu-id="ce67d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ce67d-118">Request headers</span></span>

| <span data-ttu-id="ce67d-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ce67d-119">Name</span></span>          | <span data-ttu-id="ce67d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce67d-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ce67d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ce67d-121">Authorization</span></span> | <span data-ttu-id="ce67d-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="ce67d-122">Bearer {token}</span></span> |
| <span data-ttu-id="ce67d-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ce67d-123">Content-Type</span></span> | <span data-ttu-id="ce67d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ce67d-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ce67d-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ce67d-125">Request body</span></span>

<span data-ttu-id="ce67d-126">No corpo da solicitação, forneça o identificador do objeto [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) (usando uma `@odata.id` Propriedade) que deve ser atribuído ao aplicativo ou à entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="ce67d-126">In the request body, supply the identifier of the [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object (using an `@odata.id` property) that should be assigned to the application or service principal.</span></span>

## <a name="response"></a><span data-ttu-id="ce67d-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce67d-127">Response</span></span>

<span data-ttu-id="ce67d-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ce67d-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ce67d-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ce67d-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ce67d-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ce67d-131">Request</span></span>

<span data-ttu-id="ce67d-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ce67d-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ce67d-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="ce67d-133">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="ce67d-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ce67d-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-tokenlifetimepolicy-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="ce67d-135">C#</span><span class="sxs-lookup"><span data-stu-id="ce67d-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-tokenlifetimepolicy-from-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ce67d-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ce67d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-tokenlifetimepolicy-from-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ce67d-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce67d-137">Response</span></span>

<span data-ttu-id="ce67d-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ce67d-138">The following is an example of the response.</span></span>

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
