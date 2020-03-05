---
title: Obter entrada
doc_type: apiPageType
description: Obter um objeto de entrada que contenha todas as entradas de um locatário do Azure Active Directory.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 43a8faae65b3994645b7ef273fdacb74888825e1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453272"
---
# <a name="get-signin"></a><span data-ttu-id="187ec-103">Obter entrada</span><span class="sxs-lookup"><span data-stu-id="187ec-103">Get signIn</span></span>

<span data-ttu-id="187ec-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="187ec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="187ec-105">Obtenha um objeto de [entrada](../resources/signin.md) que contenha um evento de entrada de usuário específico para seu locatário.</span><span class="sxs-lookup"><span data-stu-id="187ec-105">Get a [signIn](../resources/signin.md) object that contains a specific user sign-in event for your tenant.</span></span> <span data-ttu-id="187ec-106">Isso inclui entradas onde um usuário é solicitado a inserir um nome de usuário ou senha e tokens de sessão.</span><span class="sxs-lookup"><span data-stu-id="187ec-106">This includes sign-ins where a user is asked to enter a username or password, and session tokens.</span></span>

## <a name="permissions"></a><span data-ttu-id="187ec-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="187ec-107">Permissions</span></span>

<span data-ttu-id="187ec-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="187ec-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="187ec-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="187ec-110">Permission type</span></span>      | <span data-ttu-id="187ec-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="187ec-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="187ec-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="187ec-112">Delegated (work or school account)</span></span> | <span data-ttu-id="187ec-113">AuditLog. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="187ec-113">AuditLog.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="187ec-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="187ec-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="187ec-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="187ec-115">Not supported</span></span> |
| <span data-ttu-id="187ec-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="187ec-116">Application</span></span> | <span data-ttu-id="187ec-117">AuditLog. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="187ec-117">AuditLog.Read.All, Directory.Read.All</span></span> | 

<span data-ttu-id="187ec-118">Além disso, os aplicativos devem ser [corretamente registrados](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="187ec-118">In addition, apps must be [properly registered](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to Azure AD.</span></span>

## <a name="http-request"></a><span data-ttu-id="187ec-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="187ec-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /auditLogs/signIns/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="187ec-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="187ec-120">Optional query parameters</span></span>

<span data-ttu-id="187ec-121">Este método dá suporte a Parâmetros de consulta do OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="187ec-121">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="187ec-122">Para obter detalhes sobre como usar esses parâmetros, confira [Parâmetros de consulta do OData](/graph/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="187ec-122">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="187ec-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="187ec-123">Request headers</span></span>

| <span data-ttu-id="187ec-124">Nome</span><span class="sxs-lookup"><span data-stu-id="187ec-124">Name</span></span>      |<span data-ttu-id="187ec-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="187ec-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="187ec-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="187ec-126">Authorization</span></span> | <span data-ttu-id="187ec-127">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="187ec-127">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="187ec-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="187ec-128">Request body</span></span>

<span data-ttu-id="187ec-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="187ec-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="187ec-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="187ec-130">Response</span></span>

<span data-ttu-id="187ec-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto de [entrada](../resources/signin.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="187ec-131">If successful, this method returns a `200 OK` response code and a [signIn](../resources/signin.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="187ec-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="187ec-132">Examples</span></span>

### <a name="example-1-user-signs-in-using-mfa-which-is-triggered-by-a-conditional-access-policy-primary-authentication-is-through-fido"></a><span data-ttu-id="187ec-133">Exemplo 1: o usuário faz logon usando MFA, que é disparada por uma política de acesso condicional.</span><span class="sxs-lookup"><span data-stu-id="187ec-133">Example 1: User signs in using MFA, which is triggered by a conditional access policy.</span></span> <span data-ttu-id="187ec-134">A autenticação principal é por meio do FIDO.</span><span class="sxs-lookup"><span data-stu-id="187ec-134">Primary authentication is through FIDO.</span></span>

#### <a name="request"></a><span data-ttu-id="187ec-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="187ec-135">Request</span></span>

<span data-ttu-id="187ec-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="187ec-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="187ec-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="187ec-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signIns/{id}
```
# <a name="c"></a>[<span data-ttu-id="187ec-138">C#</span><span class="sxs-lookup"><span data-stu-id="187ec-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="187ec-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="187ec-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="187ec-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="187ec-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="187ec-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="187ec-141">Response</span></span>

<span data-ttu-id="187ec-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="187ec-142">The following is an example of the response.</span></span>

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

### <a name="example-2-user-signs-in-with-only-primary-authentication-primary-authentication-is-through-cloud-password"></a><span data-ttu-id="187ec-143">Exemplo 2: o usuário entra no com somente autenticação principal.</span><span class="sxs-lookup"><span data-stu-id="187ec-143">Example 2: User signs in with only primary authentication.</span></span> <span data-ttu-id="187ec-144">A autenticação principal é por meio da senha da nuvem.</span><span class="sxs-lookup"><span data-stu-id="187ec-144">Primary authentication is through cloud password.</span></span>

#### <a name="request"></a><span data-ttu-id="187ec-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="187ec-145">Request</span></span>

<span data-ttu-id="187ec-146">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="187ec-146">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="187ec-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="187ec-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signIns/{id}
```
# <a name="c"></a>[<span data-ttu-id="187ec-148">C#</span><span class="sxs-lookup"><span data-stu-id="187ec-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="187ec-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="187ec-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="187ec-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="187ec-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="187ec-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="187ec-151">Response</span></span>

<span data-ttu-id="187ec-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="187ec-152">The following is an example of the response.</span></span>

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
