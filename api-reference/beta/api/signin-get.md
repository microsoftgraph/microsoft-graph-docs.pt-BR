---
title: Obter entrada
description: Recupera as entradas de usuário do Azure AD usuário para seu locatário. Entradas que são interativas na natureza (onde um nome de usuário/senha é passado como parte de símbolo de autorização) e entradas federadas bem-sucedida atualmente estão incluídas nos logs de entrada.
localization_priority: Priority
ms.openlocfilehash: 5d2d0513f44196d48aa863ac19838af13d960f85
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643878"
---
# <a name="get-signin"></a><span data-ttu-id="f0ada-104">Obter entrada</span><span class="sxs-lookup"><span data-stu-id="f0ada-104">Get signIn</span></span>
<span data-ttu-id="f0ada-105">Recupera as entradas de usuário do Azure AD usuário para seu locatário.</span><span class="sxs-lookup"><span data-stu-id="f0ada-105">Retrieves the Azure AD user sign-ins for your tenant.</span></span> <span data-ttu-id="f0ada-106">Entradas que são interativas na natureza (onde um nome de usuário/senha é passado como parte de símbolo de autorização) e entradas federadas bem-sucedida atualmente estão incluídas nos logs de entrada.</span><span class="sxs-lookup"><span data-stu-id="f0ada-106">Sign-ins that are interactive in nature (where a username/password is passed as part of authorization token) and successful federated sign-ins are currently included in the sign-in logs.</span></span>


## <a name="permissions"></a><span data-ttu-id="f0ada-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f0ada-107">Permissions</span></span>
<span data-ttu-id="f0ada-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0ada-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0ada-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f0ada-110">Permission type</span></span>      | <span data-ttu-id="f0ada-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f0ada-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f0ada-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f0ada-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f0ada-113">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="f0ada-113">AuditLog.Read.All</span></span> |
|<span data-ttu-id="f0ada-114">Delegado (conta pessoal da conta Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f0ada-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0ada-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f0ada-115">Not supported</span></span>   |
|<span data-ttu-id="f0ada-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f0ada-116">Application</span></span> | <span data-ttu-id="f0ada-117">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="f0ada-117">AuditLog.Read.All</span></span> | 

<span data-ttu-id="f0ada-118">Além disso, os aplicativos devem ser [corretamente registrados](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f0ada-118">In addition, apps must be [properly registered](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to Azure AD.</span></span>

## <a name="http-request"></a><span data-ttu-id="f0ada-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f0ada-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /auditLogs/signIns/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f0ada-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f0ada-120">Optional query parameters</span></span>
<span data-ttu-id="f0ada-121">Este método dá suporte aos seguintes Parâmetros de Consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f0ada-121">This method supports the following OData Query Parameters to help customize the response.</span></span> <span data-ttu-id="f0ada-122">Verifique [parâmetros de consulta de OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) sobre como usar esses parâmetros.</span><span class="sxs-lookup"><span data-stu-id="f0ada-122">Check [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) for how to use these parameters.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f0ada-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f0ada-123">Request headers</span></span>
| <span data-ttu-id="f0ada-124">Nome</span><span class="sxs-lookup"><span data-stu-id="f0ada-124">Name</span></span>      |<span data-ttu-id="f0ada-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0ada-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f0ada-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0ada-126">Authorization</span></span>  | <span data-ttu-id="f0ada-127">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="f0ada-127">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0ada-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f0ada-128">Request body</span></span>
<span data-ttu-id="f0ada-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f0ada-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f0ada-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0ada-130">Response</span></span>
<span data-ttu-id="f0ada-131">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [signIn](../resources/signin.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f0ada-131">If successful, this method returns a `200 OK` response code and [signIn](../resources/signin.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f0ada-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f0ada-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f0ada-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f0ada-133">Request</span></span>
<span data-ttu-id="f0ada-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f0ada-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "reque|location/city| eq, startswith|
st",
  "name": "get_signin"
}-->
```http
GET https://graph.microsoft.com/beta/auditLogs/signIns/{id}
```
##### <a name="response"></a><span data-ttu-id="f0ada-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0ada-135">Response</span></span>
<span data-ttu-id="f0ada-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f0ada-136">Here is an example of the response.</span></span> 
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
            "additionalDetails": "SignIn Success & CA Sucess"
        },
        "clientAppUsed": null,
        "deviceDetail": {
            "deviceId": "34390ed6-52b3-4102-aeff-aad2292abac3",
            "displayName": "DeviceName",
            "operatingSystem": "Windows 10",
            "browser": "Rich Client v1.0.2016.0",
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
  "tocPath": ""
}-->
