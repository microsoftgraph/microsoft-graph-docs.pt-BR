---
title: Remover claimsMappingPolicy
description: Remover um claimsMappingPolicy de um servicePrincipalName.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d1ac42059754d8a9264219f797d9bebd27d7c46b
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2020
ms.locfileid: "42590264"
---
# <a name="remove-claimsmappingpolicy"></a><span data-ttu-id="2407e-103">Remover claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="2407e-103">Remove claimsMappingPolicy</span></span>

<span data-ttu-id="2407e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2407e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2407e-105">Remover um [claimsMappingPolicy](../resources/claimsmappingpolicy.md) de um [servicePrincipalName](../resources/servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="2407e-105">Remove a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) from a [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2407e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2407e-106">Permissions</span></span>

<span data-ttu-id="2407e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2407e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2407e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2407e-109">Permission type</span></span>                        | <span data-ttu-id="2407e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2407e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2407e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2407e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2407e-112">Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="2407e-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span>  |
| <span data-ttu-id="2407e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2407e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2407e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2407e-114">Not supported.</span></span> |
| <span data-ttu-id="2407e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2407e-115">Application</span></span>                            | <span data-ttu-id="2407e-116">Policy. Read. All e Application. ReadWrite. OwnedBy, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. OwnedBy, Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="2407e-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2407e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2407e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{id}/claimsMappingPolicies/{id}$ref
```

## <a name="request-headers"></a><span data-ttu-id="2407e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2407e-118">Request headers</span></span>

| <span data-ttu-id="2407e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="2407e-119">Name</span></span>          | <span data-ttu-id="2407e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="2407e-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="2407e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="2407e-121">Authorization</span></span> | <span data-ttu-id="2407e-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="2407e-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="2407e-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2407e-123">Request body</span></span>

<span data-ttu-id="2407e-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2407e-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2407e-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="2407e-125">Response</span></span>

<span data-ttu-id="2407e-126">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2407e-126">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="2407e-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2407e-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2407e-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2407e-128">Request</span></span>

<span data-ttu-id="2407e-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2407e-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2407e-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="2407e-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_claimsmappingpolicy_from_serviceprincipal"
}-->

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/claimsMappingPolicies/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="2407e-131">C#</span><span class="sxs-lookup"><span data-stu-id="2407e-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-claimsmappingpolicy-from-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2407e-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2407e-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-claimsmappingpolicy-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2407e-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2407e-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-claimsmappingpolicy-from-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2407e-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="2407e-134">Response</span></span>

<span data-ttu-id="2407e-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2407e-135">The following is an example of the response.</span></span>

> <span data-ttu-id="2407e-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2407e-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
