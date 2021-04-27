---
title: Listar accessPackageResourceRequests
description: Recupere uma lista de objetos accessPackageResourceRequest.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 4d1a59f73ec259d186f9313660947eeed309c3e0
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048537"
---
# <a name="list-accesspackageresourcerequests"></a><span data-ttu-id="0602d-103">Listar accessPackageResourceRequests</span><span class="sxs-lookup"><span data-stu-id="0602d-103">List accessPackageResourceRequests</span></span>

<span data-ttu-id="0602d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0602d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0602d-105">Recupere uma lista de [objetos accessPackageResourceRequest.](../resources/accesspackageresourcerequest.md)</span><span class="sxs-lookup"><span data-stu-id="0602d-105">Retrieve a list of [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="0602d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0602d-106">Permissions</span></span>

<span data-ttu-id="0602d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0602d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0602d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0602d-109">Permission type</span></span>                        | <span data-ttu-id="0602d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0602d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0602d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0602d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0602d-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0602d-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="0602d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0602d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0602d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0602d-114">Not supported.</span></span> |
| <span data-ttu-id="0602d-115">Application</span><span class="sxs-lookup"><span data-stu-id="0602d-115">Application</span></span>                            | <span data-ttu-id="0602d-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0602d-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0602d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0602d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageResourceRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0602d-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0602d-118">Optional query parameters</span></span>

<span data-ttu-id="0602d-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0602d-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="0602d-120">Por exemplo, para recuperar quem solicitou a adição de um recurso a um catálogo, `$expand=requestor` inclua na consulta.</span><span class="sxs-lookup"><span data-stu-id="0602d-120">For example, to retrieve who requested the addition of a resource to a catalog, include `$expand=requestor` in the query.</span></span> <span data-ttu-id="0602d-121">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="0602d-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0602d-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0602d-122">Request headers</span></span>

| <span data-ttu-id="0602d-123">Nome</span><span class="sxs-lookup"><span data-stu-id="0602d-123">Name</span></span>      |<span data-ttu-id="0602d-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="0602d-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0602d-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="0602d-125">Authorization</span></span> | <span data-ttu-id="0602d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0602d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0602d-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0602d-128">Request body</span></span>

<span data-ttu-id="0602d-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0602d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0602d-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="0602d-130">Response</span></span>

<span data-ttu-id="0602d-131">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0602d-131">If successful, this method returns a `200 OK` response code and a collection of [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0602d-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0602d-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0602d-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0602d-133">Request</span></span>

<span data-ttu-id="0602d-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0602d-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0602d-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="0602d-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresourcerequests"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageResourceRequests
```
# <a name="c"></a>[<span data-ttu-id="0602d-136">C#</span><span class="sxs-lookup"><span data-stu-id="0602d-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageresourcerequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0602d-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0602d-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageresourcerequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0602d-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0602d-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageresourcerequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0602d-139">Java</span><span class="sxs-lookup"><span data-stu-id="0602d-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageresourcerequests-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0602d-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="0602d-140">Response</span></span>

<span data-ttu-id="0602d-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0602d-141">The following is an example of the response.</span></span>

> <span data-ttu-id="0602d-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0602d-142">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageResourceRequest",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "catalogId": "26ac0c0a-08bc-4a7b-a313-839f58044ba5",
      "id": "1fe272f0-d463-42aa-a9a8-b07ab50a1c4d",
      "isValidationOnly": false,
      "justification": "String",
      "requestState": "Delivered",
      "requestStatus": "Fulfilled",
      "requestType": "AdminAdd"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageResourceRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


