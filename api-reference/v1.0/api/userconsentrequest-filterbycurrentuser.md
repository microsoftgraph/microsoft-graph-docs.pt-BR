---
title: 'userConsentRequest: filterByCurrentUser'
description: Recupere objetos userConsentRequest para os quais o usuário atual é o revistor.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: e30d94934f0ccce140610a8ee713e16aff83c3d6
ms.sourcegitcommit: ad1e4d758d4fe6025987c1c3528ce644edb27062
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/13/2021
ms.locfileid: "51698076"
---
# <a name="userconsentrequest-filterbycurrentuser"></a><span data-ttu-id="92d30-103">userConsentRequest: filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="92d30-103">userConsentRequest: filterByCurrentUser</span></span>

<span data-ttu-id="92d30-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92d30-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="92d30-105">Recupere uma coleção [de objetos userConsentRequest](../resources/userconsentrequest.md) para acessar um aplicativo especificado, para o qual o usuário atual é o revistor.</span><span class="sxs-lookup"><span data-stu-id="92d30-105">Retrieve a collection of [userConsentRequest](../resources/userconsentrequest.md) objects for accessing a specified app, for which the current user is the reviewer.</span></span>

## <a name="permissions"></a><span data-ttu-id="92d30-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="92d30-106">Permissions</span></span>

<span data-ttu-id="92d30-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92d30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92d30-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="92d30-109">Permission type</span></span>|<span data-ttu-id="92d30-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="92d30-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92d30-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="92d30-111">Delegated (work or school account)</span></span>|<span data-ttu-id="92d30-112">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92d30-112">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span></span>|
|<span data-ttu-id="92d30-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="92d30-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92d30-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92d30-114">Not supported.</span></span>|
|<span data-ttu-id="92d30-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="92d30-115">Application</span></span>|<span data-ttu-id="92d30-116">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92d30-116">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="92d30-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="92d30-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/appConsent/appConsentRequests/{id}/userConsentRequests/filterByCurrentUser(on='parameterValue')
```

## <a name="function-parameters"></a><span data-ttu-id="92d30-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="92d30-118">Function parameters</span></span>

<span data-ttu-id="92d30-119">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="92d30-119">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="92d30-120">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="92d30-120">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="92d30-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="92d30-121">Property</span></span>|<span data-ttu-id="92d30-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="92d30-122">Type</span></span>|<span data-ttu-id="92d30-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="92d30-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92d30-124">on</span><span class="sxs-lookup"><span data-stu-id="92d30-124">on</span></span>|<span data-ttu-id="92d30-125">consentRequestFilterByCurrentUserOptions</span><span class="sxs-lookup"><span data-stu-id="92d30-125">consentRequestFilterByCurrentUserOptions</span></span>|<span data-ttu-id="92d30-126">Filtrar para consultar objetos userConsentRequest para um objeto appConsentRequest para o qual o usuário atual é um revistor.</span><span class="sxs-lookup"><span data-stu-id="92d30-126">Filter to query userConsentRequest objects for an appConsentRequest object for which the current user is a reviewer.</span></span> <span data-ttu-id="92d30-127">O valor permitido é `reviewer` .</span><span class="sxs-lookup"><span data-stu-id="92d30-127">Allowed value is `reviewer`.</span></span> <span data-ttu-id="92d30-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92d30-128">Required.</span></span>|

## <a name="optional-query-parameters"></a><span data-ttu-id="92d30-129">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="92d30-129">Optional query parameters</span></span>

<span data-ttu-id="92d30-130">Essa função dá suporte ao  `$filter` parâmetro de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="92d30-130">This function supports the `$filter` OData query parameter to help customize the response.</span></span> <span data-ttu-id="92d30-131">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="92d30-131">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="92d30-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="92d30-132">Request headers</span></span>

|<span data-ttu-id="92d30-133">Nome</span><span class="sxs-lookup"><span data-stu-id="92d30-133">Name</span></span>|<span data-ttu-id="92d30-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="92d30-134">Description</span></span>|
|:---|:---|
|<span data-ttu-id="92d30-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="92d30-135">Authorization</span></span>|<span data-ttu-id="92d30-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92d30-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="92d30-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="92d30-138">Request body</span></span>

<span data-ttu-id="92d30-139">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="92d30-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="92d30-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="92d30-140">Response</span></span>

<span data-ttu-id="92d30-141">Se tiver êxito, essa função retornará um código de resposta e uma `200 OK` coleção de [objetos userConsentRequest](../resources/userconsentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="92d30-141">If successful, this function returns a `200 OK` response code and a collection of [userConsentRequest](../resources/userconsentrequest.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92d30-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="92d30-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="92d30-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="92d30-143">Request</span></span>

<span data-ttu-id="92d30-144">Nesta solicitação, você lista todos os **objetos userConsentRequest** para os quais o usuário atual é o revistor e o status é `Completed` .</span><span class="sxs-lookup"><span data-stu-id="92d30-144">In this request, you list all **userConsentRequest** objects for which the current user is the reviewer and the status is `Completed`.</span></span>

# <a name="http"></a>[<span data-ttu-id="92d30-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="92d30-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "userconsentrequest_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/appConsent/appConsentRequests/ee245379-e3bb-4944-a997-24115f0b8b5e/userConsentRequests/filterByCurrentUser(on='reviewer')?$filter= (status eq 'Completed')
```
# <a name="c"></a>[<span data-ttu-id="92d30-146">C#</span><span class="sxs-lookup"><span data-stu-id="92d30-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/userconsentrequest-filterbycurrentuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="92d30-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92d30-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/userconsentrequest-filterbycurrentuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="92d30-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="92d30-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/userconsentrequest-filterbycurrentuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="92d30-149">Java</span><span class="sxs-lookup"><span data-stu-id="92d30-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/userconsentrequest-filterbycurrentuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="92d30-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="92d30-150">Response</span></span>

<span data-ttu-id="92d30-151">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="92d30-151">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/appConsent/appConsentRequests('ee245379-e3bb-4944-a997-24115f0b8b5e')/userConsentRequests",
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
      "approval@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/appConsent/appConsentRequests('ee245379-e3bb-4944-a997-24115f0b8b5e')/userConsentRequests('acef2660-d194-4943-b927-4fe4fb5cb7e3')/approval/$entity",
      "approval": {
        "id": "acef2660-d194-4943-b927-4fe4fb5cb7e3",
        "stages@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/appConsent/appConsentRequests('ee245379-e3bb-4944-a997-24115f0b8b5e')/userConsentRequests('acef2660-d194-4943-b927-4fe4fb5cb7e3')/approval/stages",
        "stages": [
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

