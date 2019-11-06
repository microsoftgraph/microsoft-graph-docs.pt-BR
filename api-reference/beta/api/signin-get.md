---
title: Obter entrada
doc_type: apiPageType
description: Obter um objeto de entrada que contenha todas as entradas de um locatário do Azure Active Directory.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7e9f7db8bfe283e570f4b35d86badada1e64665d
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997593"
---
# <a name="get-signin"></a><span data-ttu-id="ae7d4-103">Obter entrada</span><span class="sxs-lookup"><span data-stu-id="ae7d4-103">Get signIn</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae7d4-104">Obtenha um objeto de [entrada](../resources/signin.md) que contenha um evento de entrada de usuário específico para seu locatário.</span><span class="sxs-lookup"><span data-stu-id="ae7d4-104">Get a [signIn](../resources/signin.md) object that contains a specific user sign-in event for your tenant.</span></span> <span data-ttu-id="ae7d4-105">Isso inclui entradas onde um usuário é solicitado a inserir um nome de usuário ou senha e tokens de sessão.</span><span class="sxs-lookup"><span data-stu-id="ae7d4-105">This includes sign-ins where a user is asked to enter a username or password, and session tokens.</span></span>

## <a name="permissions"></a><span data-ttu-id="ae7d4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ae7d4-106">Permissions</span></span>

<span data-ttu-id="ae7d4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae7d4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae7d4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ae7d4-109">Permission type</span></span>      | <span data-ttu-id="ae7d4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ae7d4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="ae7d4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ae7d4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ae7d4-112">AuditLog. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="ae7d4-112">AuditLog.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="ae7d4-113">Delegado (conta pessoal da conta Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ae7d4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae7d4-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="ae7d4-114">Not supported</span></span> |
| <span data-ttu-id="ae7d4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ae7d4-115">Application</span></span> | <span data-ttu-id="ae7d4-116">AuditLog. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="ae7d4-116">AuditLog.Read.All, Directory.Read.All</span></span> | 

