---
title: Lista inclui coleção de permissionGrantPolicy
description: Recupere uma lista dos conjuntos de condições que descrevem as condições nas quais um evento de concessão de permissão está incluído em uma política de concessão de permissão.
localization_priority: Normal
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 1d82b31dc657a05233cc41a068bad205bb6a6e14
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433933"
---
# <a name="list-includes-collection-of-permissiongrantpolicy"></a><span data-ttu-id="71b4f-103">Lista inclui coleção de permissionGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="71b4f-103">List includes collection of permissionGrantPolicy</span></span>

<span data-ttu-id="71b4f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71b4f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71b4f-105">Recupere os conjuntos de condições *incluídos em* [uma permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="71b4f-105">Retrieve the condition sets which are *included* in a [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="71b4f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="71b4f-106">Permissions</span></span>

<span data-ttu-id="71b4f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71b4f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71b4f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="71b4f-109">Permission type</span></span>      | <span data-ttu-id="71b4f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="71b4f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71b4f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="71b4f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="71b4f-112">Policy.Read.PermissionGrant, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="71b4f-112">Policy.Read.PermissionGrant, Directory.Read.All</span></span> |
|<span data-ttu-id="71b4f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="71b4f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71b4f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="71b4f-114">Not supported.</span></span>    |
|<span data-ttu-id="71b4f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="71b4f-115">Application</span></span> | <span data-ttu-id="71b4f-116">Policy.Read.PermissionGrant, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="71b4f-116">Policy.Read.PermissionGrant, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="71b4f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="71b4f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /policies/permissionGrantPolicies/{id}/includes
```

## <a name="optional-query-parameters"></a><span data-ttu-id="71b4f-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="71b4f-118">Optional query parameters</span></span>

<span data-ttu-id="71b4f-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="71b4f-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="71b4f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="71b4f-120">Request headers</span></span>

| <span data-ttu-id="71b4f-121">Nome</span><span class="sxs-lookup"><span data-stu-id="71b4f-121">Name</span></span>           | <span data-ttu-id="71b4f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="71b4f-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="71b4f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="71b4f-123">Authorization</span></span>  | <span data-ttu-id="71b4f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="71b4f-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="71b4f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="71b4f-126">Request body</span></span>

<span data-ttu-id="71b4f-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="71b4f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71b4f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="71b4f-128">Response</span></span>

<span data-ttu-id="71b4f-129">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção [de objetos permissionGrantConditionSet](../resources/permissiongrantconditionset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="71b4f-129">If successful, this method returns a `200 OK` response code and a collection of [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71b4f-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="71b4f-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="71b4f-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="71b4f-131">Request</span></span>

<span data-ttu-id="71b4f-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="71b4f-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="71b4f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="71b4f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "permissiongrantpolicy_get_includes"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/permissionGrantPolicies/microsoft-application-admin/includes
```
# <a name="c"></a>[<span data-ttu-id="71b4f-134">C#</span><span class="sxs-lookup"><span data-stu-id="71b4f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/permissiongrantpolicy-get-includes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="71b4f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="71b4f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/permissiongrantpolicy-get-includes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="71b4f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="71b4f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/permissiongrantpolicy-get-includes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="71b4f-137">Java</span><span class="sxs-lookup"><span data-stu-id="71b4f-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/permissiongrantpolicy-get-includes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="71b4f-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="71b4f-138">Response</span></span>

<span data-ttu-id="71b4f-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="71b4f-139">The following is an example of the response.</span></span>

> <span data-ttu-id="71b4f-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="71b4f-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
