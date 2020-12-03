---
title: Listar permissionGrantPolicies
description: Recupere uma lista de objetos permissionGrantPolicy.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 755d2146907c77baa342a0f1b8abd4ea32b87df4
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524266"
---
# <a name="list-permissiongrantpolicies"></a><span data-ttu-id="f72a0-103">Listar permissionGrantPolicies</span><span class="sxs-lookup"><span data-stu-id="f72a0-103">List permissionGrantPolicies</span></span>

<span data-ttu-id="f72a0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f72a0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f72a0-105">Recupere a lista de objetos [permissionGrantPolicy](../resources/permissiongrantpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="f72a0-105">Retrieve the list of [permissionGrantPolicy](../resources/permissiongrantpolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="f72a0-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="f72a0-106">Permissions</span></span>

<span data-ttu-id="f72a0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f72a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f72a0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f72a0-109">Permission type</span></span>                        | <span data-ttu-id="f72a0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f72a0-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f72a0-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f72a0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f72a0-112">Policy. Read. PermissionGrant, Policy. ReadWrite. PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="f72a0-112">Policy.Read.PermissionGrant, Policy.ReadWrite.PermissionGrant</span></span> |
| <span data-ttu-id="f72a0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f72a0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f72a0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f72a0-114">Not supported.</span></span> |
| <span data-ttu-id="f72a0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f72a0-115">Application</span></span>                            | <span data-ttu-id="f72a0-116">Policy. Read. PermissionGrant, Policy. ReadWrite. PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="f72a0-116">Policy.Read.PermissionGrant, Policy.ReadWrite.PermissionGrant</span></span> |

## <a name="http-request"></a><span data-ttu-id="f72a0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f72a0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/permissionGrantPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f72a0-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f72a0-118">Optional query parameters</span></span>

<span data-ttu-id="f72a0-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f72a0-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f72a0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f72a0-120">Request headers</span></span>

| <span data-ttu-id="f72a0-121">Nome</span><span class="sxs-lookup"><span data-stu-id="f72a0-121">Name</span></span>           | <span data-ttu-id="f72a0-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f72a0-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="f72a0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f72a0-123">Authorization</span></span>  | <span data-ttu-id="f72a0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f72a0-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f72a0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f72a0-126">Request body</span></span>

<span data-ttu-id="f72a0-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f72a0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f72a0-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f72a0-128">Response</span></span>

<span data-ttu-id="f72a0-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [permissionGrantPolicy](../resources/permissiongrantpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f72a0-129">If successful, this method returns a `200 OK` response code and a collection of [permissionGrantPolicy](../resources/permissiongrantpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f72a0-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f72a0-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f72a0-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f72a0-131">Request</span></span>

<span data-ttu-id="f72a0-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f72a0-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f72a0-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f72a0-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_permissiongrantpolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/permissionGrantPolicies
```
# <a name="c"></a>[<span data-ttu-id="f72a0-134">C#</span><span class="sxs-lookup"><span data-stu-id="f72a0-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-permissiongrantpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f72a0-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f72a0-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-permissiongrantpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f72a0-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f72a0-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-permissiongrantpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f72a0-137">Java</span><span class="sxs-lookup"><span data-stu-id="f72a0-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-permissiongrantpolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f72a0-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="f72a0-138">Response</span></span>

<span data-ttu-id="f72a0-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f72a0-139">The following is an example of the response.</span></span>

> <span data-ttu-id="f72a0-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f72a0-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
