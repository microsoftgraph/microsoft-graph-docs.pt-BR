---
title: Lista signIns
description: Recupera as Azure AD entradas do usuário para seu locatário. Entradas que são interativas em natureza (onde uma nome de usuário/senha é passada como parte do token de autorização) e entradas federadas bem-sucedidas atualmente estão incluídas nos logs de entrar.  Os mais recentes signIns são retornados pela primeira vez.
localization_priority: Priority
ms.openlocfilehash: 8596bd168a3e10cbea9e15e2f61d6bd668fd27b5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861786"
---
# <a name="list-signins"></a><span data-ttu-id="2e0c4-105">Lista signIns</span><span class="sxs-lookup"><span data-stu-id="2e0c4-105">List signIns</span></span>

<span data-ttu-id="2e0c4-106">Recupera as Azure AD entradas do usuário para seu locatário.</span><span class="sxs-lookup"><span data-stu-id="2e0c4-106">Retrieves the Azure AD user sign-ins for your tenant.</span></span> <span data-ttu-id="2e0c4-107">Entradas que são interativas em natureza (onde uma nome de usuário/senha é passada como parte do token de autorização) e entradas federadas bem-sucedidas atualmente estão incluídas nos logs de entrar.</span><span class="sxs-lookup"><span data-stu-id="2e0c4-107">Sign-ins that are interactive in nature (where a username/password is passed as part of authorization token) and successful federated sign-ins are currently included in the sign-in logs.</span></span>  <span data-ttu-id="2e0c4-108">Os mais recentes signIns são retornados pela primeira vez.</span><span class="sxs-lookup"><span data-stu-id="2e0c4-108">The most recent signIns are returned first.</span></span>


## <a name="permissions"></a><span data-ttu-id="2e0c4-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="2e0c4-109">Permissions</span></span>
<span data-ttu-id="2e0c4-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e0c4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e0c4-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2e0c4-112">Permission type</span></span>      | <span data-ttu-id="2e0c4-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2e0c4-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2e0c4-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2e0c4-114">Delegated (work or school account)</span></span> | <span data-ttu-id="2e0c4-115">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="2e0c4-115">AuditLog.Read.All</span></span> |
|<span data-ttu-id="2e0c4-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2e0c4-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e0c4-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2e0c4-117">Not supported</span></span>   |
|<span data-ttu-id="2e0c4-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2e0c4-118">Application</span></span> | <span data-ttu-id="2e0c4-119">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="2e0c4-119">AuditLog.Read.All</span></span> | 

