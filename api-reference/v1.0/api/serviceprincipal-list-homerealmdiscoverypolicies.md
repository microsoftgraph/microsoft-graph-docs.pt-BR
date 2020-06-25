---
title: Lista atribuída homeRealmDiscoveryPolicies
description: Listar homeRealmDiscoveryPolicies atribuídos a uma entidade de serviço.
localization_priority: Normal
author: hpsin
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 91754e1d67d9d88ff7d165638f1bc1d143580cf0
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863576"
---
# <a name="list-assigned-homerealmdiscoverypolicy"></a><span data-ttu-id="36cce-103">Lista atribuída homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="36cce-103">List assigned homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="36cce-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36cce-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="36cce-105">Lista os objetos [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) que são atribuídos a um [servicePrincipalName](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="36cce-105">List the [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) objects that are assigned to a [servicePrincipal](../resources/serviceprincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="36cce-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="36cce-106">Permissions</span></span>

<span data-ttu-id="36cce-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="36cce-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="36cce-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36cce-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="36cce-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="36cce-109">Permission type</span></span>                        | <span data-ttu-id="36cce-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="36cce-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="36cce-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="36cce-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="36cce-112">Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="36cce-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="36cce-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="36cce-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36cce-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36cce-114">Not supported.</span></span> |
| <span data-ttu-id="36cce-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="36cce-115">Application</span></span>                            | <span data-ttu-id="36cce-116">Policy. Read. All e Application. ReadWrite. OwnedBy, Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. OwnedBy, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="36cce-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="36cce-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="36cce-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /servicePrincipals/{id}/homeRealmDiscoveryPolicies
```

## <a name="request-headers"></a><span data-ttu-id="36cce-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="36cce-118">Request headers</span></span>

| <span data-ttu-id="36cce-119">Nome</span><span class="sxs-lookup"><span data-stu-id="36cce-119">Name</span></span>          | <span data-ttu-id="36cce-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="36cce-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="36cce-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="36cce-121">Authorization</span></span> | <span data-ttu-id="36cce-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="36cce-122">Bearer {token}.</span></span> <span data-ttu-id="36cce-123">Required.</span><span class="sxs-lookup"><span data-stu-id="36cce-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="36cce-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="36cce-124">Request body</span></span>

<span data-ttu-id="36cce-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="36cce-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36cce-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="36cce-126">Response</span></span>

<span data-ttu-id="36cce-127">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="36cce-127">If successful, this method returns a `200 OK` response code and a collection of [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="36cce-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="36cce-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="36cce-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="36cce-129">Request</span></span>

<span data-ttu-id="36cce-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="36cce-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="36cce-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="36cce-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_homerealmdiscoverypolicies_on_application"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/homeRealmDiscoveryPolicies
```
# <a name="c"></a>[<span data-ttu-id="36cce-132">C#</span><span class="sxs-lookup"><span data-stu-id="36cce-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-homerealmdiscoverypolicies-on-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="36cce-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36cce-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-homerealmdiscoverypolicies-on-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="36cce-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="36cce-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-homerealmdiscoverypolicies-on-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="36cce-135">Java</span><span class="sxs-lookup"><span data-stu-id="36cce-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-homerealmdiscoverypolicies-on-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="36cce-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="36cce-136">Response</span></span>

<span data-ttu-id="36cce-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="36cce-137">The following is an example of the response.</span></span>

> <span data-ttu-id="36cce-138">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="36cce-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="36cce-139">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="36cce-139">All the properties will be returned from an actual call.</span></span>

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
