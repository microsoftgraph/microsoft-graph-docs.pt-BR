---
title: Listar accessPackageAssignmentRequests
description: Recupere uma lista de objetos accessPackageAssignmentRequest.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5f0c338c5cea44f6ef979495e929d757779f4ad7
ms.sourcegitcommit: c1935e442ee973c6c3fcb01a15d76bcfa625362e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/22/2020
ms.locfileid: "44345650"
---
# <a name="list-accesspackageassignmentrequests"></a><span data-ttu-id="f913a-103">Listar accessPackageAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="f913a-103">List accessPackageAssignmentRequests</span></span>

<span data-ttu-id="f913a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f913a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f913a-105">No [Gerenciamento de direitos do Azure ad](../resources/entitlementmanagement-root.md), recupere uma lista de objetos [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="f913a-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve a list of [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) objects.</span></span>  <span data-ttu-id="f913a-106">A lista resultante inclui todas as solicitações de atribuição, atuais e bem como expiradas, que o chamador tem acesso para leitura, entre todos os catálogos e pacotes de acesso.</span><span class="sxs-lookup"><span data-stu-id="f913a-106">The resulting list includes all the assignment requests, current and well as expired, that the caller has access to read, across all catalogs and access packages.</span></span>

## <a name="permissions"></a><span data-ttu-id="f913a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f913a-107">Permissions</span></span>

<span data-ttu-id="f913a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f913a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f913a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f913a-110">Permission type</span></span>                        | <span data-ttu-id="f913a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f913a-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f913a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f913a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="f913a-113">EntitlementManagement. Read. All, EntitlementManagement. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f913a-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="f913a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f913a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f913a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f913a-115">Not supported.</span></span> |
| <span data-ttu-id="f913a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f913a-116">Application</span></span>                            | <span data-ttu-id="f913a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f913a-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f913a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f913a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f913a-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f913a-119">Optional query parameters</span></span>

<span data-ttu-id="f913a-120">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f913a-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="f913a-121">Por exemplo, para recuperar o pacote de acesso de cada solicitação, inclua `$expand=accessPackage` na consulta.</span><span class="sxs-lookup"><span data-stu-id="f913a-121">For example, to retrieve the access package of each request, include `$expand=accessPackage` in the query.</span></span>  <span data-ttu-id="f913a-122">Para recuperar apenas as solicitações para um pacote de acesso específico, inclua na consulta um filtro, como `$expand=accessPackage&$filter=accessPackage/id eq '9bbe5f7d-f1e7-4eb1-a586-38cdf6f8b1ea'` .</span><span class="sxs-lookup"><span data-stu-id="f913a-122">To retrieve only requests for a specific access package, include in the query a filter such as `$expand=accessPackage&$filter=accessPackage/id eq '9bbe5f7d-f1e7-4eb1-a586-38cdf6f8b1ea'`.</span></span>
<span data-ttu-id="f913a-123">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f913a-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f913a-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f913a-124">Request headers</span></span>

| <span data-ttu-id="f913a-125">Nome</span><span class="sxs-lookup"><span data-stu-id="f913a-125">Name</span></span>      |<span data-ttu-id="f913a-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="f913a-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f913a-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="f913a-127">Authorization</span></span> | <span data-ttu-id="f913a-128">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="f913a-128">Bearer \{token\}.</span></span> <span data-ttu-id="f913a-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f913a-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f913a-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f913a-130">Request body</span></span>

<span data-ttu-id="f913a-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f913a-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f913a-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="f913a-132">Response</span></span>

<span data-ttu-id="f913a-133">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f913a-133">If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f913a-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f913a-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f913a-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f913a-135">Request</span></span>

<span data-ttu-id="f913a-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f913a-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f913a-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="f913a-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentrequests"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests
```
# <a name="c"></a>[<span data-ttu-id="f913a-138">C#</span><span class="sxs-lookup"><span data-stu-id="f913a-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentrequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f913a-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f913a-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentrequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f913a-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f913a-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentrequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f913a-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="f913a-141">Response</span></span>

<span data-ttu-id="f913a-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f913a-142">The following is an example of the response.</span></span>

> <span data-ttu-id="f913a-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f913a-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
