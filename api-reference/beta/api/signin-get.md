---
title: Obter entrada
doc_type: apiPageType
description: Obter um objeto signIn que contenha todas as logins de um locatário do Azure Active Directory.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
ms.openlocfilehash: 139ee4c8ae45699f284d866740c494a86fcb05a9
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134124"
---
# <a name="get-signin"></a><span data-ttu-id="41fc8-103">Obter entrada</span><span class="sxs-lookup"><span data-stu-id="41fc8-103">Get signIn</span></span>

<span data-ttu-id="41fc8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41fc8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41fc8-105">Obter um [objeto signIn](../resources/signin.md) que contém um evento de login de usuário específico para seu locatário.</span><span class="sxs-lookup"><span data-stu-id="41fc8-105">Get a [signIn](../resources/signin.md) object that contains a specific user sign-in event for your tenant.</span></span> <span data-ttu-id="41fc8-106">Isso inclui as entrada em que um usuário é solicitado a inserir um nome de usuário ou senha e tokens de sessão.</span><span class="sxs-lookup"><span data-stu-id="41fc8-106">This includes sign-ins where a user is asked to enter a username or password, and session tokens.</span></span>

## <a name="permissions"></a><span data-ttu-id="41fc8-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="41fc8-107">Permissions</span></span>

<span data-ttu-id="41fc8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41fc8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41fc8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="41fc8-110">Permission type</span></span>      | <span data-ttu-id="41fc8-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="41fc8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="41fc8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="41fc8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="41fc8-113">AuditLog.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="41fc8-113">AuditLog.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="41fc8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="41fc8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41fc8-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="41fc8-115">Not supported</span></span> |
| <span data-ttu-id="41fc8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="41fc8-116">Application</span></span> | <span data-ttu-id="41fc8-117">AuditLog.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="41fc8-117">AuditLog.Read.All, Directory.Read.All</span></span> | 

