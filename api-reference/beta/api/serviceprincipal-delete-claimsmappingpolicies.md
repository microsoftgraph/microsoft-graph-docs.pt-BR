---
title: Remover claimsMappingPolicy
description: Remova um claimsMappingPolicy de um servicePrincipal.
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: fed2bd63c3b944c6a32affbd3fc49edd994f0cd7
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051953"
---
# <a name="remove-claimsmappingpolicy"></a><span data-ttu-id="26c08-103">Remover claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="26c08-103">Remove claimsMappingPolicy</span></span>

<span data-ttu-id="26c08-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26c08-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26c08-105">Remover um [claimsMappingPolicy](../resources/claimsmappingpolicy.md) de [um servicePrincipal](../resources/servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="26c08-105">Remove a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) from a [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="26c08-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="26c08-106">Permissions</span></span>

<span data-ttu-id="26c08-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26c08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="26c08-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="26c08-109">Permission type</span></span>                        | <span data-ttu-id="26c08-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="26c08-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="26c08-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="26c08-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="26c08-112">Policy.Read.All e Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration e Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26c08-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span>  |
| <span data-ttu-id="26c08-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="26c08-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26c08-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="26c08-114">Not supported.</span></span> |
| <span data-ttu-id="26c08-115">Application</span><span class="sxs-lookup"><span data-stu-id="26c08-115">Application</span></span>                            | <span data-ttu-id="26c08-116">Policy.Read.All e Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration e Application.ReadWrite.OwnedBy, Policy.Read.All e Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration e Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26c08-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="26c08-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="26c08-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{id}/claimsMappingPolicies/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="26c08-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="26c08-118">Request headers</span></span>

| <span data-ttu-id="26c08-119">Nome</span><span class="sxs-lookup"><span data-stu-id="26c08-119">Name</span></span>          | <span data-ttu-id="26c08-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="26c08-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="26c08-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="26c08-121">Authorization</span></span> | <span data-ttu-id="26c08-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="26c08-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="26c08-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="26c08-123">Request body</span></span>

<span data-ttu-id="26c08-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="26c08-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="26c08-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="26c08-125">Response</span></span>

<span data-ttu-id="26c08-126">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="26c08-126">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="26c08-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="26c08-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="26c08-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="26c08-128">Request</span></span>

<span data-ttu-id="26c08-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="26c08-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="26c08-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="26c08-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_claimsmappingpolicy_from_serviceprincipal"
}-->

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/claimsMappingPolicies/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="26c08-131">C#</span><span class="sxs-lookup"><span data-stu-id="26c08-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-claimsmappingpolicy-from-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="26c08-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="26c08-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-claimsmappingpolicy-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="26c08-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="26c08-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-claimsmappingpolicy-from-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="26c08-134">Java</span><span class="sxs-lookup"><span data-stu-id="26c08-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-claimsmappingpolicy-from-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="26c08-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="26c08-135">Response</span></span>

<span data-ttu-id="26c08-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="26c08-136">The following is an example of the response.</span></span>

> <span data-ttu-id="26c08-137">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="26c08-137">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "description": "Remove claimsMappingPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



