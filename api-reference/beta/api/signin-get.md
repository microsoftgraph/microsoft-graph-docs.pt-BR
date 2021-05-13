---
title: Obter entrada
doc_type: apiPageType
description: Obter um objeto signIn que contém todas as assinaturas de um Azure Active Directory locatário.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
ms.openlocfilehash: cb002faa818ee63f53282b9fb165339b20f4e484
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474075"
---
# <a name="get-signin"></a><span data-ttu-id="41754-103">Obter entrada</span><span class="sxs-lookup"><span data-stu-id="41754-103">Get signIn</span></span>

<span data-ttu-id="41754-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41754-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41754-105">Obter um [objeto signIn](../resources/signin.md) que contém um evento de login de usuário específico para seu locatário.</span><span class="sxs-lookup"><span data-stu-id="41754-105">Get a [signIn](../resources/signin.md) object that contains a specific user sign-in event for your tenant.</span></span> <span data-ttu-id="41754-106">Isso inclui as ingressações em que um usuário é solicitado a inserir um nome de usuário ou senha e tokens de sessão.</span><span class="sxs-lookup"><span data-stu-id="41754-106">This includes sign-ins where a user is asked to enter a username or password, and session tokens.</span></span>

## <a name="permissions"></a><span data-ttu-id="41754-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="41754-107">Permissions</span></span>

<span data-ttu-id="41754-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41754-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41754-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="41754-110">Permission type</span></span>      | <span data-ttu-id="41754-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="41754-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="41754-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="41754-112">Delegated (work or school account)</span></span> | <span data-ttu-id="41754-113">AuditLog.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="41754-113">AuditLog.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="41754-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="41754-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41754-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="41754-115">Not supported</span></span> |
| <span data-ttu-id="41754-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="41754-116">Application</span></span> | <span data-ttu-id="41754-117">AuditLog.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="41754-117">AuditLog.Read.All, Directory.Read.All</span></span> | 

<span data-ttu-id="41754-118">Além disso, os aplicativos devem ser [corretamente registrados](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="41754-118">In addition, apps must be [properly registered](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to Azure AD.</span></span>

## <a name="http-request"></a><span data-ttu-id="41754-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="41754-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /auditLogs/signIns/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="41754-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="41754-120">Optional query parameters</span></span>

<span data-ttu-id="41754-121">Este método dá suporte a Parâmetros de consulta do OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="41754-121">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="41754-122">Para obter detalhes sobre como usar esses parâmetros, confira [Parâmetros de consulta do OData](/graph/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="41754-122">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="41754-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="41754-123">Request headers</span></span>

| <span data-ttu-id="41754-124">Nome</span><span class="sxs-lookup"><span data-stu-id="41754-124">Name</span></span>      |<span data-ttu-id="41754-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="41754-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="41754-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="41754-126">Authorization</span></span> | <span data-ttu-id="41754-127">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="41754-127">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="41754-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="41754-128">Request body</span></span>

<span data-ttu-id="41754-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="41754-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41754-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="41754-130">Response</span></span>

<span data-ttu-id="41754-131">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto signIn](../resources/signin.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="41754-131">If successful, this method returns a `200 OK` response code and a [signIn](../resources/signin.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41754-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="41754-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="41754-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="41754-133">Request</span></span>

<span data-ttu-id="41754-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="41754-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="41754-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="41754-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signIns/66ea54eb-blah-4ee5-be62-ff5a759b0100
```
# <a name="c"></a>[<span data-ttu-id="41754-136">C#</span><span class="sxs-lookup"><span data-stu-id="41754-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="41754-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="41754-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="41754-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="41754-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="41754-139">Java</span><span class="sxs-lookup"><span data-stu-id="41754-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="41754-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="41754-140">Response</span></span>

<span data-ttu-id="41754-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="41754-141">The following is an example of the response.</span></span>
><span data-ttu-id="41754-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="41754-142">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.signIn"
} -->


```http
HTTP/1.1 200 OK
Content-type: application/json

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
      "authenticationStepDateTime": "2018-11-06T18:48:03.8313489Z",
      "authenticationMethod": "FIDO2",
      "authenticationMethodDetail": "1G54395783",
      "succeeded": true,
      "authenticationStepResultDetail": "methodSucceeded",
      "authenticationStepRequirement": "Primary authentication"
    },
    {
      "authenticationStepDateTime": "2018-11-06T18:48:12.94725647Z",
      "authenticationMethod": "Claim in access token",
      "authenticationMethodDetail": null,
      "succeeded": true,
      "authenticationStepResultDetail": "methodSucceeded",
      "authenticationStepRequirement": "MFA"
    }
  ],
  "authenticationRequirementPolicies": []
}
```