<span data-ttu-id="ae7d4-117">Além disso, os aplicativos devem ser [corretamente registrados](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ae7d4-117">In addition, apps must be [properly registered](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to Azure AD.</span></span>

## <a name="http-request"></a><span data-ttu-id="ae7d4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ae7d4-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /auditLogs/signIns/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ae7d4-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ae7d4-119">Optional query parameters</span></span>

<span data-ttu-id="ae7d4-120">Este método dá suporte a Parâmetros de consulta do OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ae7d4-120">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="ae7d4-121">Para obter detalhes sobre como usar esses parâmetros, confira [Parâmetros de consulta do OData](/graph/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="ae7d4-121">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ae7d4-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ae7d4-122">Request headers</span></span>

| <span data-ttu-id="ae7d4-123">Nome</span><span class="sxs-lookup"><span data-stu-id="ae7d4-123">Name</span></span>      |<span data-ttu-id="ae7d4-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae7d4-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ae7d4-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae7d4-125">Authorization</span></span> | <span data-ttu-id="ae7d4-126">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="ae7d4-126">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ae7d4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ae7d4-127">Request body</span></span>

<span data-ttu-id="ae7d4-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ae7d4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae7d4-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae7d4-129">Response</span></span>

<span data-ttu-id="ae7d4-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto de [entrada](../resources/signin.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ae7d4-130">If successful, this method returns a `200 OK` response code and a [signIn](../resources/signin.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ae7d4-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ae7d4-131">Examples</span></span>

### <a name="example-1-user-signs-in-using-mfa-which-is-triggered-by-a-conditional-access-policy-primary-authentication-is-through-fido"></a><span data-ttu-id="ae7d4-132">Exemplo 1: o usuário faz logon usando MFA, que é disparada por uma política de acesso condicional.</span><span class="sxs-lookup"><span data-stu-id="ae7d4-132">Example 1: User signs in using MFA, which is triggered by a conditional access policy.</span></span> <span data-ttu-id="ae7d4-133">A autenticação principal é por meio do FIDO.</span><span class="sxs-lookup"><span data-stu-id="ae7d4-133">Primary authentication is through FIDO.</span></span>

#### <a name="request"></a><span data-ttu-id="ae7d4-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ae7d4-134">Request</span></span>

<span data-ttu-id="ae7d4-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ae7d4-135">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ae7d4-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="ae7d4-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signIns/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ae7d4-137">C#</span><span class="sxs-lookup"><span data-stu-id="ae7d4-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ae7d4-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ae7d4-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ae7d4-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ae7d4-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="ae7d4-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae7d4-140">Response</span></span>

<span data-ttu-id="ae7d4-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ae7d4-141">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.signIn"
} -->


```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 211

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/signIns",
  "value": [
    {
      "id":"b01b1726-0147-425e-a7f7-21f252050400",
      "createdDateTime":"2018-11-06T18:48:33.8527147Z",
      "userDisplayName":"Jon Doe",
      "userPrincipalName":"jdoe@www.contoso.com",
      "userId":"d7cc485d-2c1b-422c-98fd-5ce52859a4a3",
      "appId":"c44b4083-3bb0-49c1-b47d-974e53cbdf3c",
      "appDisplayName":"Azure Portal",
      "ipAddress":"207.254.19.10",
      "clientAppUsed":"Browser",
      "authenticationDetails": [ 
        {
          "authenticationStepDateTime":"2018-11-06T18:48:03.8313489Z",
          "authenticationMethod":"FIDO2",
          "authenticationMethodDetail":"1G54395783",
          "succeeded":true,
          "authenticationStepResultDetail":"methodSucceeded",
          "authenticationStepRequirement":"Primary authentication"
        },
        {
          "authenticationStepDateTime":"2018-11-06T18:48:12.94725647Z",
          "authenticationMethod":"Claim in access token",
          "authenticationMethodDetail":null,
          "succeeded":true,
          "authenticationStepResultDetail":"methodSucceeded",
          "authenticationStepRequirement":"MFA"
        }
      ],
      "correlationId":"65dd87ce-2183-419e-81a9-d6e20379bcc2",
      "conditionalAccessStatus":"applied",
      "isInteractive":true,
      "tokenIssuerName":null,
      "tokenIssuerType":"AzureAD",
      "processingTimeInMilliseconds":100,
      "riskDetail":"none",
      "riskLevelAggregated":"none",
      "riskLevelDuringsignIn":"none",
      "riskState":"none",
      "riskEventTypes":[],
      "resourceDisplayName":"windows azure service management api",
      "resourceId":"797f4846-ba00-4fd7-ba43-dac1f8f63013",
      "status":{},
      "deviceDetail": {
        "deviceId":null,
        "displayName":null,
        "operatingSystem":"Windows 7",
        "browser":"Chrome 63.0.3239",
        "isCompliant":null,
        "isManaged":null,
        "trustType":null
      },
      "location": {
        "city":"Lithia Springs",
        "state":"Georgia",
        "countryOrRegion":"US",
        "geoCoordinates": {
          "altitude":null,
          "latitude":33.7930908203125,
          "longitude":-84.445358276367188
        }
      },
      "appliedConditionalAccessPolicies": [
        {
          "id":"6551c58c-e5da-4036-a6ea-c2c3fad264f1",
          "displayName":"MFA policy",
          "enforcedGrantControls": [
            "Mfa",
            "RequireCompliantDevice"
          ],
          "enforcedSessionControls":[],
          "result":"applied"
        },
        {
          "id":"b645a140-20fe-4ce0-a724-18ab201e9026",
          "displayName":"PipelineTest4",
          "enforcedGrantControls":[],
          "enforcedSessionControls":[],
          "result":"notEnabled"
        }
      ],
      "authenticationProcessingDetails":[],
      "networkLocationDetails":[]
    }
  ]
}
```

### <a name="example-2-user-signs-in-with-only-primary-authentication-primary-authentication-is-through-cloud-password"></a><span data-ttu-id="ae7d4-142">Exemplo 2: o usuário entra no com somente autenticação principal.</span><span class="sxs-lookup"><span data-stu-id="ae7d4-142">Example 2: User signs in with only primary authentication.</span></span> <span data-ttu-id="ae7d4-143">A autenticação principal é por meio da senha da nuvem.</span><span class="sxs-lookup"><span data-stu-id="ae7d4-143">Primary authentication is through cloud password.</span></span>

#### <a name="request"></a><span data-ttu-id="ae7d4-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ae7d4-144">Request</span></span>

<span data-ttu-id="ae7d4-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ae7d4-145">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ae7d4-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="ae7d4-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signIns/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ae7d4-147">C#</span><span class="sxs-lookup"><span data-stu-id="ae7d4-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ae7d4-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ae7d4-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ae7d4-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ae7d4-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ae7d4-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae7d4-150">Response</span></span>

<span data-ttu-id="ae7d4-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ae7d4-151">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.signIn"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 211

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/signIns",
  "value": [
    {
      "id":"b01b1726-0147-425e-a7f7-21f252050400",
      "createdDateTime":"2018-11-06T18:48:33.8527147Z",
      "userDisplayName":"Jon Doe",
      "userPrincipalName":"jdoe@www.contoso.com",
      "userId":"d7cc485d-2c1b-422c-98fd-5ce52859a4a3",
      "appId":"c44b4083-3bb0-49c1-b47d-974e53cbdf3c",
      "appDisplayName":"Azure Portal",
      "ipAddress":"207.254.19.10",
      "clientAppUsed":"Browser",
      "authenticationDetails": [
        {
          "authenticationStepDateTime":"2018-11-06T18:48:03.8313489Z",
          "authenticationMethod":"Password",
          "authenticationMethodDetail":"Cloud password",
          "succeeded":true,
          "authenticationStepResultDetail":"methodSucceeded",
          "authenticationStepRequirement":"Primary authentication"
        }
      ],
      "correlationId":"65dd87ce-2183-419e-81a9-d6e20379bcc2",
      "conditionalAccessStatus":"applied",
      "isInteractive":true,
      "tokenIssuerName":null,
      "tokenIssuerType":"AzureAD",
      "processingTimeInMilliseconds":100,
      "riskDetail":"none",
      "riskLevelAggregated":"none",
      "riskLevelDuringsignIn":"none",
      "riskState":"none",
      "riskEventTypes":[],
      "resourceDisplayName":"windows azure service management api",
      "resourceId":"797f4846-ba00-4fd7-ba43-dac1f8f63013",
      "status":{},
      "deviceDetail": {
        "deviceId":null,
        "displayName":null,
        "operatingSystem":"Windows 7",
        "browser":"Chrome 63.0.3239",
        "isCompliant":null,
        "isManaged":null,
        "trustType":null
      },
      "location": {
        "city":"Lithia Springs",
        "state":"Georgia",
        "countryOrRegion":"US",
        "geoCoordinates": {
          "altitude":null,
          "latitude":33.7930908203125,
          "longitude":-84.445358276367188
        }
      },
      "appliedConditionalAccessPolicies": [
        {
          "id":"6551c58c-e5da-4036-a6ea-c2c3fad264f1",
          "displayName":"MFA policy",
          "enforcedGrantControls": [
            "Mfa",
            "RequireCompliantDevice"
          ],
          "enforcedSessionControls":[],
          "result":"notApplied"
        },
        {
          "id":"b645a140-20fe-4ce0-a724-18ab201e9026",
          "displayName":"PipelineTest4",
          "enforcedGrantControls":[],
          "enforcedSessionControls":[],
          "result":"notEnabled"
        }
      ],
      "authenticationProcessingDetails":[],
      "networkLocationDetails":[]
    }
  ]
}
```
