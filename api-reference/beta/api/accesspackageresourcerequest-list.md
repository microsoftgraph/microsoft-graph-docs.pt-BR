---
title: Listar accessPackageResourceRequests
description: Recupere uma lista de objetos accessPackageResourceRequest.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6a165a0d678fd443c1ff237f7585de2bb115c02c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441953"
---
# <a name="list-accesspackageresourcerequests"></a><span data-ttu-id="02db9-103">Listar accessPackageResourceRequests</span><span class="sxs-lookup"><span data-stu-id="02db9-103">List accessPackageResourceRequests</span></span>

<span data-ttu-id="02db9-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="02db9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02db9-105">Recupere uma lista de objetos [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="02db9-105">Retrieve a list of [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="02db9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="02db9-106">Permissions</span></span>

<span data-ttu-id="02db9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02db9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="02db9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02db9-109">Permission type</span></span>                        | <span data-ttu-id="02db9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="02db9-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="02db9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02db9-111">Delegated (work or school account)</span></span>     |  <span data-ttu-id="02db9-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02db9-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="02db9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02db9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02db9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02db9-114">Not supported.</span></span> |
| <span data-ttu-id="02db9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="02db9-115">Application</span></span>                            | <span data-ttu-id="02db9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02db9-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="02db9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02db9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageResourceRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="02db9-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="02db9-118">Optional query parameters</span></span>

<span data-ttu-id="02db9-119">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="02db9-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="02db9-120">Por exemplo, para recuperar quem solicitou a adição de um recurso a um catálogo, `$expand=requestor` inclua na consulta.</span><span class="sxs-lookup"><span data-stu-id="02db9-120">For example, to retrieve who requested the addition of a resource to a catalog, include `$expand=requestor` in the query.</span></span> <span data-ttu-id="02db9-121">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="02db9-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="02db9-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="02db9-122">Request headers</span></span>

| <span data-ttu-id="02db9-123">Nome</span><span class="sxs-lookup"><span data-stu-id="02db9-123">Name</span></span>      |<span data-ttu-id="02db9-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="02db9-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="02db9-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="02db9-125">Authorization</span></span> | <span data-ttu-id="02db9-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02db9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="02db9-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02db9-128">Request body</span></span>

<span data-ttu-id="02db9-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="02db9-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="02db9-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="02db9-130">Response</span></span>

<span data-ttu-id="02db9-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02db9-131">If successful, this method returns a `200 OK` response code and a collection of [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="02db9-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="02db9-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="02db9-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02db9-133">Request</span></span>

<span data-ttu-id="02db9-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="02db9-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="02db9-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="02db9-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresourcerequests"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageResourceRequests
```
# <a name="c"></a>[<span data-ttu-id="02db9-136">C#</span><span class="sxs-lookup"><span data-stu-id="02db9-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageresourcerequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="02db9-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="02db9-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageresourcerequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="02db9-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="02db9-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageresourcerequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="02db9-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="02db9-139">Response</span></span>

<span data-ttu-id="02db9-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="02db9-140">The following is an example of the response.</span></span>

> <span data-ttu-id="02db9-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="02db9-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
