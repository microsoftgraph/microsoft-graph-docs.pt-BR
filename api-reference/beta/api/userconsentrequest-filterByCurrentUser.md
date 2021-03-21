---
title: 'userConsentRequests: filterByCurrentUser'
description: Recupere userConsentRequests para o qual o usuário atual é o revistor.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: a4fe32aab22b425fcdf58389bc6b71cae2147b42
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50965009"
---
# <a name="userconsentrequests-filterbycurrentuser"></a><span data-ttu-id="3f543-103">userConsentRequests: filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="3f543-103">userConsentRequests: filterByCurrentUser</span></span>
<span data-ttu-id="3f543-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f543-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f543-105">Recupere [o userConsentRequests](../resources/userconsentrequest.md) para um appConsentRequest para o qual o usuário atual é o revistor e o status do userConsentRequest é `InProgress` .</span><span class="sxs-lookup"><span data-stu-id="3f543-105">Retrieve the [userConsentRequests](../resources/userconsentrequest.md) for an appConsentRequest for which the current user is the reviewer and the status of the userConsentRequest is `InProgress`.</span></span>

## <a name="permissions"></a><span data-ttu-id="3f543-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3f543-106">Permissions</span></span>
<span data-ttu-id="3f543-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f543-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f543-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3f543-109">Permission type</span></span>|<span data-ttu-id="3f543-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3f543-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3f543-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3f543-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3f543-112">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f543-112">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span></span>|
|<span data-ttu-id="3f543-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3f543-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3f543-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3f543-114">Not supported.</span></span>|
|<span data-ttu-id="3f543-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3f543-115">Application</span></span>|<span data-ttu-id="3f543-116">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f543-116">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3f543-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3f543-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/appConsent/appConsentRequests/{id}/userConsentRequests/filterByCurrentUser(on='parameterValue')
```

## <a name="function-parameters"></a><span data-ttu-id="3f543-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="3f543-118">Function parameters</span></span>
<span data-ttu-id="3f543-119">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="3f543-119">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="3f543-120">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="3f543-120">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="3f543-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3f543-121">Property</span></span>|<span data-ttu-id="3f543-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="3f543-122">Type</span></span>|<span data-ttu-id="3f543-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f543-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f543-124">on</span><span class="sxs-lookup"><span data-stu-id="3f543-124">on</span></span>|<span data-ttu-id="3f543-125">consentRequestFilterByCurrentUserOptions</span><span class="sxs-lookup"><span data-stu-id="3f543-125">consentRequestFilterByCurrentUserOptions</span></span>|<span data-ttu-id="3f543-126">Filtrar para consultar userConsentRequests para um appConsentRequest para o qual o usuário atual é um revistor.</span><span class="sxs-lookup"><span data-stu-id="3f543-126">Filter to query userConsentRequests for an appConsentRequest for which the current user is a reviewer.</span></span> <span data-ttu-id="3f543-127">O valor permitido é `reviewer` .</span><span class="sxs-lookup"><span data-stu-id="3f543-127">Allowed value is `reviewer`.</span></span> <span data-ttu-id="3f543-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3f543-128">Required.</span></span>|

## <a name="optional-query-parameters"></a><span data-ttu-id="3f543-129">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3f543-129">Optional query parameters</span></span>
<span data-ttu-id="3f543-130">Essa função dá suporte ao  `$filter` parâmetro de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3f543-130">This function supports the `$filter` OData query parameter to help customize the response.</span></span> <span data-ttu-id="3f543-131">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="3f543-131">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="3f543-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3f543-132">Request headers</span></span>
|<span data-ttu-id="3f543-133">Nome</span><span class="sxs-lookup"><span data-stu-id="3f543-133">Name</span></span>|<span data-ttu-id="3f543-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f543-134">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3f543-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="3f543-135">Authorization</span></span>|<span data-ttu-id="3f543-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3f543-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f543-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3f543-138">Request body</span></span>
<span data-ttu-id="3f543-139">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3f543-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3f543-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="3f543-140">Response</span></span>

<span data-ttu-id="3f543-141">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos userConsentRequest](../resources/userconsentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3f543-141">If successful, this method returns a `200 OK` response code and a collection of [userConsentRequest](../resources/userconsentrequest.md) objects in the response body.</span></span>

## <a name="example-list-all-userconsentrequests-for-which-the-current-user-is-the-reviewer-and-the-status-is-completed"></a><span data-ttu-id="3f543-142">Exemplo: listar todos os userConsentRequests para os quais o usuário atual é o revistor e o status é Concluído</span><span class="sxs-lookup"><span data-stu-id="3f543-142">Example: List all userConsentRequests for which the current user is the reviewer and the status is Completed</span></span>

### <a name="request"></a><span data-ttu-id="3f543-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3f543-143">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "userconsentrequest_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/appConsent/appConsentRequests/ee245379-e3bb-4944-a997-24115f0b8b5e/userConsentRequests/filterByCurrentUser(on='reviewer')?$filter= (status eq 'Completed')
```


### <a name="response"></a><span data-ttu-id="3f543-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="3f543-144">Response</span></span>
<span data-ttu-id="3f543-145">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3f543-145">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(userConsentRequest)",
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
