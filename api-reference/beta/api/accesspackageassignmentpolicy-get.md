---
title: Obter accessPackageAssignmentPolicy
description: Recupere as propriedades e os relacionamentos de um objeto accessPackageAassignmentPolicy.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: cebad5285d9c45c1c5bade244f83e23e6b16bd77
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331168"
---
# <a name="get-accesspackageassignmentpolicy"></a><span data-ttu-id="f9b24-103">Obter accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="f9b24-103">Get accessPackageAssignmentPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9b24-104">No [Azure ad pretitulation Management](../resources/entitlementmanagement-root.md), recupere as propriedades e os relacionamentos de um objeto [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="f9b24-104">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve the properties and relationships of an [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f9b24-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f9b24-105">Permissions</span></span>

<span data-ttu-id="f9b24-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9b24-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f9b24-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f9b24-108">Permission type</span></span>                        | <span data-ttu-id="f9b24-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f9b24-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f9b24-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f9b24-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f9b24-111">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9b24-111">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="f9b24-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f9b24-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9b24-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9b24-113">Not supported.</span></span> |
| <span data-ttu-id="f9b24-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f9b24-114">Application</span></span>                            | <span data-ttu-id="f9b24-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9b24-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f9b24-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f9b24-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f9b24-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f9b24-117">Optional query parameters</span></span>

<span data-ttu-id="f9b24-118">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f9b24-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="f9b24-119">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f9b24-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f9b24-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f9b24-120">Request headers</span></span>

| <span data-ttu-id="f9b24-121">Nome</span><span class="sxs-lookup"><span data-stu-id="f9b24-121">Name</span></span>      |<span data-ttu-id="f9b24-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9b24-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f9b24-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f9b24-123">Authorization</span></span> | <span data-ttu-id="f9b24-124">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="f9b24-124">Bearer \{token\}.</span></span> <span data-ttu-id="f9b24-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f9b24-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f9b24-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f9b24-126">Request body</span></span>

<span data-ttu-id="f9b24-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f9b24-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f9b24-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9b24-128">Response</span></span>

<span data-ttu-id="f9b24-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f9b24-129">If successful, this method returns a `200 OK` response code and the requested [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f9b24-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f9b24-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f9b24-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f9b24-131">Request</span></span>

<span data-ttu-id="f9b24-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f9b24-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f9b24-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f9b24-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentpolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="f9b24-134">C#</span><span class="sxs-lookup"><span data-stu-id="f9b24-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f9b24-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f9b24-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f9b24-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f9b24-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f9b24-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9b24-137">Response</span></span>

<span data-ttu-id="f9b24-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f9b24-138">The following is an example of the response.</span></span>

> <span data-ttu-id="f9b24-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f9b24-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "All users can request for access to the directory.",
  "isDenyPolicy": false,
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
