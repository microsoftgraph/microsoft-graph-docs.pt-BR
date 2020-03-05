---
title: Obter accessPackageAssignmentResourceRole
description: Recupere as propriedades e os relacionamentos de um objeto accessPackageAssignmentResourceRole.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ae44a167d7e89ac659e816e5ebe90d1995b5258b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42442002"
---
# <a name="get-accesspackageassignmentresourcerole"></a><span data-ttu-id="8e29a-103">Obter accessPackageAssignmentResourceRole</span><span class="sxs-lookup"><span data-stu-id="8e29a-103">Get accessPackageAssignmentResourceRole</span></span>

<span data-ttu-id="8e29a-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8e29a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e29a-105">Recupere as propriedades e os relacionamentos de um objeto [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) .</span><span class="sxs-lookup"><span data-stu-id="8e29a-105">Retrieve the properties and relationships of an [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8e29a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8e29a-106">Permissions</span></span>

<span data-ttu-id="8e29a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e29a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8e29a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8e29a-109">Permission type</span></span>                        | <span data-ttu-id="8e29a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8e29a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8e29a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8e29a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8e29a-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e29a-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="8e29a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8e29a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e29a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8e29a-114">Not supported.</span></span> |
| <span data-ttu-id="8e29a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8e29a-115">Application</span></span>                            | <span data-ttu-id="8e29a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8e29a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8e29a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8e29a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentResourceRoles/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8e29a-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8e29a-118">Optional query parameters</span></span>

<span data-ttu-id="8e29a-119">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8e29a-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="8e29a-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="8e29a-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="8e29a-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8e29a-121">Request headers</span></span>

| <span data-ttu-id="8e29a-122">Nome</span><span class="sxs-lookup"><span data-stu-id="8e29a-122">Name</span></span>      |<span data-ttu-id="8e29a-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e29a-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8e29a-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="8e29a-124">Authorization</span></span> | <span data-ttu-id="8e29a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8e29a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8e29a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8e29a-127">Request body</span></span>

<span data-ttu-id="8e29a-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8e29a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8e29a-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e29a-129">Response</span></span>

<span data-ttu-id="8e29a-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8e29a-130">If successful, this method returns a `200 OK` response code and the requested [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8e29a-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8e29a-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8e29a-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8e29a-132">Request</span></span>

<span data-ttu-id="8e29a-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8e29a-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8e29a-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e29a-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentresourcerole"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentResourceRoles/{id}
```
# <a name="c"></a>[<span data-ttu-id="8e29a-135">C#</span><span class="sxs-lookup"><span data-stu-id="8e29a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentresourcerole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8e29a-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e29a-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentresourcerole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8e29a-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8e29a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentresourcerole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8e29a-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e29a-138">Response</span></span>

<span data-ttu-id="8e29a-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8e29a-139">The following is an example of the response.</span></span>

> <span data-ttu-id="8e29a-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8e29a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
