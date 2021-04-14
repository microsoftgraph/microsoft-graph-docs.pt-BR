---
title: 'appConsentRequest: filterByCurrentUser'
description: Recupere objetos appConsentRequest para os quais o usuário atual é o revistor.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: c17e44b27b135eec034eb66399d5ce5163a5928f
ms.sourcegitcommit: ad1e4d758d4fe6025987c1c3528ce644edb27062
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/13/2021
ms.locfileid: "51697947"
---
# <a name="appconsentrequest-filterbycurrentuser"></a><span data-ttu-id="c2fa6-103">appConsentRequest: filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="c2fa6-103">appConsentRequest: filterByCurrentUser</span></span>

<span data-ttu-id="c2fa6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2fa6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c2fa6-105">Recupere uma coleção de [objetos appConsentRequest](../resources/appconsentrequest.md) para os quais o usuário atual é o revistor e o status do userConsentRequest para acessar o aplicativo especificado é `InProgress` .</span><span class="sxs-lookup"><span data-stu-id="c2fa6-105">Retrieve a collection of [appConsentRequest](../resources/appconsentrequest.md) objects for which the current user is the reviewer and the status of the userConsentRequest for accessing the specified app is `InProgress`.</span></span>

## <a name="permissions"></a><span data-ttu-id="c2fa6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c2fa6-106">Permissions</span></span>

<span data-ttu-id="c2fa6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2fa6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2fa6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c2fa6-109">Permission type</span></span>|<span data-ttu-id="c2fa6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c2fa6-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c2fa6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c2fa6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c2fa6-112">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2fa6-112">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span></span>|
|<span data-ttu-id="c2fa6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c2fa6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c2fa6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c2fa6-114">Not supported.</span></span>|
|<span data-ttu-id="c2fa6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c2fa6-115">Application</span></span>|<span data-ttu-id="c2fa6-116">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2fa6-116">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c2fa6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c2fa6-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/appConsent/appConsentRequests/filterByCurrentUser(on='parameterValue')
```

## <a name="function-parameters"></a><span data-ttu-id="c2fa6-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="c2fa6-118">Function parameters</span></span>

<span data-ttu-id="c2fa6-119">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="c2fa6-119">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="c2fa6-120">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="c2fa6-120">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="c2fa6-121">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c2fa6-121">Parameter</span></span>|<span data-ttu-id="c2fa6-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="c2fa6-122">Type</span></span>|<span data-ttu-id="c2fa6-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2fa6-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2fa6-124">on</span><span class="sxs-lookup"><span data-stu-id="c2fa6-124">on</span></span>|<span data-ttu-id="c2fa6-125">consentRequestFilterByCurrentUserOptions</span><span class="sxs-lookup"><span data-stu-id="c2fa6-125">consentRequestFilterByCurrentUserOptions</span></span>|<span data-ttu-id="c2fa6-126">Filtre para consultar objetos appConsentRequest para os quais o usuário atual é um revistor.</span><span class="sxs-lookup"><span data-stu-id="c2fa6-126">Filter to query appConsentRequest objects for which the current user is a reviewer.</span></span> <span data-ttu-id="c2fa6-127">O valor permitido é `reviewer` .</span><span class="sxs-lookup"><span data-stu-id="c2fa6-127">Allowed value is `reviewer`.</span></span> <span data-ttu-id="c2fa6-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c2fa6-128">Required.</span></span>|

## <a name="query-parameters"></a><span data-ttu-id="c2fa6-129">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="c2fa6-129">Query parameters</span></span>

<span data-ttu-id="c2fa6-130">Essa função exige que o parâmetro de consulta OData retorne uma coleção de objetos  `$filter` [userConsentRequest](../resources/userconsentrequest.md) para os quais o status é `InProgress` .</span><span class="sxs-lookup"><span data-stu-id="c2fa6-130">This function requires the `$filter` OData query parameter to return a collection of [userConsentRequest](../resources/userconsentrequest.md) objects for which the status is `InProgress`.</span></span> <span data-ttu-id="c2fa6-131">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="c2fa6-131">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c2fa6-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c2fa6-132">Request headers</span></span>

|<span data-ttu-id="c2fa6-133">Nome</span><span class="sxs-lookup"><span data-stu-id="c2fa6-133">Name</span></span>|<span data-ttu-id="c2fa6-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2fa6-134">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c2fa6-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="c2fa6-135">Authorization</span></span>|<span data-ttu-id="c2fa6-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c2fa6-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2fa6-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c2fa6-138">Request body</span></span>

<span data-ttu-id="c2fa6-139">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c2fa6-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2fa6-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2fa6-140">Response</span></span>

<span data-ttu-id="c2fa6-141">Se tiver êxito, essa função retornará um código de resposta e uma `200 OK` coleção de [objetos appConsentRequest](../resources/appconsentrequest.md)  no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c2fa6-141">If successful, this function returns a `200 OK` response code and a collection of [appConsentRequest](../resources/appconsentrequest.md)  objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2fa6-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c2fa6-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="c2fa6-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c2fa6-143">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c2fa6-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="c2fa6-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "appconsentrequest_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/appConsent/appConsentRequests/filterByCurrentUser(on='reviewer')?$filter=userConsentRequests/any(u:u/status eq 'InProgress')
```
# <a name="c"></a>[<span data-ttu-id="c2fa6-145">C#</span><span class="sxs-lookup"><span data-stu-id="c2fa6-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/appconsentrequest-filterbycurrentuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c2fa6-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c2fa6-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/appconsentrequest-filterbycurrentuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c2fa6-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c2fa6-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/appconsentrequest-filterbycurrentuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c2fa6-148">Java</span><span class="sxs-lookup"><span data-stu-id="c2fa6-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/appconsentrequest-filterbycurrentuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c2fa6-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2fa6-149">Response</span></span>

<span data-ttu-id="c2fa6-150">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c2fa6-150">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.appConsentRequest)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(appConsentRequest)",
  "@odata.count": 1,
  "value": [
    {
      "id": "af330b30-dd59-4482-a848-0fd81b0438ed",
      "appId": "3ca5f23f-94b4-4930-aec9-b8ca0f060e68",
      "appDisplayName": "Moodle",
      "pendingScopes": [],
      "userConsentRequests@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/appConsent/appConsentRequests('af330b30-dd59-4482-a848-0fd81b0438ed')/userConsentRequests",
      "userConsentRequests": []
    }
  ]
}
```

