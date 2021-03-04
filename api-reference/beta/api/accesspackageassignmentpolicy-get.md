---
title: Obter accessPackageAssignmentPolicy
description: Recupere as propriedades e as relações de um objeto accessPackageAassignmentPolicy.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 8ab969653cd9787ed51a9269fa9060b2e2e07d9c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439727"
---
# <a name="get-accesspackageassignmentpolicy"></a><span data-ttu-id="17bbe-103">Obter accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="17bbe-103">Get accessPackageAssignmentPolicy</span></span>

<span data-ttu-id="17bbe-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17bbe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17bbe-105">No gerenciamento de direitos do [Azure AD,](../resources/entitlementmanagement-root.md)recupere as propriedades e as relações de um [objeto accessPackageAssignmentPolicy.](../resources/accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="17bbe-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve the properties and relationships of an [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="17bbe-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="17bbe-106">Permissions</span></span>

<span data-ttu-id="17bbe-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17bbe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="17bbe-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="17bbe-109">Permission type</span></span>                        | <span data-ttu-id="17bbe-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="17bbe-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="17bbe-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="17bbe-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="17bbe-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17bbe-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="17bbe-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="17bbe-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="17bbe-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="17bbe-114">Not supported.</span></span> |
| <span data-ttu-id="17bbe-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="17bbe-115">Application</span></span>                            | <span data-ttu-id="17bbe-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17bbe-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="17bbe-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="17bbe-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="17bbe-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="17bbe-118">Optional query parameters</span></span>

<span data-ttu-id="17bbe-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="17bbe-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="17bbe-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="17bbe-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="17bbe-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="17bbe-121">Request headers</span></span>

| <span data-ttu-id="17bbe-122">Nome</span><span class="sxs-lookup"><span data-stu-id="17bbe-122">Name</span></span>      |<span data-ttu-id="17bbe-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="17bbe-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="17bbe-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="17bbe-124">Authorization</span></span> | <span data-ttu-id="17bbe-125">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="17bbe-125">Bearer \{token\}.</span></span> <span data-ttu-id="17bbe-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="17bbe-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="17bbe-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="17bbe-127">Request body</span></span>

<span data-ttu-id="17bbe-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="17bbe-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="17bbe-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="17bbe-129">Response</span></span>

<span data-ttu-id="17bbe-130">Se tiver êxito, este método retornará um código de resposta e `200 OK` o [objeto accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="17bbe-130">If successful, this method returns a `200 OK` response code and the requested [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="17bbe-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="17bbe-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="17bbe-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="17bbe-132">Request</span></span>

<span data-ttu-id="17bbe-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="17bbe-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="17bbe-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="17bbe-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentpolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="17bbe-135">C#</span><span class="sxs-lookup"><span data-stu-id="17bbe-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="17bbe-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="17bbe-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="17bbe-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="17bbe-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="17bbe-138">Java</span><span class="sxs-lookup"><span data-stu-id="17bbe-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageassignmentpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="17bbe-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="17bbe-139">Response</span></span>

<span data-ttu-id="17bbe-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="17bbe-140">The following is an example of the response.</span></span>

> <span data-ttu-id="17bbe-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="17bbe-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "b2eba9a1-b357-42ee-83a8-336522ed6cbf",
  "accessPackageId": "1b153a13-76da-4d07-9afa-c6c2b1f2e824",
  "displayName": "All Users",
  "description": "All users in the directory can request access.",
  "canExtend": false,
  "durationInDays": 365,
  "accessReviewSettings": null
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get accessPackageAssignmentPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


