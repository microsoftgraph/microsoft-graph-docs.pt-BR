---
title: Obter accessPackageAssignmentResourceRole
description: Recupere as propriedades e as relações de um objeto accessPackageAssignmentResourceRole.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 82ff4afdf94001cb807cdd7e2e7840a98a5d209f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048586"
---
# <a name="get-accesspackageassignmentresourcerole"></a><span data-ttu-id="213f9-103">Obter accessPackageAssignmentResourceRole</span><span class="sxs-lookup"><span data-stu-id="213f9-103">Get accessPackageAssignmentResourceRole</span></span>

<span data-ttu-id="213f9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="213f9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="213f9-105">Recupere as propriedades e as relações de um [objeto accessPackageAssignmentResourceRole.](../resources/accesspackageassignmentresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="213f9-105">Retrieve the properties and relationships of an [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="213f9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="213f9-106">Permissions</span></span>

<span data-ttu-id="213f9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="213f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="213f9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="213f9-109">Permission type</span></span>                        | <span data-ttu-id="213f9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="213f9-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="213f9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="213f9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="213f9-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="213f9-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="213f9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="213f9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="213f9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="213f9-114">Not supported.</span></span> |
| <span data-ttu-id="213f9-115">Application</span><span class="sxs-lookup"><span data-stu-id="213f9-115">Application</span></span>                            | <span data-ttu-id="213f9-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="213f9-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="213f9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="213f9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentResourceRoles/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="213f9-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="213f9-118">Optional query parameters</span></span>

<span data-ttu-id="213f9-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="213f9-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="213f9-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="213f9-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="213f9-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="213f9-121">Request headers</span></span>

| <span data-ttu-id="213f9-122">Nome</span><span class="sxs-lookup"><span data-stu-id="213f9-122">Name</span></span>      |<span data-ttu-id="213f9-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="213f9-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="213f9-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="213f9-124">Authorization</span></span> | <span data-ttu-id="213f9-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="213f9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="213f9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="213f9-127">Request body</span></span>

<span data-ttu-id="213f9-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="213f9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="213f9-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="213f9-129">Response</span></span>

<span data-ttu-id="213f9-130">Se tiver êxito, este método retornará um código de resposta e o `200 OK` [objeto accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="213f9-130">If successful, this method returns a `200 OK` response code and the requested [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="213f9-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="213f9-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="213f9-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="213f9-132">Request</span></span>

<span data-ttu-id="213f9-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="213f9-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="213f9-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="213f9-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentresourcerole"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentResourceRoles/{id}
```
# <a name="c"></a>[<span data-ttu-id="213f9-135">C#</span><span class="sxs-lookup"><span data-stu-id="213f9-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentresourcerole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="213f9-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="213f9-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentresourcerole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="213f9-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="213f9-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentresourcerole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="213f9-138">Java</span><span class="sxs-lookup"><span data-stu-id="213f9-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageassignmentresourcerole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="213f9-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="213f9-139">Response</span></span>

<span data-ttu-id="213f9-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="213f9-140">The following is an example of the response.</span></span>

> <span data-ttu-id="213f9-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="213f9-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentResourceRole"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "1bf101d2-4d9c-437f-bbf5-3d13d98f5479",
  "originId": "originId-value",
  "originSystem": "SharePointOnline",
  "status": "Fulfilled"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get accessPackageAssignmentResourceRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


