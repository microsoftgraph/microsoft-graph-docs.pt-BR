---
title: Listar logons
description: Descreve o método de lista do recurso signIn (entidade) da API Graph Microsoft.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: 8ee9f01bf2b7f590332abcd726e3d6d21b506125
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241125"
---
# <a name="list-signins"></a><span data-ttu-id="da114-103">Listar logons</span><span class="sxs-lookup"><span data-stu-id="da114-103">List signIns</span></span>

<span data-ttu-id="da114-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da114-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="da114-105">Recupera os logons de usuário do Azure AD para seu locatário.</span><span class="sxs-lookup"><span data-stu-id="da114-105">Retrieve the Azure AD user sign-ins for your tenant.</span></span> <span data-ttu-id="da114-106">As inserções interativas de natureza (onde um nome de usuário/senha é passado como parte do token de autenticação) e as inserções federadas bem-sucedidas estão atualmente incluídas nos logs de login.</span><span class="sxs-lookup"><span data-stu-id="da114-106">Sign-ins that are interactive in nature (where a username/password is passed as part of auth token) and successful federated sign-ins are currently included in the sign-in logs.</span></span> <span data-ttu-id="da114-107">O tamanho máximo e padrão da página é de 1.000 objetos e, por padrão, as inscrições mais recentes são retornadas primeiro.</span><span class="sxs-lookup"><span data-stu-id="da114-107">The maximum and default page size is 1,000 objects and by default, the most recent sign-ins are returned first.</span></span>

## <a name="permissions"></a><span data-ttu-id="da114-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="da114-108">Permissions</span></span>

<span data-ttu-id="da114-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="da114-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="da114-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="da114-111">Permission type</span></span>      | <span data-ttu-id="da114-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="da114-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da114-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="da114-113">Delegated (work or school account)</span></span> | <span data-ttu-id="da114-114">AuditLog.Read.All e Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="da114-114">AuditLog.Read.All and Directory.Read.All</span></span> |
|<span data-ttu-id="da114-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="da114-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da114-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="da114-116">Not supported</span></span>   |
|<span data-ttu-id="da114-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="da114-117">Application</span></span> | <span data-ttu-id="da114-118">AuditLog.Read.All e Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="da114-118">AuditLog.Read.All and Directory.Read.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="da114-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="da114-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET auditLogs/signIns
```

## <a name="optional-query-parameters"></a><span data-ttu-id="da114-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="da114-120">Optional query parameters</span></span>

<span data-ttu-id="da114-121">Este método dá suporte `$top` aos `$skiptoken` parâmetros , e `$filter` OData Query para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="da114-121">This method supports the `$top`, `$skiptoken`, and `$filter` OData Query Parameters to help customize the response.</span></span> <span data-ttu-id="da114-122">Para obter detalhes sobre como usar esses parâmetros, confira [Parâmetros de consulta do OData](/graph/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="da114-122">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

## <a name="response"></a><span data-ttu-id="da114-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="da114-123">Response</span></span>

<span data-ttu-id="da114-124">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos de [logon](../resources/signin.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="da114-124">If successful, this method returns a `200 OK` response code and collection of [signIn](../resources/signin.md) objects in the response body.</span></span> <span data-ttu-id="da114-125">A coleção de objetos é listada em ordem decrescente com base em **createdDateTime**.</span><span class="sxs-lookup"><span data-stu-id="da114-125">The collection of objects is listed in descending order based on **createdDateTime**.</span></span>

## <a name="examples"></a><span data-ttu-id="da114-126">Exemplos</span><span class="sxs-lookup"><span data-stu-id="da114-126">Examples</span></span>

### <a name="example-1-list-all-sign-ins"></a><span data-ttu-id="da114-127">Exemplo 1: Listar todas as assinaturas</span><span class="sxs-lookup"><span data-stu-id="da114-127">Example 1: List all sign-ins</span></span>

#### <a name="request"></a><span data-ttu-id="da114-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="da114-128">Request</span></span>

<span data-ttu-id="da114-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="da114-129">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="da114-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="da114-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_signins"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/auditLogs/signIns
```
# <a name="c"></a>[<span data-ttu-id="da114-131">C#</span><span class="sxs-lookup"><span data-stu-id="da114-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-signins-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="da114-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="da114-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-signins-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="da114-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="da114-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-signins-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="da114-134">Java</span><span class="sxs-lookup"><span data-stu-id="da114-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-signins-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="da114-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="da114-135">Response</span></span>

