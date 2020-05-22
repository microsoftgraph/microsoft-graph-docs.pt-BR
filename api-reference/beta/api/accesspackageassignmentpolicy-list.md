---
title: Listar accessPackageAssignmentPolicies
description: Recupere uma lista de objetos accessPackageAssignmentPolicy.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0ba846a7e5dc407db52cf4f343444cb7f84fd5f6
ms.sourcegitcommit: c1935e442ee973c6c3fcb01a15d76bcfa625362e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/22/2020
ms.locfileid: "44345195"
---
# <a name="list-accesspackageassignmentpolicies"></a><span data-ttu-id="135d1-103">Listar accessPackageAssignmentPolicies</span><span class="sxs-lookup"><span data-stu-id="135d1-103">List accessPackageAssignmentPolicies</span></span>

<span data-ttu-id="135d1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="135d1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="135d1-105">No [Gerenciamento de direitos do Azure ad](../resources/entitlementmanagement-root.md), recupere uma lista de objetos [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="135d1-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve a list of [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) objects.</span></span>   <span data-ttu-id="135d1-106">A lista resultante inclui todas as políticas de atribuição às quais o chamador tem acesso para leitura, entre todos os catálogos e pacotes de acesso.</span><span class="sxs-lookup"><span data-stu-id="135d1-106">The resulting list includes all the assignment policies which the caller has access to read, across all catalogs and access packages.</span></span>

## <a name="permissions"></a><span data-ttu-id="135d1-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="135d1-107">Permissions</span></span>

<span data-ttu-id="135d1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="135d1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="135d1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="135d1-110">Permission type</span></span>                        | <span data-ttu-id="135d1-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="135d1-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="135d1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="135d1-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="135d1-113">EntitlementManagement. Read. All, EntitlementManagement. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="135d1-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="135d1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="135d1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="135d1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="135d1-115">Not supported.</span></span> |
| <span data-ttu-id="135d1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="135d1-116">Application</span></span>                            | <span data-ttu-id="135d1-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="135d1-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="135d1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="135d1-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="135d1-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="135d1-119">Optional query parameters</span></span>

<span data-ttu-id="135d1-120">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="135d1-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="135d1-121">Por exemplo, para recuperar uma política de atribuição de pacote do Access com um nome de exibição especificado, inclua `$filter=displayName eq 'Employee sales support'` na consulta.</span><span class="sxs-lookup"><span data-stu-id="135d1-121">For example, to retrieve a access package assignment policy with a specified display name, include `$filter=displayName eq 'Employee sales support'` in the query.</span></span> <span data-ttu-id="135d1-122">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="135d1-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="135d1-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="135d1-123">Request headers</span></span>

| <span data-ttu-id="135d1-124">Nome</span><span class="sxs-lookup"><span data-stu-id="135d1-124">Name</span></span>      |<span data-ttu-id="135d1-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="135d1-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="135d1-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="135d1-126">Authorization</span></span> | <span data-ttu-id="135d1-127">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="135d1-127">Bearer \{token\}.</span></span> <span data-ttu-id="135d1-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="135d1-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="135d1-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="135d1-129">Request body</span></span>

<span data-ttu-id="135d1-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="135d1-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="135d1-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="135d1-131">Response</span></span>

<span data-ttu-id="135d1-132">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="135d1-132">If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="135d1-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="135d1-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="135d1-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="135d1-134">Request</span></span>

<span data-ttu-id="135d1-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="135d1-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="135d1-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="135d1-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentpolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
```
# <a name="c"></a>[<span data-ttu-id="135d1-137">C#</span><span class="sxs-lookup"><span data-stu-id="135d1-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="135d1-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="135d1-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="135d1-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="135d1-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="135d1-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="135d1-140">Response</span></span>

<span data-ttu-id="135d1-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="135d1-141">The following is an example of the response.</span></span>

> <span data-ttu-id="135d1-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="135d1-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentPolicy",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "b2eba9a1-b357-42ee-83a8-336522ed6cbf",
      "accessPackageId": "1b153a13-76da-4d07-9afa-c6c2b1f2e824",
      "displayName": "All Users",
      "description": "All users can request for access to the directory.",
      "canExtend": false,
      "durationInDays": 365,
      "accessReviewSettings": null
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageAssignmentPolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
