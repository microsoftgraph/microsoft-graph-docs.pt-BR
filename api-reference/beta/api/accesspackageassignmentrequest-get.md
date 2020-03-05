---
title: Obter accessPackageAssignmentRequest
description: Recupere as propriedades e os relacionamentos de um objeto accessPackageAssignmentRequest.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 285badec81e03f4dc71b3fcf479152a7ae39f484
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448435"
---
# <a name="get-accesspackageassignmentrequest"></a><span data-ttu-id="d4b56-103">Obter accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="d4b56-103">Get accessPackageAssignmentRequest</span></span>

<span data-ttu-id="d4b56-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d4b56-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4b56-105">No [Azure ad pretitulation Management](../resources/entitlementmanagement-root.md), recupere as propriedades e os relacionamentos de um objeto [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="d4b56-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve the properties and relationships of an  [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d4b56-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d4b56-106">Permissions</span></span>

<span data-ttu-id="d4b56-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4b56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d4b56-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d4b56-109">Permission type</span></span>                        | <span data-ttu-id="d4b56-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d4b56-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d4b56-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d4b56-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d4b56-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4b56-112">EntitlementManagement.ReadWrite.All</span></span>  |
| <span data-ttu-id="d4b56-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d4b56-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4b56-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d4b56-114">Not supported.</span></span> |
| <span data-ttu-id="d4b56-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d4b56-115">Application</span></span>                            | <span data-ttu-id="d4b56-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d4b56-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d4b56-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d4b56-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d4b56-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d4b56-118">Optional query parameters</span></span>

<span data-ttu-id="d4b56-119">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d4b56-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="d4b56-120">Por exemplo, para recuperar o pacote do Access que foi solicitado, `$expand=accessPackage` inclua na consulta.</span><span class="sxs-lookup"><span data-stu-id="d4b56-120">For example, to retrieve the access package that was requested, include `$expand=accessPackage` in the query.</span></span> <span data-ttu-id="d4b56-121">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="d4b56-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d4b56-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d4b56-122">Request headers</span></span>

| <span data-ttu-id="d4b56-123">Nome</span><span class="sxs-lookup"><span data-stu-id="d4b56-123">Name</span></span>      |<span data-ttu-id="d4b56-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4b56-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d4b56-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="d4b56-125">Authorization</span></span> | <span data-ttu-id="d4b56-126">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="d4b56-126">Bearer \{token\}.</span></span> <span data-ttu-id="d4b56-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d4b56-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d4b56-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d4b56-128">Request body</span></span>

<span data-ttu-id="d4b56-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d4b56-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d4b56-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4b56-130">Response</span></span>

<span data-ttu-id="d4b56-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d4b56-131">If successful, this method returns a `200 OK` response code and the requested [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d4b56-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d4b56-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d4b56-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d4b56-133">Request</span></span>

<span data-ttu-id="d4b56-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d4b56-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d4b56-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="d4b56-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{id}
```
# <a name="c"></a>[<span data-ttu-id="d4b56-136">C#</span><span class="sxs-lookup"><span data-stu-id="d4b56-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d4b56-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d4b56-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d4b56-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d4b56-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d4b56-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4b56-139">Response</span></span>

<span data-ttu-id="d4b56-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d4b56-140">The following is an example of the response.</span></span>

> <span data-ttu-id="d4b56-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d4b56-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "433dafca-5047-4614-95f7-a03510b1ded3",
  "requestType": "AdminAdd",
  "requestState": "Delivered",
  "requestStatus": "Fulfilled",
  "isValidationOnly": false,
  "createdDateTime": "2019-10-25T22:55:11.623Z"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get accessPackageAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