<span data-ttu-id="da114-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="da114-136">Here is an example of the response.</span></span>
><span data-ttu-id="da114-137">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="da114-137">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.signIn",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#auditLogs/signIns",
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/auditLogs/signIns?$top=1&$skiptoken=9177f2e3532fcd4c4d225f68f7b9bdf7_1",
    "value": [
        {
            "id": "66ea54eb-6301-4ee5-be62-ff5a759b0100",
            "createdDateTime": "2020-03-13T19:15:41.6195833Z",
            "userDisplayName": "Test Contoso",
            "userPrincipalName": "testaccount1@contoso.com",
            "userId": "26be570a-ae82-4189-b4e2-a37c6808512d",
            "appId": "de8bc8b5-d9f9-48b1-a8ad-b748da725064",
            "appDisplayName": "Graph explorer",
            "ipAddress": "131.107.159.37",
            "clientAppUsed": "Browser",
            "correlationId": "d79f5bee-5860-4832-928f-3133e22ae912",
            "conditionalAccessStatus": "notApplied",
            "isInteractive": true,
            "riskDetail": "none",
            "riskLevelAggregated": "none",
            "riskLevelDuringSignIn": "none",
            "riskState": "none",
            "riskEventTypes": [],
            "resourceDisplayName": "Microsoft Graph",
            "resourceId": "00000003-0000-0000-c000-000000000000",
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
                    "result": "notEnabled"
                },
                {
                    "id": "6701123a-b4c6-48af-8565-565c8bf7cabc",
                    "displayName": "Medium signin risk block",
                    "enforcedGrantControls": [],
                    "enforcedSessionControls": [],
                    "result": "notEnabled"
                },
              ]
        }
    ]
}
```

### <a name="example-2-retrieve-the-first-10-sign-ins-to-apps-with-the-appdisplayname-that-starts-with-graph"></a><span data-ttu-id="da114-138">Exemplo 2: Recuperar os primeiros 10 logins em aplicativos com o appDisplayName que começa com "Graph"</span><span class="sxs-lookup"><span data-stu-id="da114-138">Example 2: Retrieve the first 10 sign-ins to apps with the appDisplayName that starts with 'Graph'</span></span>

#### <a name="request"></a><span data-ttu-id="da114-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="da114-139">Request</span></span>

<span data-ttu-id="da114-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="da114-140">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_signins_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/auditLogs/signIns?&$filter=startsWith(appDisplayName,'Graph')&top=10
```

#### <a name="response"></a><span data-ttu-id="da114-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="da114-141">Response</span></span>

<span data-ttu-id="da114-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="da114-142">Here is an example of the response.</span></span> <span data-ttu-id="da114-143">A resposta inclui uma `@odata.nextLink` propriedade que contém uma URL que pode ser usada para recuperar os próximos 10 resultados.</span><span class="sxs-lookup"><span data-stu-id="da114-143">The response includes a `@odata.nextLink` property which contains a URL that can be used to retrieve the next 10 results.</span></span>
><span data-ttu-id="da114-144">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="da114-144">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.signIn",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#auditLogs/signIns",
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/auditLogs/signins?$filter=startsWith(appDisplayName%2c%27Graph%27)&$top=10&$skiptoken=70f66c0893886b49370ffdb44cd8d137b1a12b9ba02f34a16f33c5e0f7c42fc7",
    "value": [
        {
            "id": "66ea54eb-6301-4ee5-be62-ff5a759b0100",
            "createdDateTime": "2020-03-13T19:15:41.6195833Z",
            "userDisplayName": "Test Contoso",
            "userPrincipalName": "testaccount1@contoso.com",
            "userId": "26be570a-ae82-4189-b4e2-a37c6808512d",
            "appId": "de8bc8b5-d9f9-48b1-a8ad-b748da725064",
            "appDisplayName": "Graph explorer",
            "ipAddress": "131.107.159.37",
            "clientAppUsed": "Browser",
            "correlationId": "d79f5bee-5860-4832-928f-3133e22ae912",
            "conditionalAccessStatus": "notApplied",
            "isInteractive": true,
            "riskDetail": "none",
            "riskLevelAggregated": "none",
            "riskLevelDuringSignIn": "none",
            "riskState": "none",
            "riskEventTypes": [],
            "resourceDisplayName": "Microsoft Graph",
            "resourceId": "00000003-0000-0000-c000-000000000000",
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
                    "result": "notEnabled"
                },
                {
                    "id": "6701123a-b4c6-48af-8565-565c8bf7cabc",
                    "displayName": "Medium signin risk block",
                    "enforcedGrantControls": [],
                    "enforcedSessionControls": [],
                    "result": "notEnabled"
                },
              ]
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List signIns",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

