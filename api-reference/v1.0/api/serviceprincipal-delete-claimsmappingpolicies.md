---
title: Remover claimsMappingPolicy
description: Remover um claimsMappingPolicy de um servicePrincipalName.
localization_priority: Normal
author: paulgarn
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4231bf11e28b3514f8543c41b76d132029fb122a
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2020
ms.locfileid: "44864148"
---
# <a name="remove-claimsmappingpolicy"></a><span data-ttu-id="8761c-103">Remover claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="8761c-103">Remove claimsMappingPolicy</span></span>

<span data-ttu-id="8761c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8761c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8761c-105">Remover um [claimsMappingPolicy](../resources/claimsmappingpolicy.md) de um [servicePrincipalName](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="8761c-105">Remove a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) from a [servicePrincipal](../resources/serviceprincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8761c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8761c-106">Permissions</span></span>

<span data-ttu-id="8761c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8761c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8761c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8761c-109">Permission type</span></span>                        | <span data-ttu-id="8761c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8761c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8761c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8761c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8761c-112">Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="8761c-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="8761c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8761c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8761c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8761c-114">Not supported.</span></span> |
| <span data-ttu-id="8761c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8761c-115">Application</span></span>                            | <span data-ttu-id="8761c-116">Policy. Read. All e Application. ReadWrite. OwnedBy, Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. OwnedBy, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="8761c-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8761c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8761c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{id}/claimsMappingPolicies/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="8761c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8761c-118">Request headers</span></span>

| <span data-ttu-id="8761c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="8761c-119">Name</span></span>          | <span data-ttu-id="8761c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="8761c-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8761c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8761c-121">Authorization</span></span> | <span data-ttu-id="8761c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8761c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8761c-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8761c-124">Request body</span></span>

<span data-ttu-id="8761c-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8761c-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8761c-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="8761c-126">Response</span></span>

<span data-ttu-id="8761c-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8761c-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="8761c-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8761c-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8761c-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8761c-129">Request</span></span>

<span data-ttu-id="8761c-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8761c-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8761c-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="8761c-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_claimsmappingpolicy_from_servicePrincipal"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/servicePrincipals/{id}/claimsMappingPolicies/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="8761c-132">C#</span><span class="sxs-lookup"><span data-stu-id="8761c-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-claimsmappingpolicy-from-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8761c-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8761c-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-claimsmappingpolicy-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8761c-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8761c-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-claimsmappingpolicy-from-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8761c-135">Java</span><span class="sxs-lookup"><span data-stu-id="8761c-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-claimsmappingpolicy-from-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8761c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="8761c-136">Response</span></span>

<span data-ttu-id="8761c-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8761c-137">The following is an example of the response.</span></span>

> <span data-ttu-id="8761c-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8761c-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