<span data-ttu-id="41fc8-118">Além disso, os aplicativos devem ser [corretamente registrados](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="41fc8-118">In addition, apps must be [properly registered](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to Azure AD.</span></span>

## <a name="http-request"></a><span data-ttu-id="41fc8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="41fc8-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /auditLogs/signIns/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="41fc8-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="41fc8-120">Optional query parameters</span></span>

<span data-ttu-id="41fc8-121">Este método dá suporte a Parâmetros de consulta do OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="41fc8-121">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="41fc8-122">Para obter detalhes sobre como usar esses parâmetros, confira [Parâmetros de consulta do OData](/graph/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="41fc8-122">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="41fc8-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="41fc8-123">Request headers</span></span>

| <span data-ttu-id="41fc8-124">Nome</span><span class="sxs-lookup"><span data-stu-id="41fc8-124">Name</span></span>      |<span data-ttu-id="41fc8-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="41fc8-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="41fc8-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="41fc8-126">Authorization</span></span> | <span data-ttu-id="41fc8-127">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="41fc8-127">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="41fc8-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="41fc8-128">Request body</span></span>

<span data-ttu-id="41fc8-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="41fc8-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41fc8-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="41fc8-130">Response</span></span>

<span data-ttu-id="41fc8-131">Se bem-sucedido, este método retorna `200 OK` um código de resposta e um objeto [signIn](../resources/signin.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="41fc8-131">If successful, this method returns a `200 OK` response code and a [signIn](../resources/signin.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="41fc8-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="41fc8-132">Examples</span></span>

### <a name="example-1-user-signs-in-using-mfa-which-is-triggered-by-a-conditional-access-policy-primary-authentication-is-through-fido"></a><span data-ttu-id="41fc8-133">Exemplo 1: o usuário faz o acesso usando a MFA, que é disparada por uma política de acesso condicional.</span><span class="sxs-lookup"><span data-stu-id="41fc8-133">Example 1: User signs in using MFA, which is triggered by a conditional access policy.</span></span> <span data-ttu-id="41fc8-134">A autenticação principal é por meio do FIDO.</span><span class="sxs-lookup"><span data-stu-id="41fc8-134">Primary authentication is through FIDO.</span></span>

#### <a name="request"></a><span data-ttu-id="41fc8-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="41fc8-135">Request</span></span>

<span data-ttu-id="41fc8-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="41fc8-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="41fc8-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="41fc8-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signIns/{id}
```
# <a name="c"></a>[<span data-ttu-id="41fc8-138">C#</span><span class="sxs-lookup"><span data-stu-id="41fc8-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="41fc8-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="41fc8-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="41fc8-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="41fc8-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="41fc8-141">Java</span><span class="sxs-lookup"><span data-stu-id="41fc8-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="41fc8-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="41fc8-142">Response</span></span>

<span data-ttu-id="41fc8-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="41fc8-143">The following is an example of the response.</span></span>

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
            "id": "66ea54eb-blah-4ee5-be62-ff5a759b0100",
            "createdDateTime": "2020-03-13T19:15:41.6195833Z",
            "userDisplayName": "Test contoso",
            "userPrincipalName": "testaccount1@contoso.com",
            "userId": "26be570a-1111-5555-b4e2-a37c6808512d",
            "appId": "de8bc8b5-5555-6666-a8ad-b748da725064",
            "appDisplayName": "Graph explorer",
            "authenticationRequirement": "MultifactorAuthentication",
            "ipAddress": "131.107.159.37",
            "clientAppUsed": "Browser",
            "userAgent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/80.0.3987.132 Safari/537.36 Edg/80.0.361.66",
            "correlationId": "d79f5bee-blah-4832-928f-3133e22ae912",
            "conditionalAccessStatus": "notApplied",
            "originalRequestId": "66ea54eb-blah-4ee5-be62-ff5a759b0100",
            "isInteractive": true,
            "tokenIssuerName": "",
            "tokenIssuerType": "AzureAD",
            "processingTimeInMilliseconds": 541,
            "riskDetail": "none",
            "riskLevelAggregated": "none",
            "riskLevelDuringSignIn": "none",
            "riskState": "none",
            "riskEventTypes": [],
            "riskEventTypes_v2": [],
            "resourceDisplayName": "Microsoft Graph",
            "resourceId": "00000003-0000-0000-c000-000000000000",
            "authenticationMethodsUsed": [],
            "alternateSignInName": "testaccount2@contoso.com",
            "servicePrincipalName": null,
            "servicePrincipalId": "",
            "mfaDetail": null,
            "status": {
                "errorCode": 0,
                "failureReason": null,
                "additionalDetails": null
            },
            "deviceDetail": {
                "deviceId": "",
                "displayName": null,
                "operatingSystem": "Windows 10",
                "browser": "Edge 80.0.361",
                "isCompliant": null,
                "isManaged": null,
                "trustType": null
            },
            "location": {
                "city": "Redmond",
                "state": "Washington",
                "countryOrRegion": "US",
                "geoCoordinates": {
                    "altitude": null,
                    "latitude": 47.68050003051758,
                    "longitude": -122.12094116210938
                }
            },
            "appliedConditionalAccessPolicies": [
                {
                    "id": "de7e60eb-ed89-4d73-8205-2227def6b7c9",
                    "displayName": "SharePoint limited access for guest workers",
                    "enforcedGrantControls": [],
                    "enforcedSessionControls": [],
                    "result": "notEnabled",
                    "conditionsSatisfied": "none",
                    "conditionsNotSatisfied": "none"
                },
                {
                    "id": "6701123a-b4c6-48af-8565-565c8bf7cabc",
                    "displayName": "Medium signin risk block",
                    "enforcedGrantControls": [],
                    "enforcedSessionControls": [],
                    "result": "notEnabled",
                    "conditionsSatisfied": "none",
                    "conditionsNotSatisfied": "none"
                },
               
            ],
            "authenticationProcessingDetails": [],
            "networkLocationDetails": [],
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
            "authenticationRequirementPolicies": []
        }
    ]
}
```

### <a name="example-2-user-signs-in-with-only-primary-authentication-primary-authentication-is-through-cloud-password"></a><span data-ttu-id="41fc8-144">Exemplo 2: o usuário se insi com apenas a autenticação principal.</span><span class="sxs-lookup"><span data-stu-id="41fc8-144">Example 2: User signs in with only primary authentication.</span></span> <span data-ttu-id="41fc8-145">A autenticação principal é por meio da senha da nuvem.</span><span class="sxs-lookup"><span data-stu-id="41fc8-145">Primary authentication is through cloud password.</span></span>

#### <a name="request"></a><span data-ttu-id="41fc8-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="41fc8-146">Request</span></span>

<span data-ttu-id="41fc8-147">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="41fc8-147">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="41fc8-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="41fc8-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signIns/{id}
```
# <a name="c"></a>[<span data-ttu-id="41fc8-149">C#</span><span class="sxs-lookup"><span data-stu-id="41fc8-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="41fc8-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="41fc8-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="41fc8-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="41fc8-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="41fc8-152">Java</span><span class="sxs-lookup"><span data-stu-id="41fc8-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="41fc8-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="41fc8-153">Response</span></span>

<span data-ttu-id="41fc8-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="41fc8-154">The following is an example of the response.</span></span>

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
      "userPrincipalName":"jdoe@contoso.com",
      "userId":"d7cc485d-2c1b-422c-98fd-5ce52859a4a3",
      "appId":"c44b4083-3bb0-49c1-b47d-974e53cbdf3c",
      "appDisplayName":"Azure Portal",
       "authenticationRequirement": "singleFactorAuthentication",
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
