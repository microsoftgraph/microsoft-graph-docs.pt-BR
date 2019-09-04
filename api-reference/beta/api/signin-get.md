---
title: Obter entrada
doc_type: apiPageType
description: Recupere um evento específico de entrada do Azure AD para seu locatário.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ae597257544645ddf705be0156a10febcf272e29
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36722360"
---
# <a name="get-signin"></a><span data-ttu-id="853f3-103">Obter entrada</span><span class="sxs-lookup"><span data-stu-id="853f3-103">Get signIn</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="853f3-104">Recupere um evento específico de entrada do Azure AD para seu locatário.</span><span class="sxs-lookup"><span data-stu-id="853f3-104">Retrieve a specific Azure AD user sign-in event for your tenant.</span></span> <span data-ttu-id="853f3-105">Entradas que são interativas na natureza (onde um nome de usuário/senha é passado como parte de símbolo de autorização) e entradas federadas bem-sucedida atualmente estão incluídas nos logs de entrada.</span><span class="sxs-lookup"><span data-stu-id="853f3-105">Sign-ins that are interactive in nature (where a username/password is passed as part of authorization token) and successful federated sign-ins are currently included in the sign-in logs.</span></span>


## <a name="permissions"></a><span data-ttu-id="853f3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="853f3-106">Permissions</span></span>

<span data-ttu-id="853f3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="853f3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="853f3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="853f3-109">Permission type</span></span>      | <span data-ttu-id="853f3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="853f3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="853f3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="853f3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="853f3-112">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="853f3-112">AuditLog.Read.All</span></span> |
|<span data-ttu-id="853f3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="853f3-113">Delegated (work or school account)</span></span> | <span data-ttu-id="853f3-114">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="853f3-114">Directory.Read.All</span></span> |
|<span data-ttu-id="853f3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="853f3-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="853f3-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="853f3-116">Not supported</span></span>   |
|<span data-ttu-id="853f3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="853f3-117">Application</span></span> | <span data-ttu-id="853f3-118">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="853f3-118">AuditLog.Read.All</span></span> | 
|<span data-ttu-id="853f3-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="853f3-119">Application</span></span> | <span data-ttu-id="853f3-120">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="853f3-120">Directory.Read.All</span></span> | 


<span data-ttu-id="853f3-121">Além disso, os aplicativos devem ser [corretamente registrados](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="853f3-121">In addition, apps must be [properly registered](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to Azure AD.</span></span>

## <a name="http-request"></a><span data-ttu-id="853f3-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="853f3-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /auditLogs/signIns/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="853f3-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="853f3-123">Optional query parameters</span></span>

<span data-ttu-id="853f3-124">Este método dá suporte a Parâmetros de consulta do OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="853f3-124">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="853f3-125">Para obter detalhes sobre como usar esses parâmetros, confira [Parâmetros de consulta do OData](/graph/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="853f3-125">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="853f3-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="853f3-126">Request headers</span></span>

| <span data-ttu-id="853f3-127">Nome</span><span class="sxs-lookup"><span data-stu-id="853f3-127">Name</span></span>      |<span data-ttu-id="853f3-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="853f3-128">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="853f3-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="853f3-129">Authorization</span></span>  | <span data-ttu-id="853f3-130">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="853f3-130">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="853f3-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="853f3-131">Request body</span></span>

<span data-ttu-id="853f3-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="853f3-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="853f3-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="853f3-133">Response</span></span>

<span data-ttu-id="853f3-134">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [signIn](../resources/signin.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="853f3-134">If successful, this method returns a `200 OK` response code and [signIn](../resources/signin.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="853f3-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="853f3-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="853f3-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="853f3-136">Request</span></span>

<span data-ttu-id="853f3-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="853f3-137">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="853f3-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="853f3-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signIns/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="853f3-139">C#</span><span class="sxs-lookup"><span data-stu-id="853f3-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="853f3-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="853f3-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="853f3-141">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="853f3-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="853f3-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="853f3-142">Response</span></span>

<span data-ttu-id="853f3-143">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="853f3-143">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.signIn"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 211
```

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/signIns",
    "value": [{
        "id": "id",
        "createdDateTime": "2018-01-09T21:17:21.5077253Z",
        "userDisplayName": "Jamie Doe",
        "userPrincipalName": "jdoe@contoso.com",
        "userId": "bbb3b4b5-e6e6-f7f5-f7f5-090805040302",
        "appId": "d3590ed6-52b3-4102-aeff-aad2292ab01c",
        "appDisplayName": "Azure",
        "ipAddress": "127.0.0.1",
        "status": {
            "errorCode": 0,
            "failureReason": null,
            "additionalDetails": "SignIn Success & CA Success"
        },
        "clientAppUsed": null,
        "deviceDetail": {
            "deviceId": "34390ed6-52b3-4102-aeff-aad2292abac3",
            "displayName": "DeviceName",
            "operatingSystem": "Windows 10",
            "browser": "Rich Client v3.14.1592.7",
            "isCompliant": true,
            "isManaged": true,
            "trustType": ""
        },
        "location": {
            "city": "Redmond",
            "state": "WA",
            "countryOrRegion": "USA",
            "geoCoordinates": {
                "altitude": 41.589,
                "latitude": 41.589,
                "longitude": -93.6151
            }
        },
        "mfaDetail": {
            "mfaAuthMethod": "Phone Auth",
            "mfaAuthDetail": null
        },
        "correlationId": "17c47d3c-593d-4d08-ac20-813892b87e42",
        "conditionalAccessApplied": true,
        "conditionalAccessPolicies": [{
            "id": "26490ed6-52b3-4102-aeff-aad2292abacf",
            "displayName": "capPolicy",
            "enforcedAccessControls": ["MFA", "TOU"],
            "enforcedSessionControls": ["CloudAppSecurity"],
            "result": "success"
        }],
        "isRisky": false,
        "riskLevel": "low"
    }]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get signIn",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
