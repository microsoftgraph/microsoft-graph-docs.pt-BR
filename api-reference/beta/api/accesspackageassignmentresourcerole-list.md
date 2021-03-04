---
title: Listar accessPackageAssignmentResourceRoles
description: Recupere uma lista de objetos accessPackageAssignmentResourceRole.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: e1d6c10437f4fa0c2eee26026dca3d323bf3bdd0
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439608"
---
# <a name="list-accesspackageassignmentresourceroles"></a><span data-ttu-id="ab3e2-103">Listar accessPackageAssignmentResourceRoles</span><span class="sxs-lookup"><span data-stu-id="ab3e2-103">List accessPackageAssignmentResourceRoles</span></span>

<span data-ttu-id="ab3e2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab3e2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab3e2-105">Recupere uma lista de [objetos accessPackageAssignmentResourceRole.](../resources/accesspackageassignmentresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="ab3e2-105">Retrieve a list of [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) objects.</span></span>  <span data-ttu-id="ab3e2-106">A lista resultante inclui todas as funções de recurso de todas as atribuições que o chamador tem acesso para ler, em todos os catálogos e pacotes de acesso.</span><span class="sxs-lookup"><span data-stu-id="ab3e2-106">The resulting list includes all the resource roles of all assignments that the caller has access to read, across all catalogs and access packages.</span></span>

## <a name="permissions"></a><span data-ttu-id="ab3e2-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="ab3e2-107">Permissions</span></span>

<span data-ttu-id="ab3e2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab3e2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ab3e2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ab3e2-110">Permission type</span></span>                        | <span data-ttu-id="ab3e2-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ab3e2-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ab3e2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ab3e2-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="ab3e2-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab3e2-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="ab3e2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ab3e2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab3e2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ab3e2-115">Not supported.</span></span> |
| <span data-ttu-id="ab3e2-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ab3e2-116">Application</span></span>                            | <span data-ttu-id="ab3e2-117">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab3e2-117">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab3e2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ab3e2-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentResourceRoles
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ab3e2-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ab3e2-119">Optional query parameters</span></span>

<span data-ttu-id="ab3e2-120">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ab3e2-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="ab3e2-121">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ab3e2-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

<span data-ttu-id="ab3e2-122">Por exemplo, para recuperar apenas funções de recurso de atribuição de pacote de acesso para um usuário específico, você pode incluir uma consulta com um filtro direcionando a ID do objeto desse usuário `?$expand=accessPackageSubject&$filter=accessPackageSubject/objectId+eq+'9b835e5c-bf18-4ad9-8556-9b1ea0019c6b'` .</span><span class="sxs-lookup"><span data-stu-id="ab3e2-122">For example, to retrieve only access package assignment resource roles for a particular user, you can include a query with a filter targeting the object ID of that user `?$expand=accessPackageSubject&$filter=accessPackageSubject/objectId+eq+'9b835e5c-bf18-4ad9-8556-9b1ea0019c6b'`.</span></span>


## <a name="request-headers"></a><span data-ttu-id="ab3e2-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ab3e2-123">Request headers</span></span>

| <span data-ttu-id="ab3e2-124">Nome</span><span class="sxs-lookup"><span data-stu-id="ab3e2-124">Name</span></span>      |<span data-ttu-id="ab3e2-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab3e2-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ab3e2-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="ab3e2-126">Authorization</span></span> | <span data-ttu-id="ab3e2-127">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="ab3e2-127">Bearer \{token\}.</span></span> <span data-ttu-id="ab3e2-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ab3e2-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ab3e2-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ab3e2-129">Request body</span></span>

<span data-ttu-id="ab3e2-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ab3e2-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab3e2-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab3e2-131">Response</span></span>

<span data-ttu-id="ab3e2-132">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ab3e2-132">If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ab3e2-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ab3e2-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ab3e2-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ab3e2-134">Request</span></span>

<span data-ttu-id="ab3e2-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ab3e2-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ab3e2-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="ab3e2-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentresourceroles"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentResourceRoles
```
# <a name="c"></a>[<span data-ttu-id="ab3e2-137">C#</span><span class="sxs-lookup"><span data-stu-id="ab3e2-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentresourceroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ab3e2-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ab3e2-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentresourceroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ab3e2-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ab3e2-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentresourceroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ab3e2-140">Java</span><span class="sxs-lookup"><span data-stu-id="ab3e2-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageassignmentresourceroles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ab3e2-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab3e2-141">Response</span></span>

<span data-ttu-id="ab3e2-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ab3e2-142">The following is an example of the response.</span></span>

> <span data-ttu-id="ab3e2-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ab3e2-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentResourceRole",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "1bf101d2-4d9c-437f-bbf5-3d13d98f5479",
      "originId": "originId-value",
      "originSystem": "SharePointOnline",
      "status": "Fulfilled"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageAssignmentResourceRoles",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


