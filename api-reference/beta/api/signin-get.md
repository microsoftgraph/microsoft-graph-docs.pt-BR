---
title: Obter entrada
description: Recupere um evento específico de entrada do Azure AD para seu locatário.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4b1a6aad8847bfaf2b30439c86c841a85005a3d2
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657368"
---
# <a name="get-signin"></a><span data-ttu-id="9b067-103">Obter entrada</span><span class="sxs-lookup"><span data-stu-id="9b067-103">Get signIn</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b067-104">Recupere um evento específico de entrada do Azure AD para seu locatário.</span><span class="sxs-lookup"><span data-stu-id="9b067-104">Retrieve a specific Azure AD user sign-in event for your tenant.</span></span> <span data-ttu-id="9b067-105">Entradas que são interativas na natureza (onde um nome de usuário/senha é passado como parte de símbolo de autorização) e entradas federadas bem-sucedida atualmente estão incluídas nos logs de entrada.</span><span class="sxs-lookup"><span data-stu-id="9b067-105">Sign-ins that are interactive in nature (where a username/password is passed as part of authorization token) and successful federated sign-ins are currently included in the sign-in logs.</span></span>


## <a name="permissions"></a><span data-ttu-id="9b067-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9b067-106">Permissions</span></span>

<span data-ttu-id="9b067-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b067-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b067-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9b067-109">Permission type</span></span>      | <span data-ttu-id="9b067-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9b067-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9b067-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9b067-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9b067-112">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="9b067-112">AuditLog.Read.All</span></span> |
|<span data-ttu-id="9b067-113">Delegado (conta pessoal da conta Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9b067-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b067-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="9b067-114">Not supported</span></span>   |
|<span data-ttu-id="9b067-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9b067-115">Application</span></span> | <span data-ttu-id="9b067-116">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="9b067-116">AuditLog.Read.All</span></span> | 

<span data-ttu-id="9b067-117">Além disso, os aplicativos devem ser [corretamente registrados](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9b067-117">In addition, apps must be [properly registered](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to Azure AD.</span></span>

## <a name="http-request"></a><span data-ttu-id="9b067-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9b067-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /auditLogs/signIns/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9b067-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9b067-119">Optional query parameters</span></span>

<span data-ttu-id="9b067-120">Este método dá suporte a Parâmetros de consulta do OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9b067-120">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="9b067-121">Para obter detalhes sobre como usar esses parâmetros, confira [Parâmetros de consulta do OData](/graph/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="9b067-121">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9b067-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9b067-122">Request headers</span></span>

| <span data-ttu-id="9b067-123">Nome</span><span class="sxs-lookup"><span data-stu-id="9b067-123">Name</span></span>      |<span data-ttu-id="9b067-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b067-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9b067-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b067-125">Authorization</span></span>  | <span data-ttu-id="9b067-126">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="9b067-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b067-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9b067-127">Request body</span></span>

<span data-ttu-id="9b067-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9b067-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9b067-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b067-129">Response</span></span>

<span data-ttu-id="9b067-130">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [signIn](../resources/signin.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9b067-130">If successful, this method returns a `200 OK` response code and [signIn](../resources/signin.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b067-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9b067-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="9b067-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9b067-132">Request</span></span>

<span data-ttu-id="9b067-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9b067-133">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_signin"
}-->
```http
GET https://graph.microsoft.com/beta/auditLogs/signIns/{id}
```

### <a name="response"></a><span data-ttu-id="9b067-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b067-134">Response</span></span>

<span data-ttu-id="9b067-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9b067-135">Here is an example of the response.</span></span> 

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="9b067-136">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="9b067-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="9b067-137">C#</span><span class="sxs-lookup"><span data-stu-id="9b067-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_signin-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9b067-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="9b067-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_signin-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get signIn",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/signin-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/signin-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
