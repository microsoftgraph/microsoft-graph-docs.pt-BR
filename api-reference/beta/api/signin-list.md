---
title: Listar logons
doc_type: apiPageType
description: Obter uma lista dos logins do usuário em um Azure Active Directory locatário.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
ms.openlocfilehash: c85788d7ee1023e8f21097561105d7715f2074cd
ms.sourcegitcommit: 8a9be6f65f62f29973508d82e0348d4142c18f23
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2021
ms.locfileid: "53129486"
---
# <a name="list-signins"></a><span data-ttu-id="f0c91-103">Listar logons</span><span class="sxs-lookup"><span data-stu-id="f0c91-103">List signIns</span></span>

<span data-ttu-id="f0c91-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0c91-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0c91-105">Obter uma lista de [objetos signIn.](../resources/signin.md)</span><span class="sxs-lookup"><span data-stu-id="f0c91-105">Get a list of [signIn](../resources/signin.md) objects.</span></span> <span data-ttu-id="f0c91-106">A lista contém as assinaturas do usuário para seu Azure Active Directory locatário.</span><span class="sxs-lookup"><span data-stu-id="f0c91-106">The list contains the user sign-ins for your Azure Active Directory tenant.</span></span> <span data-ttu-id="f0c91-107">As inserções em que um nome de usuário e senha são passados como parte do token de autorização e as inserções federadas bem-sucedidas estão incluídas nos logs de login.</span><span class="sxs-lookup"><span data-stu-id="f0c91-107">Sign-ins where a username and password are passed as part of authorization token, and successful federated sign-ins are currently included in the sign-in logs.</span></span> <span data-ttu-id="f0c91-108">O tamanho máximo e padrão da página é de 1.000 objetos e, por padrão, as inscrições mais recentes são retornadas primeiro.</span><span class="sxs-lookup"><span data-stu-id="f0c91-108">The maximum and default page size is 1,000 objects and by default, the most recent sign-ins are returned first.</span></span>

## <a name="permissions"></a><span data-ttu-id="f0c91-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="f0c91-109">Permissions</span></span>

<span data-ttu-id="f0c91-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0c91-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f0c91-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f0c91-112">Permission type</span></span> | <span data-ttu-id="f0c91-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f0c91-113">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="f0c91-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f0c91-114">Delegated (work or school account)</span></span> | <span data-ttu-id="f0c91-115">AuditLog.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="f0c91-115">AuditLog.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="f0c91-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f0c91-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0c91-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f0c91-117">Not supported</span></span> |
| <span data-ttu-id="f0c91-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f0c91-118">Application</span></span> | <span data-ttu-id="f0c91-119">AuditLog.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="f0c91-119">AuditLog.Read.All, Directory.Read.All</span></span> | 

