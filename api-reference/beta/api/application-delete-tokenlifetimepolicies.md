---
title: Remover tokenLifetimePolicy
description: Remova um tokenLifetimePolicy de um aplicativo ou servicePrincipal.
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: efe54936a33c468590bfb31d046b116544a373a5
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129233"
---
# <a name="remove-tokenlifetimepolicy"></a><span data-ttu-id="06e4f-103">Remover tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="06e4f-103">Remove tokenLifetimePolicy</span></span>

<span data-ttu-id="06e4f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06e4f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06e4f-105">Remover um [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) de um [aplicativo ou](../resources/application.md) [servicePrincipal](../resources/servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="06e4f-105">Remove a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) from an [application](../resources/application.md) or [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="06e4f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="06e4f-106">Permissions</span></span>

<span data-ttu-id="06e4f-107">Um dos seguintes conjuntos de permissões é necessário para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="06e4f-107">One of the following sets of permissions is required to call this API.</span></span> <span data-ttu-id="06e4f-108">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06e4f-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="06e4f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="06e4f-109">Permission type</span></span>                        | <span data-ttu-id="06e4f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="06e4f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="06e4f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="06e4f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="06e4f-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06e4f-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="06e4f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="06e4f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06e4f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06e4f-114">Not supported.</span></span> |
| <span data-ttu-id="06e4f-115">Application</span><span class="sxs-lookup"><span data-stu-id="06e4f-115">Application</span></span>                            | <span data-ttu-id="06e4f-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06e4f-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="06e4f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="06e4f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /applications/{id}/tokenLifetimePolicies/{id}/$ref
DELETE /servicePrincipals/{id}/tokenLifetimePolicies/{id}$ref
```

## <a name="request-headers"></a><span data-ttu-id="06e4f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="06e4f-118">Request headers</span></span>

| <span data-ttu-id="06e4f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="06e4f-119">Name</span></span>          | <span data-ttu-id="06e4f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="06e4f-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="06e4f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="06e4f-121">Authorization</span></span> | <span data-ttu-id="06e4f-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="06e4f-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="06e4f-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="06e4f-123">Request body</span></span>

<span data-ttu-id="06e4f-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="06e4f-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06e4f-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="06e4f-125">Response</span></span>

<span data-ttu-id="06e4f-126">Quando é bem-sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="06e4f-126">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="06e4f-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="06e4f-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="06e4f-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="06e4f-128">Request</span></span>

<span data-ttu-id="06e4f-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="06e4f-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="06e4f-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="06e4f-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_tokenlifetimepolicy_from_application"
}-->

```http
DELETE https://graph.microsoft.com/beta/applications/{id}/tokenLifetimePolicies/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="06e4f-131">C#</span><span class="sxs-lookup"><span data-stu-id="06e4f-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-tokenlifetimepolicy-from-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="06e4f-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="06e4f-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-tokenlifetimepolicy-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="06e4f-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="06e4f-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-tokenlifetimepolicy-from-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="06e4f-134">Java</span><span class="sxs-lookup"><span data-stu-id="06e4f-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-tokenlifetimepolicy-from-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="06e4f-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="06e4f-135">Response</span></span>

<span data-ttu-id="06e4f-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="06e4f-136">The following is an example of the response.</span></span>

> <span data-ttu-id="06e4f-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="06e4f-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "Remove tokenLifetimePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



