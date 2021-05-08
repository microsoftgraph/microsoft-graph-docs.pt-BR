---
title: Obter entrada
description: Descreve o método get do recurso signIn (entidade) da API Graph Microsoft.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: 007047fe0fe9364f99af31ee0447967da7618060
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52238397"
---
# <a name="get-signin"></a><span data-ttu-id="378ed-103">Obter entrada</span><span class="sxs-lookup"><span data-stu-id="378ed-103">Get signIn</span></span>

<span data-ttu-id="378ed-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="378ed-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="378ed-105">Recupere um evento específico de entrada do Azure AD para seu locatário.</span><span class="sxs-lookup"><span data-stu-id="378ed-105">Retrieve a specific Azure AD user sign-in event for your tenant.</span></span> <span data-ttu-id="378ed-106">As inserções interativas de natureza (onde um nome de usuário/senha é passado como parte do token de autenticação) e as inserções federadas bem-sucedidas estão atualmente incluídas nos logs de login.</span><span class="sxs-lookup"><span data-stu-id="378ed-106">Sign-ins that are interactive in nature (where a username/password is passed as part of auth token) and successful federated sign-ins are currently included in the sign-in logs.</span></span>

## <a name="permissions"></a><span data-ttu-id="378ed-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="378ed-107">Permissions</span></span>

<span data-ttu-id="378ed-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="378ed-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="378ed-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="378ed-110">Permission type</span></span>      | <span data-ttu-id="378ed-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="378ed-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="378ed-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="378ed-112">Delegated (work or school account)</span></span> | <span data-ttu-id="378ed-113">AuditLog.Read.All e Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="378ed-113">AuditLog.Read.All and Directory.Read.All</span></span> |
|<span data-ttu-id="378ed-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="378ed-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="378ed-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="378ed-115">Not supported</span></span>   |
|<span data-ttu-id="378ed-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="378ed-116">Application</span></span> | <span data-ttu-id="378ed-117">AuditLog.Read.All e Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="378ed-117">AuditLog.Read.All and Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="378ed-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="378ed-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /auditLogs/signIns/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="378ed-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="378ed-119">Optional query parameters</span></span>

<span data-ttu-id="378ed-120">Este método dá suporte a Parâmetros de consulta do OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="378ed-120">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="378ed-121">Para obter detalhes sobre como usar esses parâmetros, confira [Parâmetros de consulta do OData](/graph/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="378ed-121">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="378ed-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="378ed-122">Request headers</span></span>

| <span data-ttu-id="378ed-123">Nome</span><span class="sxs-lookup"><span data-stu-id="378ed-123">Name</span></span>      |<span data-ttu-id="378ed-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="378ed-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="378ed-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="378ed-125">Authorization</span></span>  | <span data-ttu-id="378ed-126">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="378ed-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="378ed-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="378ed-127">Request body</span></span>

<span data-ttu-id="378ed-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="378ed-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="378ed-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="378ed-129">Response</span></span>

<span data-ttu-id="378ed-130">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [signIn](../resources/signin.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="378ed-130">If successful, this method returns a `200 OK` response code and [signIn](../resources/signin.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="378ed-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="378ed-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="378ed-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="378ed-132">Request</span></span>

<span data-ttu-id="378ed-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="378ed-133">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_signin"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/auditLogs/signIns/66ea54eb-6301-4ee5-be62-ff5a759b0100
```

### <a name="response"></a><span data-ttu-id="378ed-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="378ed-134">Response</span></span>

<span data-ttu-id="378ed-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="378ed-135">Here is an example of the response.</span></span>
><span data-ttu-id="378ed-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="378ed-136">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.signIn"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#auditLogs/signIns",
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
  "description": "Get signIn",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

