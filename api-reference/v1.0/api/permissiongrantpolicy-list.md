---
title: Listar permissionGrantPolicies
description: Recupere uma lista de objetos permissionGrantPolicy.
localization_priority: Normal
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 283b5da9499245b0c6cca929d7cecdd8bc4a4d27
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448092"
---
# <a name="list-permissiongrantpolicies"></a><span data-ttu-id="e8d16-103">Listar permissionGrantPolicies</span><span class="sxs-lookup"><span data-stu-id="e8d16-103">List permissionGrantPolicies</span></span>

<span data-ttu-id="e8d16-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8d16-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e8d16-105">Recupere a lista de [objetos permissionGrantPolicy.](../resources/permissiongrantpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e8d16-105">Retrieve the list of [permissionGrantPolicy](../resources/permissiongrantpolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8d16-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e8d16-106">Permissions</span></span>

<span data-ttu-id="e8d16-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8d16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e8d16-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8d16-109">Permission type</span></span>                        | <span data-ttu-id="e8d16-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e8d16-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e8d16-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8d16-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e8d16-112">Policy.Read.PermissionGrant, Policy.ReadWrite.PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="e8d16-112">Policy.Read.PermissionGrant, Policy.ReadWrite.PermissionGrant</span></span> |
| <span data-ttu-id="e8d16-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8d16-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8d16-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8d16-114">Not supported.</span></span> |
| <span data-ttu-id="e8d16-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8d16-115">Application</span></span>                            | <span data-ttu-id="e8d16-116">Policy.Read.PermissionGrant, Policy.ReadWrite.PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="e8d16-116">Policy.Read.PermissionGrant, Policy.ReadWrite.PermissionGrant</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8d16-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8d16-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/permissionGrantPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e8d16-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e8d16-118">Optional query parameters</span></span>

<span data-ttu-id="e8d16-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e8d16-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e8d16-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e8d16-120">Request headers</span></span>

| <span data-ttu-id="e8d16-121">Nome</span><span class="sxs-lookup"><span data-stu-id="e8d16-121">Name</span></span>           | <span data-ttu-id="e8d16-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8d16-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="e8d16-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e8d16-123">Authorization</span></span>  | <span data-ttu-id="e8d16-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8d16-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e8d16-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8d16-126">Request body</span></span>

<span data-ttu-id="e8d16-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e8d16-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8d16-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8d16-128">Response</span></span>

<span data-ttu-id="e8d16-129">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção [de objetos permissionGrantPolicy](../resources/permissiongrantpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e8d16-129">If successful, this method returns a `200 OK` response code and a collection of [permissionGrantPolicy](../resources/permissiongrantpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e8d16-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e8d16-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e8d16-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8d16-131">Request</span></span>

<span data-ttu-id="e8d16-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e8d16-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e8d16-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="e8d16-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_permissiongrantpolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/permissionGrantPolicies
```
# <a name="c"></a>[<span data-ttu-id="e8d16-134">C#</span><span class="sxs-lookup"><span data-stu-id="e8d16-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-permissiongrantpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e8d16-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e8d16-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-permissiongrantpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e8d16-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e8d16-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-permissiongrantpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e8d16-137">Java</span><span class="sxs-lookup"><span data-stu-id="e8d16-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-permissiongrantpolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e8d16-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8d16-138">Response</span></span>

<span data-ttu-id="e8d16-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e8d16-139">The following is an example of the response.</span></span>

> <span data-ttu-id="e8d16-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e8d16-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permissionGrantPolicy",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "tier-1",
      "displayName": "Tier 1 Help Desk",
      "description": "Custom permission grant policy for tier 1 help desk.",
      "includes": [
        {
          "id": "198d8d6b-ecf6-47bc-a3dd-eaa2fe0544c5",
          "permissionClassification": "low",
          "permissionType": "delegated",
          "resourceApplication": "any",
          "permissions": [ "all" ],
          "clientApplicationIds": [ "all" ],
          "clientApplicationTenantIds": [ "all" ],
          "clientApplicationPublisherIds": [ "all" ],
          "clientApplicationsFromVerifiedPublisherOnly": true
        }
      ],
      "excludes": []
    },
    {
      "id": "microsoft-company-admin",
      "displayName": "Company Admin Policy",
      "description": "Permissions consentable by Company Administrators.",
      "includes": [
        {
          "id": "1f06f3a1-42d3-4243-8fbc-5d0c30d4de4c",
          "permissionClassification": "all",
          "permissionType": "application",
          "resourceApplication": "any",
          "permissions": [ "all" ],
          "clientApplicationIds": [ "all" ],
          "clientApplicationTenantIds": [ "all" ],
          "clientApplicationPublisherIds": [ "all" ],
          "clientApplicationsFromVerifiedPublisherOnly": false
        },
        {
          "id": "08619a19-ae6f-406c-b9a0-ea6af1f1558d",
          "permissionClassification": "all",
          "permissionType": "delegated",
          "resourceApplication": "any",
          "permissions": [ "all" ],
          "clientApplicationIds": [ "all" ],
          "clientApplicationTenantIds": [ "all" ],
          "clientApplicationPublisherIds": [ "all" ],
          "clientApplicationsFromVerifiedPublisherOnly": false
        }
      ],
      "excludes": []
    }
  ]
}
```
