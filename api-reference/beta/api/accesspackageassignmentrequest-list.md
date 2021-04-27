---
title: Listar accessPackageAssignmentRequests
description: Recupere uma lista de objetos accessPackageAssignmentRequest.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: c53f900db5f53d3e4cff2d0de17c808b9f80d3a2
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048607"
---
# <a name="list-accesspackageassignmentrequests"></a><span data-ttu-id="9b9af-103">Listar accessPackageAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="9b9af-103">List accessPackageAssignmentRequests</span></span>

<span data-ttu-id="9b9af-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b9af-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b9af-105">No gerenciamento de direitos do [Azure AD,](../resources/entitlementmanagement-root.md)recupere uma lista de objetos [accessPackageAssignmentRequest.](../resources/accesspackageassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="9b9af-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve a list of [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) objects.</span></span>  <span data-ttu-id="9b9af-106">A lista resultante inclui todas as solicitações de atribuição, atuais e bem como expiradas, que o chamador tem acesso à leitura, em todos os catálogos e pacotes de acesso.</span><span class="sxs-lookup"><span data-stu-id="9b9af-106">The resulting list includes all the assignment requests, current and well as expired, that the caller has access to read, across all catalogs and access packages.</span></span>

## <a name="permissions"></a><span data-ttu-id="9b9af-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="9b9af-107">Permissions</span></span>

<span data-ttu-id="9b9af-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b9af-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9b9af-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9b9af-110">Permission type</span></span>                        | <span data-ttu-id="9b9af-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9b9af-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9b9af-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9b9af-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="9b9af-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b9af-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="9b9af-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9b9af-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b9af-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9b9af-115">Not supported.</span></span> |
| <span data-ttu-id="9b9af-116">Application</span><span class="sxs-lookup"><span data-stu-id="9b9af-116">Application</span></span>                            | <span data-ttu-id="9b9af-117">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b9af-117">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9b9af-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9b9af-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9b9af-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9b9af-119">Optional query parameters</span></span>

<span data-ttu-id="9b9af-120">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9b9af-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="9b9af-121">Por exemplo, para recuperar o pacote de acesso de cada solicitação, `$expand=accessPackage` inclua na consulta.</span><span class="sxs-lookup"><span data-stu-id="9b9af-121">For example, to retrieve the access package of each request, include `$expand=accessPackage` in the query.</span></span>  <span data-ttu-id="9b9af-122">Para recuperar apenas solicitações para um pacote de acesso específico, inclua na consulta um filtro como `$expand=accessPackage&$filter=accessPackage/id eq '9bbe5f7d-f1e7-4eb1-a586-38cdf6f8b1ea'` .</span><span class="sxs-lookup"><span data-stu-id="9b9af-122">To retrieve only requests for a specific access package, include in the query a filter such as `$expand=accessPackage&$filter=accessPackage/id eq '9bbe5f7d-f1e7-4eb1-a586-38cdf6f8b1ea'`.</span></span>  <span data-ttu-id="9b9af-123">Para recuperar a atribuição resultante, `$expand=accessPackageAssignment` inclua na consulta.</span><span class="sxs-lookup"><span data-stu-id="9b9af-123">To retrieve the resulting assignment, include `$expand=accessPackageAssignment` in the query.</span></span>
<span data-ttu-id="9b9af-124">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="9b9af-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9b9af-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9b9af-125">Request headers</span></span>

| <span data-ttu-id="9b9af-126">Nome</span><span class="sxs-lookup"><span data-stu-id="9b9af-126">Name</span></span>      |<span data-ttu-id="9b9af-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b9af-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9b9af-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="9b9af-128">Authorization</span></span> | <span data-ttu-id="9b9af-p104">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9b9af-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9b9af-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9b9af-131">Request body</span></span>

<span data-ttu-id="9b9af-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9b9af-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9b9af-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b9af-133">Response</span></span>

<span data-ttu-id="9b9af-134">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9b9af-134">If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9b9af-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9b9af-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9b9af-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9b9af-136">Request</span></span>

<span data-ttu-id="9b9af-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9b9af-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9b9af-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="9b9af-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentrequests"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests
```
# <a name="c"></a>[<span data-ttu-id="9b9af-139">C#</span><span class="sxs-lookup"><span data-stu-id="9b9af-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentrequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9b9af-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9b9af-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentrequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9b9af-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9b9af-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentrequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9b9af-142">Java</span><span class="sxs-lookup"><span data-stu-id="9b9af-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageassignmentrequests-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9b9af-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b9af-143">Response</span></span>

<span data-ttu-id="9b9af-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9b9af-144">The following is an example of the response.</span></span>

> <span data-ttu-id="9b9af-145">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9b9af-145">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "433dafca-5047-4614-95f7-a03510b1ded3",
      "requestType": "AdminAdd",
      "requestState": "Delivered",
      "requestStatus": "Fulfilled",
      "isValidationOnly": false,
      "createdDateTime": "2019-10-25T22:55:11.623Z"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageAssignmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


