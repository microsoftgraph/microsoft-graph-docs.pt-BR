---
title: Listar accessPackageAssignmentRequests
description: Recupere uma lista de objetos accessPackageAssignmentRequest.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: d5ce1ca824f104de9058be4ed748d5b87a731e71
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2021
ms.locfileid: "53466933"
---
# <a name="list-accesspackageassignmentrequests"></a><span data-ttu-id="0f48f-103">Listar accessPackageAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="0f48f-103">List accessPackageAssignmentRequests</span></span>

<span data-ttu-id="0f48f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f48f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f48f-105">No gerenciamento de direitos do [Azure AD,](../resources/entitlementmanagement-root.md)recupere uma lista de objetos [accessPackageAssignmentRequest.](../resources/accesspackageassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="0f48f-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve a list of [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) objects.</span></span>  <span data-ttu-id="0f48f-106">A lista resultante inclui todas as solicitações de atribuição, atuais e bem como expiradas, que o chamador tem acesso à leitura, em todos os catálogos e pacotes de acesso.</span><span class="sxs-lookup"><span data-stu-id="0f48f-106">The resulting list includes all the assignment requests, current and well as expired, that the caller has access to read, across all catalogs and access packages.</span></span>

## <a name="permissions"></a><span data-ttu-id="0f48f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="0f48f-107">Permissions</span></span>

<span data-ttu-id="0f48f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f48f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0f48f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0f48f-110">Permission type</span></span>                        | <span data-ttu-id="0f48f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0f48f-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0f48f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0f48f-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="0f48f-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f48f-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="0f48f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0f48f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f48f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f48f-115">Not supported.</span></span> |
| <span data-ttu-id="0f48f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0f48f-116">Application</span></span>                            | <span data-ttu-id="0f48f-117">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f48f-117">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0f48f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0f48f-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0f48f-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0f48f-119">Optional query parameters</span></span>

<span data-ttu-id="0f48f-120">Este método dá suporte aos `$expand` `$filter` parâmetros de consulta E OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0f48f-120">This method supports the `$expand` and `$filter` OData query parameters to help customize the response.</span></span> <span data-ttu-id="0f48f-121">Por exemplo, para recuperar o pacote de acesso de cada solicitação, `$expand=accessPackage` inclua na consulta.</span><span class="sxs-lookup"><span data-stu-id="0f48f-121">For example, to retrieve the access package of each request, include `$expand=accessPackage` in the query.</span></span>  <span data-ttu-id="0f48f-122">Para recuperar apenas solicitações para um pacote de acesso específico, inclua na consulta um filtro como `$expand=accessPackage&$filter=accessPackage/id eq '9bbe5f7d-f1e7-4eb1-a586-38cdf6f8b1ea'` .</span><span class="sxs-lookup"><span data-stu-id="0f48f-122">To retrieve only requests for a specific access package, include in the query a filter such as `$expand=accessPackage&$filter=accessPackage/id eq '9bbe5f7d-f1e7-4eb1-a586-38cdf6f8b1ea'`.</span></span>  <span data-ttu-id="0f48f-123">Para recuperar a atribuição resultante, `$expand=accessPackageAssignment` inclua na consulta.</span><span class="sxs-lookup"><span data-stu-id="0f48f-123">To retrieve the resulting assignment, include `$expand=accessPackageAssignment` in the query.</span></span>  <span data-ttu-id="0f48f-124">Para obter mais detalhes sobre o solicitante, `$expand=requestor` inclua na consulta.</span><span class="sxs-lookup"><span data-stu-id="0f48f-124">To obtain more details on the requestor, include `$expand=requestor` in the query.</span></span>
<span data-ttu-id="0f48f-125">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="0f48f-125">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0f48f-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0f48f-126">Request headers</span></span>

| <span data-ttu-id="0f48f-127">Nome</span><span class="sxs-lookup"><span data-stu-id="0f48f-127">Name</span></span>      |<span data-ttu-id="0f48f-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f48f-128">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0f48f-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="0f48f-129">Authorization</span></span> | <span data-ttu-id="0f48f-p104">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0f48f-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0f48f-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0f48f-132">Request body</span></span>

<span data-ttu-id="0f48f-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0f48f-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0f48f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f48f-134">Response</span></span>

<span data-ttu-id="0f48f-135">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0f48f-135">If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0f48f-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0f48f-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0f48f-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0f48f-137">Request</span></span>

<span data-ttu-id="0f48f-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0f48f-138">The following is an example of the request.</span></span> <span data-ttu-id="0f48f-139">O URI de solicitação inclui apenas retornar solicitações em um estado específico e para retornar detalhes do solicitante e sua `$filter` `$expand` organização conectada também.</span><span class="sxs-lookup"><span data-stu-id="0f48f-139">The request URI includes `$filter` to only return requests in a particular state, and `$expand` to return details of the requestor and their connected organization as well.</span></span>

# <a name="http"></a>[<span data-ttu-id="0f48f-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="0f48f-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentrequests"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests?$expand=requestor($expand=connectedOrganization)&$filter=(requestState eq 'PendingApproval')
```
# <a name="c"></a>[<span data-ttu-id="0f48f-141">C#</span><span class="sxs-lookup"><span data-stu-id="0f48f-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentrequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0f48f-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0f48f-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentrequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0f48f-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0f48f-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentrequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0f48f-144">Java</span><span class="sxs-lookup"><span data-stu-id="0f48f-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageassignmentrequests-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0f48f-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f48f-145">Response</span></span>

<span data-ttu-id="0f48f-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0f48f-146">The following is an example of the response.</span></span>

> <span data-ttu-id="0f48f-147">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0f48f-147">**Note:** The response object shown here might be shortened for readability.</span></span>

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
      "requestType": "UserAdd",
      "requestState": "PendingApproval",
      "createdDateTime": "2019-10-25T22:55:11.623Z",
      "justification": "Need access",
      "answers": [],
      "requestor": {
        "connectedOrganizationId": "c3c2adbc-a863-437f-9383-ee578665317d",
        "id": "ba7ef0fb-e16f-474b-87aa-02815d061e67",
        "displayName": "displayname",
        "email": "displayname@example.com",
        "type": "User",
        "connectedOrganization": {
          "id": "c3c2adbc-a863-437f-9383-ee578665317d",
          "displayName": "example"
        }
      }
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

