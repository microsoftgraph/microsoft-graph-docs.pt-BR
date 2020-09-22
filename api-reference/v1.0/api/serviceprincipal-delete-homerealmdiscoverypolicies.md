---
title: Remover homeRealmDiscoveryPolicy
description: Remover um homeRealmDiscoveryPolicy de um servicePrincipalName.
localization_priority: Normal
author: hpsin
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a5d45f7d6dba80b1f36f978181898bef8b7e4a02
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013010"
---
# <a name="remove-homerealmdiscoverypolicy"></a><span data-ttu-id="b20d3-103">Remover homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="b20d3-103">Remove homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="b20d3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b20d3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b20d3-105">Remover um [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) de um [servicePrincipalName](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="b20d3-105">Remove a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) from a [servicePrincipal](../resources/serviceprincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b20d3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b20d3-106">Permissions</span></span>

<span data-ttu-id="b20d3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b20d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b20d3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b20d3-109">Permission type</span></span>                        | <span data-ttu-id="b20d3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b20d3-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b20d3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b20d3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b20d3-112">Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b20d3-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="b20d3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b20d3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b20d3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b20d3-114">Not supported.</span></span> |
| <span data-ttu-id="b20d3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b20d3-115">Application</span></span>                            | <span data-ttu-id="b20d3-116">Policy. Read. All e Application. ReadWrite. OwnedBy, Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. OwnedBy, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b20d3-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b20d3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b20d3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{id}/homeRealmDiscoveryPolicies/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="b20d3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b20d3-118">Request headers</span></span>

| <span data-ttu-id="b20d3-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b20d3-119">Name</span></span>          | <span data-ttu-id="b20d3-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b20d3-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b20d3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b20d3-121">Authorization</span></span> | <span data-ttu-id="b20d3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b20d3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b20d3-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b20d3-124">Request body</span></span>

<span data-ttu-id="b20d3-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b20d3-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b20d3-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="b20d3-126">Response</span></span>

<span data-ttu-id="b20d3-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b20d3-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="b20d3-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b20d3-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b20d3-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b20d3-129">Request</span></span>

<span data-ttu-id="b20d3-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b20d3-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b20d3-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="b20d3-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_homerealmdiscoverypolicy_from_servicePrincipal"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/servicePrincipals/{id}/homeRealmDiscoveryPolicies/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="b20d3-132">C#</span><span class="sxs-lookup"><span data-stu-id="b20d3-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-homerealmdiscoverypolicy-from-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b20d3-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b20d3-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-homerealmdiscoverypolicy-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b20d3-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b20d3-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-homerealmdiscoverypolicy-from-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b20d3-135">Java</span><span class="sxs-lookup"><span data-stu-id="b20d3-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-homerealmdiscoverypolicy-from-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b20d3-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="b20d3-136">Response</span></span>

<span data-ttu-id="b20d3-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b20d3-137">The following is an example of the response.</span></span>

> <span data-ttu-id="b20d3-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b20d3-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "Remove homeRealmDiscoveryPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

