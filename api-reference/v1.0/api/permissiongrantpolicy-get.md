---
title: Obter permissionGrantPolicy
description: Recupere um único objeto permissionGrantPolicy.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 9bcd99c04c0bc6149ac5f14d2587776540fe24a6
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524469"
---
# <a name="get-permissiongrantpolicy"></a><span data-ttu-id="7d3b6-103">Obter permissionGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="7d3b6-103">Get permissionGrantPolicy</span></span>

<span data-ttu-id="7d3b6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d3b6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7d3b6-105">Recupere um único objeto [permissionGrantPolicy](../resources/permissiongrantpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="7d3b6-105">Retrieve a single [permissionGrantPolicy](../resources/permissiongrantpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7d3b6-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="7d3b6-106">Permissions</span></span>

<span data-ttu-id="7d3b6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d3b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7d3b6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7d3b6-109">Permission type</span></span>                        | <span data-ttu-id="7d3b6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7d3b6-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7d3b6-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7d3b6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7d3b6-112">Policy. Read. PermissionGrant, Policy. ReadWrite. PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="7d3b6-112">Policy.Read.PermissionGrant, Policy.ReadWrite.PermissionGrant</span></span> |
| <span data-ttu-id="7d3b6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7d3b6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d3b6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d3b6-114">Not supported.</span></span> |
| <span data-ttu-id="7d3b6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d3b6-115">Application</span></span>                            | <span data-ttu-id="7d3b6-116">Policy. Read. PermissionGrant, Policy. ReadWrite. PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="7d3b6-116">Policy.Read.PermissionGrant, Policy.ReadWrite.PermissionGrant</span></span> |

## <a name="http-request"></a><span data-ttu-id="7d3b6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7d3b6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/permissionGrantPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7d3b6-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7d3b6-118">Optional query parameters</span></span>

<span data-ttu-id="7d3b6-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7d3b6-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7d3b6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7d3b6-120">Request headers</span></span>

| <span data-ttu-id="7d3b6-121">Nome</span><span class="sxs-lookup"><span data-stu-id="7d3b6-121">Name</span></span>           | <span data-ttu-id="7d3b6-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d3b6-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="7d3b6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7d3b6-123">Authorization</span></span>  | <span data-ttu-id="7d3b6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7d3b6-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7d3b6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7d3b6-126">Request body</span></span>

<span data-ttu-id="7d3b6-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7d3b6-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7d3b6-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d3b6-128">Response</span></span>

<span data-ttu-id="7d3b6-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [permissionGrantPolicy](../resources/permissiongrantpolicy.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7d3b6-129">If successful, this method returns a `200 OK` response code and the requested [permissionGrantPolicy](../resources/permissiongrantpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7d3b6-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7d3b6-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7d3b6-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7d3b6-131">Request</span></span>

<span data-ttu-id="7d3b6-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7d3b6-132">The following is an example of the request.</span></span>
<span data-ttu-id="7d3b6-133">Neste exemplo, a política solicitada é a política de concessão de permissão interna `microsoft-user-default-low` , que inclui as permissões delegadas baixas, para aplicativos de editores ou aplicativos verificados registrados neste locatário.</span><span class="sxs-lookup"><span data-stu-id="7d3b6-133">In this example, the requested policy is the built-in permission grant policy `microsoft-user-default-low`, which includes delegated permissions classified low, for apps from verified publishers or apps registered in this tenant.</span></span>



# <a name="http"></a>[<span data-ttu-id="7d3b6-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="7d3b6-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_permissiongrantpolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/permissionGrantPolicies/microsoft-user-default-low
```
# <a name="c"></a>[<span data-ttu-id="7d3b6-135">C#</span><span class="sxs-lookup"><span data-stu-id="7d3b6-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-permissiongrantpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7d3b6-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7d3b6-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-permissiongrantpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7d3b6-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7d3b6-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-permissiongrantpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7d3b6-138">Java</span><span class="sxs-lookup"><span data-stu-id="7d3b6-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-permissiongrantpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7d3b6-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d3b6-139">Response</span></span>

<span data-ttu-id="7d3b6-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7d3b6-140">The following is an example of the response.</span></span> <span data-ttu-id="7d3b6-141">A política tem dois `includes` conjuntos de condição, um que corresponde a permissões delegadas classificadas `low` para aplicativos clientes registrados neste locatário e as outras que correspondem a permissões delegadas classificadas `low` para aplicativos de editores verificados (independentemente de qual locatário o aplicativo está registrado).</span><span class="sxs-lookup"><span data-stu-id="7d3b6-141">The policy has two `includes` condition sets, one which matches with delegated permission classified `low` for client apps registered in this tenant, and the other which matches delegated permissions classified `low` for apps from verified publishers (regardless of which tenant the app is registered in).</span></span>

> <span data-ttu-id="7d3b6-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7d3b6-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permissionGrantPolicy",
  "isCollection": false
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "microsoft-user-default-low",
    "displayName": "Default User Low Risk Policy",
    "description": "All low risk permissions are consentable by member type users by default.",
    "includes": [
        {
            "id": "cb0c20dd-919d-40c5-ba6d-7ffb233b4b0b",
            "permissionClassification": "low",
            "permissionType": "delegated",
            "resourceApplication": "any",
            "permissions": [ "all" ],
            "clientApplicationIds": [ "all" ],
            "clientApplicationTenantIds": [ "11e37ee2-48fe-42e0-aab9-07d0bb165353" ],
            "clientApplicationPublisherIds": [ "all" ],
            "clientApplicationsFromVerifiedPublisherOnly": false
        },
        {
            "id": "8ce99f96-730c-4ebd-8397-07ee65942b97",
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
}
```