<span data-ttu-id="f0c91-120">Os aplicativos devem [estar registrados corretamente](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f0c91-120">Apps must be [properly registered](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to Azure AD.</span></span>

<span data-ttu-id="f0c91-121">Além das permissões delegadas, o usuário inscreveu precisa pertencer a uma das seguintes funções de diretório que permitem ler relatórios de logons.</span><span class="sxs-lookup"><span data-stu-id="f0c91-121">In addition to the delegated permissions, the signed-in user needs to belong to one of the following directory roles that allow them to read sign-in reports.</span></span> <span data-ttu-id="f0c91-122">Para saber mais sobre funções de diretório, consulte Funções do [Azure AD integrados](/azure/active-directory/roles/permissions-reference):</span><span class="sxs-lookup"><span data-stu-id="f0c91-122">To learn more about directory roles, see [Azure AD built-in roles](/azure/active-directory/roles/permissions-reference):</span></span>
+ <span data-ttu-id="f0c91-123">Administrador global</span><span class="sxs-lookup"><span data-stu-id="f0c91-123">Global Administrator</span></span>
+ <span data-ttu-id="f0c91-124">Leitor global</span><span class="sxs-lookup"><span data-stu-id="f0c91-124">Global Reader</span></span>
+ <span data-ttu-id="f0c91-125">Leitor de Relatórios</span><span class="sxs-lookup"><span data-stu-id="f0c91-125">Reports Reader</span></span>
+ <span data-ttu-id="f0c91-126">Administrador de Segurança</span><span class="sxs-lookup"><span data-stu-id="f0c91-126">Security Administrator</span></span>
+ <span data-ttu-id="f0c91-127">Operador de segurança</span><span class="sxs-lookup"><span data-stu-id="f0c91-127">Security Operator</span></span>
+ <span data-ttu-id="f0c91-128">Leitor de segurança</span><span class="sxs-lookup"><span data-stu-id="f0c91-128">Security Reader</span></span>

## <a name="http-request"></a><span data-ttu-id="f0c91-129">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f0c91-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET auditLogs/signIns
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f0c91-130">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f0c91-130">Optional query parameters</span></span>

<span data-ttu-id="f0c91-131">Este método dá suporte `$top` aos `$skiptoken` parâmetros , e `$filter` OData Query para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f0c91-131">This method supports the `$top`, `$skiptoken`, and `$filter` OData Query Parameters to help customize the response.</span></span> <span data-ttu-id="f0c91-132">Para obter detalhes sobre como usar esses parâmetros, confira [Parâmetros de consulta do OData](/graph/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="f0c91-132">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f0c91-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f0c91-133">Request headers</span></span>

| <span data-ttu-id="f0c91-134">Nome</span><span class="sxs-lookup"><span data-stu-id="f0c91-134">Name</span></span>      |<span data-ttu-id="f0c91-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0c91-135">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f0c91-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="f0c91-136">Authorization</span></span> | <span data-ttu-id="f0c91-137">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="f0c91-137">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="f0c91-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f0c91-138">Request body</span></span>

<span data-ttu-id="f0c91-139">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f0c91-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f0c91-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0c91-140">Response</span></span>

<span data-ttu-id="f0c91-141">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos de [logon](../resources/signin.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f0c91-141">If successful, this method returns a `200 OK` response code and collection of [signIn](../resources/signin.md) objects in the response body.</span></span> <span data-ttu-id="f0c91-142">A coleção de objetos é listada em ordem decrescente com base em **createdDateTime**.</span><span class="sxs-lookup"><span data-stu-id="f0c91-142">The collection of objects is listed in descending order based on **createdDateTime**.</span></span>

## <a name="examples"></a><span data-ttu-id="f0c91-143">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f0c91-143">Examples</span></span>

### <a name="example-1-list-all-sign-ins"></a><span data-ttu-id="f0c91-144">Exemplo 1: Listar todas as assinaturas</span><span class="sxs-lookup"><span data-stu-id="f0c91-144">Example 1: List all sign-ins</span></span>
<span data-ttu-id="f0c91-145">Neste exemplo, o objeto de resposta mostra o usuário que se inscreveu usando o MFA que foi disparado por uma política de acesso condicional, e o método de autenticação principal é por meio do FIDO.</span><span class="sxs-lookup"><span data-stu-id="f0c91-145">In this example, the response object shows the user signed in using MFA which was triggered by a conditional access policy, and the primary authentication method is through FIDO.</span></span>

#### <a name="request"></a><span data-ttu-id="f0c91-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f0c91-146">Request</span></span>

<span data-ttu-id="f0c91-147">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f0c91-147">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f0c91-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="f0c91-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signins_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signIns
```
# <a name="c"></a>[<span data-ttu-id="f0c91-149">C#</span><span class="sxs-lookup"><span data-stu-id="f0c91-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signins-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f0c91-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f0c91-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signins-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f0c91-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f0c91-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signins-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f0c91-152">Java</span><span class="sxs-lookup"><span data-stu-id="f0c91-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signins-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="f0c91-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0c91-153">Response</span></span>
><span data-ttu-id="f0c91-154">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f0c91-154">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.signIn"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

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
      "authenticationRequirement": "multiFactorAuthentication",
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
      "alternateSignInName": "testaccount2.contoso.com",
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
### <a name="example-2-retrieve-the-first-10-sign-ins-to-apps-with-the-appdisplayname-that-starts-with-azure"></a><span data-ttu-id="f0c91-155">Exemplo 2: Recuperar os primeiros 10 logins em aplicativos com o appDisplayName que começa com 'Azure'</span><span class="sxs-lookup"><span data-stu-id="f0c91-155">Example 2: Retrieve the first 10 sign-ins to apps with the appDisplayName that starts with 'Azure'</span></span>

<span data-ttu-id="f0c91-156">Neste exemplo, o objeto de resposta mostra o usuário se inscreveu usando apenas o método de autenticação principal, uma senha de nuvem.</span><span class="sxs-lookup"><span data-stu-id="f0c91-156">In this example, the response object shows the user signed in using only their primary authentication method—a cloud password.</span></span> <span data-ttu-id="f0c91-157">A resposta inclui uma `@odata.nextLink` propriedade que contém uma URL que pode ser usada para recuperar os próximos 10 resultados.</span><span class="sxs-lookup"><span data-stu-id="f0c91-157">The response includes a `@odata.nextLink` property which contains a URL that can be used to retrieve the next 10 results.</span></span>

#### <a name="request"></a><span data-ttu-id="f0c91-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f0c91-158">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_signins_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signins?&$filter=startsWith(appDisplayName,'Azure')&top=10
```

#### <a name="response"></a><span data-ttu-id="f0c91-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0c91-159">Response</span></span>
><span data-ttu-id="f0c91-160">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f0c91-160">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.signIn"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/signIns",
  "@odata.nextLink": "https://graph.microsoft.com/beta/auditLogs/signins?$filter=startsWith(appDisplayName%2c%27Azure%27)&$top=10&$skiptoken=3cff228c89605cc89b0dc753668deef4153e8644caa6d83ed1bb5f711b21cba4",
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
      "ipAddress":"131.107.159.37",
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
      "resourceDisplayName":"Windows Azure Service Management API",
      "resourceId":"797f4846-ba00-4fd7-ba43-dac1f8f63013",
      "status":{},
      "deviceDetail": {
        "deviceId":null,
        "displayName":null,
        "operatingSystem":"Windows 10",
        "browser":"Chrome 90.0.4430",
        "isCompliant":null,
        "isManaged":null,
        "trustType":null
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
