---
title: Obter accessPackageAssignmentRequest
description: Recupere as propriedades e as relações de um objeto accessPackageAssignmentRequest.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 78340e93b202d4088b453e39594b84345a247cbe
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048600"
---
# <a name="get-accesspackageassignmentrequest"></a><span data-ttu-id="d852b-103">Obter accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="d852b-103">Get accessPackageAssignmentRequest</span></span>

<span data-ttu-id="d852b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d852b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d852b-105">No gerenciamento de direitos do [Azure AD,](../resources/entitlementmanagement-root.md)recupere as propriedades e as relações de um [objeto accessPackageAssignmentRequest.](../resources/accesspackageassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="d852b-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve the properties and relationships of an  [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d852b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d852b-106">Permissions</span></span>

<span data-ttu-id="d852b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d852b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d852b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d852b-109">Permission type</span></span>                        | <span data-ttu-id="d852b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d852b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d852b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d852b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d852b-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d852b-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span>  |
| <span data-ttu-id="d852b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d852b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d852b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d852b-114">Not supported.</span></span> |
| <span data-ttu-id="d852b-115">Application</span><span class="sxs-lookup"><span data-stu-id="d852b-115">Application</span></span>                            | <span data-ttu-id="d852b-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d852b-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d852b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d852b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d852b-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d852b-118">Optional query parameters</span></span>

<span data-ttu-id="d852b-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d852b-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="d852b-120">Por exemplo, para recuperar o pacote de acesso solicitado, `$expand=accessPackage` inclua na consulta.</span><span class="sxs-lookup"><span data-stu-id="d852b-120">For example, to retrieve the access package that was requested, include `$expand=accessPackage` in the query.</span></span> <span data-ttu-id="d852b-121">Para recuperar a atribuição resultante, `$expand=accessPackageAssignment` inclua na consulta.</span><span class="sxs-lookup"><span data-stu-id="d852b-121">To retrieve the resulting assignment, include `$expand=accessPackageAssignment` in the query.</span></span>  <span data-ttu-id="d852b-122">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="d852b-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d852b-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d852b-123">Request headers</span></span>

| <span data-ttu-id="d852b-124">Nome</span><span class="sxs-lookup"><span data-stu-id="d852b-124">Name</span></span>      |<span data-ttu-id="d852b-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="d852b-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d852b-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="d852b-126">Authorization</span></span> | <span data-ttu-id="d852b-p103">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d852b-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d852b-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d852b-129">Request body</span></span>

<span data-ttu-id="d852b-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d852b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d852b-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d852b-131">Response</span></span>

<span data-ttu-id="d852b-132">Se tiver êxito, este método retornará um código de resposta e `200 OK` o [objeto accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d852b-132">If successful, this method returns a `200 OK` response code and the requested [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d852b-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d852b-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d852b-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d852b-134">Request</span></span>

<span data-ttu-id="d852b-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d852b-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d852b-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="d852b-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{id}
```
# <a name="c"></a>[<span data-ttu-id="d852b-137">C#</span><span class="sxs-lookup"><span data-stu-id="d852b-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d852b-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d852b-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d852b-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d852b-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d852b-140">Java</span><span class="sxs-lookup"><span data-stu-id="d852b-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageassignmentrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d852b-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="d852b-141">Response</span></span>

<span data-ttu-id="d852b-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d852b-142">The following is an example of the response.</span></span>

> <span data-ttu-id="d852b-143">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d852b-143">**Note:** The response object shown here might be shortened for readability.</span></span>

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


