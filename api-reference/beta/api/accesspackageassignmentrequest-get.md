---
title: Obter accessPackageAssignmentRequest
description: Recupere as propriedades e as relações de um objeto accessPackageAssignmentRequest.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 0184e1146b6450cb5c500e8b377e817a42f82ff1
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439681"
---
# <a name="get-accesspackageassignmentrequest"></a><span data-ttu-id="89b1e-103">Obter accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="89b1e-103">Get accessPackageAssignmentRequest</span></span>

<span data-ttu-id="89b1e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89b1e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89b1e-105">No gerenciamento de direitos do [Azure AD,](../resources/entitlementmanagement-root.md)recupere as propriedades e as relações de um [objeto accessPackageAssignmentRequest.](../resources/accesspackageassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="89b1e-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve the properties and relationships of an  [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="89b1e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="89b1e-106">Permissions</span></span>

<span data-ttu-id="89b1e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89b1e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="89b1e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="89b1e-109">Permission type</span></span>                        | <span data-ttu-id="89b1e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="89b1e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="89b1e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="89b1e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="89b1e-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89b1e-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span>  |
| <span data-ttu-id="89b1e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="89b1e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89b1e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="89b1e-114">Not supported.</span></span> |
| <span data-ttu-id="89b1e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="89b1e-115">Application</span></span>                            | <span data-ttu-id="89b1e-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89b1e-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="89b1e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="89b1e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="89b1e-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="89b1e-118">Optional query parameters</span></span>

<span data-ttu-id="89b1e-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="89b1e-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="89b1e-120">Por exemplo, para recuperar o pacote de acesso solicitado, `$expand=accessPackage` inclua na consulta.</span><span class="sxs-lookup"><span data-stu-id="89b1e-120">For example, to retrieve the access package that was requested, include `$expand=accessPackage` in the query.</span></span> <span data-ttu-id="89b1e-121">Para recuperar a atribuição resultante, `$expand=accessPackageAssignment` inclua na consulta.</span><span class="sxs-lookup"><span data-stu-id="89b1e-121">To retrieve the resulting assignment, include `$expand=accessPackageAssignment` in the query.</span></span>  <span data-ttu-id="89b1e-122">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="89b1e-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="89b1e-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="89b1e-123">Request headers</span></span>

| <span data-ttu-id="89b1e-124">Nome</span><span class="sxs-lookup"><span data-stu-id="89b1e-124">Name</span></span>      |<span data-ttu-id="89b1e-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="89b1e-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="89b1e-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="89b1e-126">Authorization</span></span> | <span data-ttu-id="89b1e-127">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="89b1e-127">Bearer \{token\}.</span></span> <span data-ttu-id="89b1e-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="89b1e-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="89b1e-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="89b1e-129">Request body</span></span>

<span data-ttu-id="89b1e-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="89b1e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="89b1e-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="89b1e-131">Response</span></span>

<span data-ttu-id="89b1e-132">Se tiver êxito, este método retornará um código de resposta e `200 OK` o [objeto accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="89b1e-132">If successful, this method returns a `200 OK` response code and the requested [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="89b1e-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="89b1e-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="89b1e-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="89b1e-134">Request</span></span>

<span data-ttu-id="89b1e-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="89b1e-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="89b1e-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="89b1e-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{id}
```
# <a name="c"></a>[<span data-ttu-id="89b1e-137">C#</span><span class="sxs-lookup"><span data-stu-id="89b1e-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="89b1e-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="89b1e-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="89b1e-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="89b1e-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="89b1e-140">Java</span><span class="sxs-lookup"><span data-stu-id="89b1e-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageassignmentrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="89b1e-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="89b1e-141">Response</span></span>

<span data-ttu-id="89b1e-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="89b1e-142">The following is an example of the response.</span></span>

> <span data-ttu-id="89b1e-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="89b1e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


