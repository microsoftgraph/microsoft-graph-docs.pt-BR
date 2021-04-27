---
title: Listar homeRealmDiscoveryPolicies atribuídas
description: Listar homeRealmDiscoveryPolicies atribuídas a um servicePrincipal.
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 73bc69c6ef53f831126f2d87205c1ec423d61b92
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52036613"
---
# <a name="list-assigned-homerealmdiscoverypolicy"></a><span data-ttu-id="2586c-103">Listar homeRealmDiscoveryPolicy atribuída</span><span class="sxs-lookup"><span data-stu-id="2586c-103">List assigned homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="2586c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2586c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2586c-105">Listar [os objetos homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) atribuídos a [um servicePrincipal](../resources/servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="2586c-105">List the [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) objects that are assigned to a [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2586c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2586c-106">Permissions</span></span>

<span data-ttu-id="2586c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2586c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2586c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2586c-109">Permission type</span></span>                        | <span data-ttu-id="2586c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2586c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2586c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2586c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2586c-112">Policy.Read.All e Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration e Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2586c-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span>  |
| <span data-ttu-id="2586c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2586c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2586c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2586c-114">Not supported.</span></span> |
| <span data-ttu-id="2586c-115">Application</span><span class="sxs-lookup"><span data-stu-id="2586c-115">Application</span></span>                            | <span data-ttu-id="2586c-116">Policy.Read.All e Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration e Application.ReadWrite.OwnedBy, Policy.Read.All e Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration e Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2586c-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2586c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2586c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /servicePrincipals/{id}/homeRealmDiscoveryPolicies
```

## <a name="request-headers"></a><span data-ttu-id="2586c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2586c-118">Request headers</span></span>

| <span data-ttu-id="2586c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="2586c-119">Name</span></span>          | <span data-ttu-id="2586c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="2586c-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="2586c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="2586c-121">Authorization</span></span> | <span data-ttu-id="2586c-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="2586c-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="2586c-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2586c-123">Request body</span></span>

<span data-ttu-id="2586c-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2586c-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2586c-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="2586c-125">Response</span></span>

<span data-ttu-id="2586c-126">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos homeRealmDiscoveryPolicy](../resources/homeRealmDiscoveryPolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2586c-126">If successful, this method returns a `200 OK` response code and a collection of [homeRealmDiscoveryPolicy](../resources/homeRealmDiscoveryPolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2586c-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2586c-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="2586c-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2586c-128">Request</span></span>

<span data-ttu-id="2586c-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2586c-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2586c-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="2586c-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_homerealmdiscoverypolicies_on_serviceprincipal"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/homeRealmDiscoveryPolicies
```
# <a name="c"></a>[<span data-ttu-id="2586c-131">C#</span><span class="sxs-lookup"><span data-stu-id="2586c-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-homerealmdiscoverypolicies-on-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2586c-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2586c-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-homerealmdiscoverypolicies-on-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2586c-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2586c-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-homerealmdiscoverypolicies-on-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2586c-134">Java</span><span class="sxs-lookup"><span data-stu-id="2586c-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-homerealmdiscoverypolicies-on-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2586c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="2586c-135">Response</span></span>

<span data-ttu-id="2586c-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2586c-136">The following is an example of the response.</span></span>

> <span data-ttu-id="2586c-137">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2586c-137">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.homeRealmDiscoveryPolicy",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "definition": [
        "definition-value"
      ],
      "displayName": "displayName-value",
      "isOrganizationDefault": true,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List assigned homeRealmDiscoveryPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



