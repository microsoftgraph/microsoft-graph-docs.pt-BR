---
title: Lista inclui coleção de permissionGrantPolicy
description: Recupere uma lista dos conjuntos de condições que descrevem as condições nas quais um evento de concessão de permissão está incluído em uma política de concessão de permissão.
localization_priority: Normal
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: c1fc71f56c662b1558d11fe10404a67395fb4813
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055411"
---
# <a name="list-includes-collection-of-permissiongrantpolicy"></a><span data-ttu-id="2ec14-103">Lista inclui coleção de permissionGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="2ec14-103">List includes collection of permissionGrantPolicy</span></span>

<span data-ttu-id="2ec14-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ec14-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ec14-105">Recupere os conjuntos de condições *incluídos em* [uma permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2ec14-105">Retrieve the condition sets which are *included* in a [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2ec14-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2ec14-106">Permissions</span></span>

<span data-ttu-id="2ec14-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ec14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ec14-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2ec14-109">Permission type</span></span>      | <span data-ttu-id="2ec14-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2ec14-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2ec14-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2ec14-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2ec14-112">Policy.Read.PermissionGrant, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="2ec14-112">Policy.Read.PermissionGrant, Directory.Read.All</span></span> |
|<span data-ttu-id="2ec14-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2ec14-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ec14-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ec14-114">Not supported.</span></span>    |
|<span data-ttu-id="2ec14-115">Application</span><span class="sxs-lookup"><span data-stu-id="2ec14-115">Application</span></span> | <span data-ttu-id="2ec14-116">Policy.Read.PermissionGrant, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="2ec14-116">Policy.Read.PermissionGrant, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2ec14-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2ec14-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /policies/permissionGrantPolicies/{id}/includes
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2ec14-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2ec14-118">Optional query parameters</span></span>

<span data-ttu-id="2ec14-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2ec14-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2ec14-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2ec14-120">Request headers</span></span>

| <span data-ttu-id="2ec14-121">Nome</span><span class="sxs-lookup"><span data-stu-id="2ec14-121">Name</span></span>           | <span data-ttu-id="2ec14-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ec14-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="2ec14-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2ec14-123">Authorization</span></span>  | <span data-ttu-id="2ec14-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2ec14-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2ec14-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2ec14-126">Request body</span></span>

<span data-ttu-id="2ec14-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2ec14-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ec14-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ec14-128">Response</span></span>

<span data-ttu-id="2ec14-129">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção [de objetos permissionGrantConditionSet](../resources/permissiongrantconditionset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2ec14-129">If successful, this method returns a `200 OK` response code and a collection of [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ec14-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2ec14-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2ec14-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2ec14-131">Request</span></span>

<span data-ttu-id="2ec14-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2ec14-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2ec14-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ec14-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "permissiongrantpolicy_get_includes"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/permissionGrantPolicies/microsoft-application-admin/includes
```
# <a name="c"></a>[<span data-ttu-id="2ec14-134">C#</span><span class="sxs-lookup"><span data-stu-id="2ec14-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/permissiongrantpolicy-get-includes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2ec14-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ec14-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/permissiongrantpolicy-get-includes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2ec14-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2ec14-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/permissiongrantpolicy-get-includes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2ec14-137">Java</span><span class="sxs-lookup"><span data-stu-id="2ec14-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/permissiongrantpolicy-get-includes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2ec14-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ec14-138">Response</span></span>

<span data-ttu-id="2ec14-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2ec14-139">The following is an example of the response.</span></span>

> <span data-ttu-id="2ec14-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2ec14-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permissionGrantConditionSet",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "811d2da7-443c-43da-96e7-28d285b234e9",
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
      "id": "60461179-740e-4d8b-9e00-1456a338c44b",
      "permissionClassification": "all",
      "permissionType": "delegated",
      "resourceApplication": "any",
      "permissions": [ "all" ],
      "clientApplicationIds": [ "all" ],
      "clientApplicationTenantIds": [ "all" ],
      "clientApplicationPublisherIds": [ "all" ],
      "clientApplicationsFromVerifiedPublisherOnly": false
    }
  ]
}
```