<span data-ttu-id="2e0c4-120">Além disso, os aplicativos devem ser [registrado corretamente](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) para o Windows Azure AD.</span><span class="sxs-lookup"><span data-stu-id="2e0c4-120">In addition, apps must be [properly registered](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to Azure AD.</span></span>

## <a name="http-request"></a><span data-ttu-id="2e0c4-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2e0c4-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET auditLogs/signIns
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2e0c4-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2e0c4-122">Optional query parameters</span></span>
<span data-ttu-id="2e0c4-123">Este método dá suporte aos seguintes Parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2e0c4-123">This method supports the following OData Query Parameters to help customize the response.</span></span> <span data-ttu-id="2e0c4-124">Verifique [Os parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para como usar esses parâmetros.</span><span class="sxs-lookup"><span data-stu-id="2e0c4-124">Check [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) for how to use these parameters.</span></span>

|<span data-ttu-id="2e0c4-125">Nome</span><span class="sxs-lookup"><span data-stu-id="2e0c4-125">Name</span></span>     |<span data-ttu-id="2e0c4-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e0c4-126">Description</span></span>                            |<span data-ttu-id="2e0c4-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2e0c4-127">Example</span></span>|
|:--------------------|----------------|------------------------------------------------------------------------|
|[<span data-ttu-id="2e0c4-128">$filter</span><span class="sxs-lookup"><span data-stu-id="2e0c4-128">$filter</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#filter-parameter)|<span data-ttu-id="2e0c4-129">Filtra os resultados (linhas).</span><span class="sxs-lookup"><span data-stu-id="2e0c4-129">Filters results (rows).</span></span> |`/auditLogs/signIns?&$filter=createdDateTime le 2018-01-24`
|[<span data-ttu-id="2e0c4-130">$top</span><span class="sxs-lookup"><span data-stu-id="2e0c4-130">$top</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top-parameter)|<span data-ttu-id="2e0c4-131">Define o tamanho de página de resultados.</span><span class="sxs-lookup"><span data-stu-id="2e0c4-131">Sets the page size of results.</span></span>|`/auditLogs/signIns?$top=1`|
|[<span data-ttu-id="2e0c4-132">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="2e0c4-132">$skiptoken</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skiptoken-parameter)|<span data-ttu-id="2e0c4-133">Recupera que a próxima página de resultados do resultado define que ocupar várias páginas.</span><span class="sxs-lookup"><span data-stu-id="2e0c4-133">Retrieves the next page of results from result sets that span multiple pages.</span></span>|`/auditLogs/signIns?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1`|

### <a name="list-of-attributes-supported-by-filter-parameter"></a><span data-ttu-id="2e0c4-134">Lista de atributos suportados pelo parâmetro $filter</span><span class="sxs-lookup"><span data-stu-id="2e0c4-134">List of attributes supported by $filter parameter</span></span>
|<span data-ttu-id="2e0c4-135">Nome do atributo</span><span class="sxs-lookup"><span data-stu-id="2e0c4-135">Attribute Name</span></span> |<span data-ttu-id="2e0c4-136">Operadores com suporte</span><span class="sxs-lookup"><span data-stu-id="2e0c4-136">Supported operators</span></span>|
|:----------------|:------|
|<span data-ttu-id="2e0c4-137">id</span><span class="sxs-lookup"><span data-stu-id="2e0c4-137">id</span></span>|<span data-ttu-id="2e0c4-138">eq</span><span class="sxs-lookup"><span data-stu-id="2e0c4-138">eq</span></span>|
|<span data-ttu-id="2e0c4-139">userId</span><span class="sxs-lookup"><span data-stu-id="2e0c4-139">userId</span></span>|<span data-ttu-id="2e0c4-140">eq</span><span class="sxs-lookup"><span data-stu-id="2e0c4-140">eq</span></span>|
|<span data-ttu-id="2e0c4-141">appId</span><span class="sxs-lookup"><span data-stu-id="2e0c4-141">appId</span></span>|<span data-ttu-id="2e0c4-142">eq</span><span class="sxs-lookup"><span data-stu-id="2e0c4-142">eq</span></span>|
|<span data-ttu-id="2e0c4-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2e0c4-143">createdDateTime</span></span>| <span data-ttu-id="2e0c4-144">EQ, le, ge</span><span class="sxs-lookup"><span data-stu-id="2e0c4-144">eq, le, ge</span></span>|
|<span data-ttu-id="2e0c4-145">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="2e0c4-145">userDisplayName</span></span>| <span data-ttu-id="2e0c4-146">EQ, startswith</span><span class="sxs-lookup"><span data-stu-id="2e0c4-146">eq, startswith</span></span>|
|<span data-ttu-id="2e0c4-147">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2e0c4-147">userPrincipalName</span></span>| <span data-ttu-id="2e0c4-148">EQ, startswith</span><span class="sxs-lookup"><span data-stu-id="2e0c4-148">eq, startswith</span></span>|
|<span data-ttu-id="2e0c4-149">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="2e0c4-149">appDisplayName</span></span>| <span data-ttu-id="2e0c4-150">EQ, startswith</span><span class="sxs-lookup"><span data-stu-id="2e0c4-150">eq, startswith</span></span>|
|<span data-ttu-id="2e0c4-151">ipAddress</span><span class="sxs-lookup"><span data-stu-id="2e0c4-151">ipAddress</span></span>| <span data-ttu-id="2e0c4-152">EQ, startswith</span><span class="sxs-lookup"><span data-stu-id="2e0c4-152">eq, startswith</span></span>|
|<span data-ttu-id="2e0c4-153">Cidade do local</span><span class="sxs-lookup"><span data-stu-id="2e0c4-153">location/city</span></span>| <span data-ttu-id="2e0c4-154">EQ, startswith</span><span class="sxs-lookup"><span data-stu-id="2e0c4-154">eq, startswith</span></span>|
|<span data-ttu-id="2e0c4-155">local/estado</span><span class="sxs-lookup"><span data-stu-id="2e0c4-155">location/state</span></span>| <span data-ttu-id="2e0c4-156">EQ, startswith</span><span class="sxs-lookup"><span data-stu-id="2e0c4-156">eq, startswith</span></span>|
|<span data-ttu-id="2e0c4-157">local/countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="2e0c4-157">location/countryOrRegion</span></span>| <span data-ttu-id="2e0c4-158">EQ, startswith</span><span class="sxs-lookup"><span data-stu-id="2e0c4-158">eq, startswith</span></span>|
|<span data-ttu-id="2e0c4-159">status/errorCode</span><span class="sxs-lookup"><span data-stu-id="2e0c4-159">status/errorCode</span></span>|<span data-ttu-id="2e0c4-160">eq</span><span class="sxs-lookup"><span data-stu-id="2e0c4-160">eq</span></span>|
|<span data-ttu-id="2e0c4-161">id/de usuário de initiatedBy</span><span class="sxs-lookup"><span data-stu-id="2e0c4-161">initiatedBy/user/id</span></span>|<span data-ttu-id="2e0c4-162">eq</span><span class="sxs-lookup"><span data-stu-id="2e0c4-162">eq</span></span>|
|<span data-ttu-id="2e0c4-163">displayName/de usuário de initiatedBy</span><span class="sxs-lookup"><span data-stu-id="2e0c4-163">initiatedBy/user/displayName</span></span>| <span data-ttu-id="2e0c4-164">eq</span><span class="sxs-lookup"><span data-stu-id="2e0c4-164">eq</span></span>|
|<span data-ttu-id="2e0c4-165">initiatedBy/usuário/userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2e0c4-165">initiatedBy/user/userPrincipalName</span></span>| <span data-ttu-id="2e0c4-166">EQ, startswith</span><span class="sxs-lookup"><span data-stu-id="2e0c4-166">eq, startswith</span></span>|
|<span data-ttu-id="2e0c4-167">clientAppUsed</span><span class="sxs-lookup"><span data-stu-id="2e0c4-167">clientAppUsed</span></span>| <span data-ttu-id="2e0c4-168">eq</span><span class="sxs-lookup"><span data-stu-id="2e0c4-168">eq</span></span>|
|<span data-ttu-id="2e0c4-169">conditionalAccessStatus</span><span class="sxs-lookup"><span data-stu-id="2e0c4-169">conditionalAccessStatus</span></span> | <span data-ttu-id="2e0c4-170">eq</span><span class="sxs-lookup"><span data-stu-id="2e0c4-170">eq</span></span>|
|<span data-ttu-id="2e0c4-171">deviceDetail/navegador</span><span class="sxs-lookup"><span data-stu-id="2e0c4-171">deviceDetail/browser</span></span>| <span data-ttu-id="2e0c4-172">EQ, startswith</span><span class="sxs-lookup"><span data-stu-id="2e0c4-172">eq, startswith</span></span>|
|<span data-ttu-id="2e0c4-173">deviceDetail/operatingSystem</span><span class="sxs-lookup"><span data-stu-id="2e0c4-173">deviceDetail/operatingSystem</span></span>| <span data-ttu-id="2e0c4-174">EQ, startswith</span><span class="sxs-lookup"><span data-stu-id="2e0c4-174">eq, startswith</span></span>|
|<span data-ttu-id="2e0c4-175">correlationId</span><span class="sxs-lookup"><span data-stu-id="2e0c4-175">correlationId</span></span>| <span data-ttu-id="2e0c4-176">eq</span><span class="sxs-lookup"><span data-stu-id="2e0c4-176">eq</span></span>|
|<span data-ttu-id="2e0c4-177">riskDetail</span><span class="sxs-lookup"><span data-stu-id="2e0c4-177">riskDetail</span></span>| <span data-ttu-id="2e0c4-178">eq</span><span class="sxs-lookup"><span data-stu-id="2e0c4-178">eq</span></span>|
|<span data-ttu-id="2e0c4-179">riskLevelAggregated</span><span class="sxs-lookup"><span data-stu-id="2e0c4-179">riskLevelAggregated</span></span>| <span data-ttu-id="2e0c4-180">eq</span><span class="sxs-lookup"><span data-stu-id="2e0c4-180">eq</span></span>|
|<span data-ttu-id="2e0c4-181">riskLevelDuringSignIn</span><span class="sxs-lookup"><span data-stu-id="2e0c4-181">riskLevelDuringSignIn</span></span>| <span data-ttu-id="2e0c4-182">eq</span><span class="sxs-lookup"><span data-stu-id="2e0c4-182">eq</span></span>|
|<span data-ttu-id="2e0c4-183">riskEventTypes</span><span class="sxs-lookup"><span data-stu-id="2e0c4-183">riskEventTypes</span></span>| <span data-ttu-id="2e0c4-184">eq</span><span class="sxs-lookup"><span data-stu-id="2e0c4-184">eq</span></span>|
|<span data-ttu-id="2e0c4-185">riskState</span><span class="sxs-lookup"><span data-stu-id="2e0c4-185">riskState</span></span>| <span data-ttu-id="2e0c4-186">eq</span><span class="sxs-lookup"><span data-stu-id="2e0c4-186">eq</span></span>|
|<span data-ttu-id="2e0c4-187">originalRequestId</span><span class="sxs-lookup"><span data-stu-id="2e0c4-187">originalRequestId</span></span>| <span data-ttu-id="2e0c4-188">eq</span><span class="sxs-lookup"><span data-stu-id="2e0c4-188">eq</span></span>|
|<span data-ttu-id="2e0c4-189">tokenIssuerName</span><span class="sxs-lookup"><span data-stu-id="2e0c4-189">tokenIssuerName</span></span>| <span data-ttu-id="2e0c4-190">eq</span><span class="sxs-lookup"><span data-stu-id="2e0c4-190">eq</span></span>|
|<span data-ttu-id="2e0c4-191">tokenIssuerType</span><span class="sxs-lookup"><span data-stu-id="2e0c4-191">tokenIssuerType</span></span>| <span data-ttu-id="2e0c4-192">eq</span><span class="sxs-lookup"><span data-stu-id="2e0c4-192">eq</span></span>|
|<span data-ttu-id="2e0c4-193">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="2e0c4-193">resourceDisplayName</span></span>| <span data-ttu-id="2e0c4-194">eq</span><span class="sxs-lookup"><span data-stu-id="2e0c4-194">eq</span></span>|
|<span data-ttu-id="2e0c4-195">resourceId</span><span class="sxs-lookup"><span data-stu-id="2e0c4-195">resourceId</span></span>| <span data-ttu-id="2e0c4-196">eq</span><span class="sxs-lookup"><span data-stu-id="2e0c4-196">eq</span></span>|


## <a name="response"></a><span data-ttu-id="2e0c4-197">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e0c4-197">Response</span></span>
<span data-ttu-id="2e0c4-198">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos de [entrar](../resources/signin.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2e0c4-198">If successful, this method returns a `200 OK` response code and collection of [signIn](../resources/signin.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2e0c4-199">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2e0c4-199">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2e0c4-200">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2e0c4-200">Request</span></span>
<span data-ttu-id="2e0c4-201">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2e0c4-201">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_signins"
}-->
```http
GET https://graph.microsoft.com/beta/auditLogs/signIns
```
##### <a name="response"></a><span data-ttu-id="2e0c4-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e0c4-202">Response</span></span>
<span data-ttu-id="2e0c4-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2e0c4-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.signIn",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 264
```
```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/signIns",
    "value": [{
        "id":"b01b1726-0147-425e-a7f7-21f252050400",
        "createdDateTime":"2018-11-06T18:48:33.8527147Z",
        "userDisplayName":"Jon Doe",
         "userPrincipalName":"admin@aad171.ccsctp.net",
         "userId":"d7cc485d-2c1b-422c-98fd-5ce52859a4a3",
        "appId":"c44b4083-3bb0-49c1-b47d-974e53cbdf3c",
         "appDisplayName":"Azure Portal",
         "ipAddress":"207.254.19.10",
         "clientAppUsed":"Browser",
        "mfaDetail":null,
         "correlationId":"65dd87ce-2183-419e-81a9-d6e20379bcc2",
         "conditionalAccessStatus":"notApplied",
        "originalRequestId":null,
        "isInteractive":true,
        "tokenIssuerName":null,
        "tokenIssuerType":"AzureAD",
        "processingTimeInMilliseconds":0,
        "riskDetail":"none",
        "riskLevelAggregated":"none",
        "riskLevelDuringSignIn":"none",
        "riskState":"none",
        "riskEventTypes":[

        ],
        "resourceDisplayName":"windows azure service management api",
        "resourceId":"797f4846-ba00-4fd7-ba43-dac1f8f63013",
        "authenticationMethodsUsed":[

        ],
        "status":{
            "errorCode":50140,
            "failureReason":"This error occurred due to 'Keep me signed in' interrupt when the user was signing-in.",
            "additionalDetails":null
        },
        "deviceDetail":{
            "deviceId":null,
            "displayName":null,
            "operatingSystem":"Windows 7",
            "browser":"Chrome 63.0.3239",
            "isCompliant":null,
            "isManaged":null,
            "trustType":null
        },
        "location":{
            "city":"Lithia Springs",
            "state":"Georgia",
            "countryOrRegion":"US",
            "geoCoordinates":{
                "altitude":null,
                "latitude":33.7930908203125,
                "longitude":-84.445358276367188
            }
        },
        "appliedConditionalAccessPolicies":[
            {
            "id":"6551c58c-e5da-4036-a6ea-c2c3fad264f1",
            "displayName":"New Name here4",
            "enforcedGrantControls":[
                "Mfa",
                "RequireCompliantDevice"
            ],
            "enforcedSessionControls":[

            ],
            "result":"notApplied"
            },
            {
            "id":"b645a140-20fe-4ce0-a724-18ab201e9026",
            "displayName":"PipelineTest4",
            "enforcedGrantControls":[

            ],
            "enforcedSessionControls":[

            ],
            "result":"notEnabled"
            }
        ],
        "authenticationProcessingDetails":[

        ],
        "networkLocationDetails":[

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
  "tocPath": ""
}-->
