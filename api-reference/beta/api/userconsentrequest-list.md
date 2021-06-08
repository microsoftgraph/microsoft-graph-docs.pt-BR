---
title: Listar userConsentRequests
description: Recupere objetos userConsentRequest e suas propriedades.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: a99c863e67040b156b84f17dc5c55414498a5b5b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759921"
---
# <a name="list-userconsentrequests"></a><span data-ttu-id="a0dec-103">Listar userConsentRequests</span><span class="sxs-lookup"><span data-stu-id="a0dec-103">List userConsentRequests</span></span>
<span data-ttu-id="a0dec-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0dec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0dec-105">Recupere uma coleção de [objetos userConsentRequest](../resources/userconsentrequest.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="a0dec-105">Retrieve a collection of [userConsentRequest](../resources/userconsentrequest.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="a0dec-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a0dec-106">Permissions</span></span>
<span data-ttu-id="a0dec-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0dec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0dec-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a0dec-109">Permission type</span></span>|<span data-ttu-id="a0dec-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a0dec-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0dec-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a0dec-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a0dec-112">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0dec-112">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span></span>|
|<span data-ttu-id="a0dec-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a0dec-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0dec-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0dec-114">Not supported.</span></span>|
|<span data-ttu-id="a0dec-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a0dec-115">Application</span></span>|<span data-ttu-id="a0dec-116">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0dec-116">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0dec-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a0dec-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/appConsent/appConsentRequests/{id}/userConsentRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a0dec-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a0dec-118">Optional query parameters</span></span>
<span data-ttu-id="a0dec-119">Este método dá suporte aos parâmetros de consulta , , , e OData para  `$select` ajudar a personalizar a `$skip` `$top` `$filter` `$orderby` resposta.</span><span class="sxs-lookup"><span data-stu-id="a0dec-119">This method supports the `$select`, `$skip`, `$top`, `$filter`, and `$orderby` OData query parameters to help customize the response.</span></span> <span data-ttu-id="a0dec-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a0dec-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a0dec-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a0dec-121">Request headers</span></span>
|<span data-ttu-id="a0dec-122">Nome</span><span class="sxs-lookup"><span data-stu-id="a0dec-122">Name</span></span>|<span data-ttu-id="a0dec-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0dec-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a0dec-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a0dec-124">Authorization</span></span>|<span data-ttu-id="a0dec-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a0dec-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0dec-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a0dec-127">Request body</span></span>
<span data-ttu-id="a0dec-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a0dec-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0dec-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0dec-129">Response</span></span>

<span data-ttu-id="a0dec-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos userConsentRequest](../resources/userconsentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a0dec-130">If successful, this method returns a `200 OK` response code and a collection of [userConsentRequest](../resources/userconsentrequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a0dec-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a0dec-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a0dec-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a0dec-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a0dec-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a0dec-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_userconsentrequest"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/appConsent/appConsentRequests/ee245379-e3bb-4944-a997-24115f0b8b5e/userConsentRequests
```
# <a name="c"></a>[<span data-ttu-id="a0dec-134">C#</span><span class="sxs-lookup"><span data-stu-id="a0dec-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-userconsentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a0dec-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a0dec-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-userconsentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a0dec-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a0dec-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-userconsentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a0dec-137">Java</span><span class="sxs-lookup"><span data-stu-id="a0dec-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-userconsentrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="a0dec-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0dec-138">Response</span></span>
><span data-ttu-id="a0dec-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a0dec-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.userConsentRequest)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/appConsent/appConsentRequests('ee245379-e3bb-4944-a997-24115f0b8b5e')/userConsentRequests",
  "@odata.count": 1,
  "value": [
    {
      "id": "acef2660-d194-4943-b927-4fe4fb5cb7e3",
      "reason": "I need access",
      "status": "Completed",
      "createdDateTime": "2019-10-18T19:07:19.7374554Z",
      "createdBy": {
        "user": {
          "id": "db60ab61-caea-4889-a824-98de31ef31b5",
          "displayName": "Alex Wilber",
          "userPrincipalName": "AlexW@contoso.com",
          "mail": "AlexW@contoso.com"
        }
      },
      "approval@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/appConsent/appConsentRequests('ee245379-e3bb-4944-a997-24115f0b8b5e')/userConsentRequests('acef2660-d194-4943-b927-4fe4fb5cb7e3')/approval/$entity",
      "approval": {
        "id": "acef2660-d194-4943-b927-4fe4fb5cb7e3",
        "steps@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/appConsent/appConsentRequests('ee245379-e3bb-4944-a997-24115f0b8b5e')/userConsentRequests('acef2660-d194-4943-b927-4fe4fb5cb7e3')/approval/steps",
        "steps": [
          {
            "id": "f5a4ca4a-1316-4872-8112-993c55dab51e",
            "displayName": null,
            "reviewedDateTime": "2019-10-19T04:12:09.633Z",
            "reviewResult": "Approve",
            "status": "Completed",
            "assignedToMe": true,
            "justification": "Admin consent granted.",
            "reviewedBy": {
              "id": "00000001-0000-0000-c000-000000000000",
              "displayName": "",
              "userPrincipalName": "",
              "mail": ""
            }
          }
        ]
      },
      "approvalId": "acef2660-d194-4943-b927-4fe4fb5cb7e3",
      "completedDateTime": null,
      "customData": null
    }
  ]
}
```
