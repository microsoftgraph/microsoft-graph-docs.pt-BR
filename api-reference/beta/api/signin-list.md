---
title: Listar logons
description: Recupera as entradas de usuário do Azure AD usuário para seu locatário. Entradas que são interativas na natureza (onde um nome de usuário/senha é passado como parte de símbolo de autorização) e entradas federadas bem-sucedida atualmente estão incluídas nos logs de entrada.  Os logons mais recentes são retornados primeiro.
localization_priority: Priority
ms.openlocfilehash: 8596bd168a3e10cbea9e15e2f61d6bd668fd27b5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32545154"
---
# <a name="list-signins"></a><span data-ttu-id="c04a9-105">Listar logons</span><span class="sxs-lookup"><span data-stu-id="c04a9-105">List sign-ins</span></span>

<span data-ttu-id="c04a9-106">Recupera as entradas de usuário do Azure AD usuário para seu locatário.</span><span class="sxs-lookup"><span data-stu-id="c04a9-106">Retrieves the Azure AD user sign-ins for your tenant.</span></span> <span data-ttu-id="c04a9-107">Entradas que são interativas na natureza (onde um nome de usuário/senha é passado como parte de símbolo de autorização) e entradas federadas bem-sucedida atualmente estão incluídas nos logs de entrada.</span><span class="sxs-lookup"><span data-stu-id="c04a9-107">Sign-ins that are interactive in nature (where a username/password is passed as part of authorization token) and successful federated sign-ins are currently included in the sign-in logs.</span></span>  <span data-ttu-id="c04a9-108">Os logons mais recentes são retornados primeiro.</span><span class="sxs-lookup"><span data-stu-id="c04a9-108">The most recent signIns are returned first.</span></span>


## <a name="permissions"></a><span data-ttu-id="c04a9-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="c04a9-109">Permissions</span></span>
<span data-ttu-id="c04a9-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c04a9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c04a9-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c04a9-112">Permission type</span></span>      | <span data-ttu-id="c04a9-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c04a9-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c04a9-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c04a9-114">Delegated (work or school account)</span></span> | <span data-ttu-id="c04a9-115">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="c04a9-115">AuditLog.Read.All</span></span> |
|<span data-ttu-id="c04a9-116">Delegado (conta pessoal da conta Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c04a9-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c04a9-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="c04a9-117">Not supported</span></span>   |
|<span data-ttu-id="c04a9-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c04a9-118">Application</span></span> | <span data-ttu-id="c04a9-119">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="c04a9-119">AuditLog.Read.All</span></span> | 

<span data-ttu-id="c04a9-120">Além disso, os aplicativos devem ser [corretamente registrados](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c04a9-120">In addition, apps must be [properly registered](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to Azure AD.</span></span>

## <a name="http-request"></a><span data-ttu-id="c04a9-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c04a9-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET auditLogs/signIns
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c04a9-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c04a9-122">Optional query parameters</span></span>
<span data-ttu-id="c04a9-123">Este método dá suporte aos seguintes Parâmetros de Consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c04a9-123">This method supports the following OData Query Parameters to help customize the response.</span></span> <span data-ttu-id="c04a9-124">Verifique [Parâmetros de Consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para saber como usar esses parâmetros.</span><span class="sxs-lookup"><span data-stu-id="c04a9-124">Check [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) for how to use these parameters.</span></span>

|<span data-ttu-id="c04a9-125">Nome</span><span class="sxs-lookup"><span data-stu-id="c04a9-125">Name</span></span>     |<span data-ttu-id="c04a9-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="c04a9-126">Description</span></span>                            |<span data-ttu-id="c04a9-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c04a9-127">Example</span></span>|
|:--------------------|----------------|------------------------------------------------------------------------|
|[<span data-ttu-id="c04a9-128">$filter</span><span class="sxs-lookup"><span data-stu-id="c04a9-128">$filter</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#filter-parameter)|<span data-ttu-id="c04a9-129">Filtra os resultados (linhas).</span><span class="sxs-lookup"><span data-stu-id="c04a9-129">Filters results (rows).</span></span> |`/auditLogs/signIns?&$filter=createdDateTime le 2018-01-24`
|[<span data-ttu-id="c04a9-130">$top</span><span class="sxs-lookup"><span data-stu-id="c04a9-130">$top</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top-parameter)|<span data-ttu-id="c04a9-131">Define o tamanho de página de resultados.</span><span class="sxs-lookup"><span data-stu-id="c04a9-131">Sets the page size of results.</span></span>|`/auditLogs/signIns?$top=1`|
|[<span data-ttu-id="c04a9-132">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="c04a9-132">$skiptoken</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skiptoken-parameter)|<span data-ttu-id="c04a9-133">Recupera a próxima página de resultados de conjuntos de resultados que abrangem várias páginas.</span><span class="sxs-lookup"><span data-stu-id="c04a9-133">Retrieves the next page of results from result sets that span multiple pages.</span></span>|`/auditLogs/signIns?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1`|

### <a name="list-of-attributes-supported-by-filter-parameter"></a><span data-ttu-id="c04a9-134">Lista de atributos com suporte parâmetro $filter</span><span class="sxs-lookup"><span data-stu-id="c04a9-134">List of attributes supported by $filter parameter</span></span>
|<span data-ttu-id="c04a9-135">Nome do Atributo</span><span class="sxs-lookup"><span data-stu-id="c04a9-135">Attribute Name</span></span> |<span data-ttu-id="c04a9-136">Operadores com suporte</span><span class="sxs-lookup"><span data-stu-id="c04a9-136">Supported operators</span></span>|
|:----------------|:------|
|<span data-ttu-id="c04a9-137">id</span><span class="sxs-lookup"><span data-stu-id="c04a9-137">id</span></span>|<span data-ttu-id="c04a9-138">eq</span><span class="sxs-lookup"><span data-stu-id="c04a9-138">eq</span></span>|
|<span data-ttu-id="c04a9-139">userId</span><span class="sxs-lookup"><span data-stu-id="c04a9-139">userId</span></span>|<span data-ttu-id="c04a9-140">eq</span><span class="sxs-lookup"><span data-stu-id="c04a9-140">eq</span></span>|
|<span data-ttu-id="c04a9-141">appId</span><span class="sxs-lookup"><span data-stu-id="c04a9-141">appId</span></span>|<span data-ttu-id="c04a9-142">eq</span><span class="sxs-lookup"><span data-stu-id="c04a9-142">eq</span></span>|
|<span data-ttu-id="c04a9-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c04a9-143">createdDateTime</span></span>| <span data-ttu-id="c04a9-144">eq, le, ge</span><span class="sxs-lookup"><span data-stu-id="c04a9-144">eq, ge, le</span></span>|
|<span data-ttu-id="c04a9-145">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="c04a9-145">userDisplayName</span></span>| <span data-ttu-id="c04a9-146">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="c04a9-146">eq, startswith</span></span>|
|<span data-ttu-id="c04a9-147">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c04a9-147">userPrincipalName</span></span>| <span data-ttu-id="c04a9-148">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="c04a9-148">eq, startswith</span></span>|
|<span data-ttu-id="c04a9-149">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="c04a9-149">appDisplayName</span></span>| <span data-ttu-id="c04a9-150">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="c04a9-150">eq, startswith</span></span>|
|<span data-ttu-id="c04a9-151">ipAddress</span><span class="sxs-lookup"><span data-stu-id="c04a9-151">ipAddress</span></span>| <span data-ttu-id="c04a9-152">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="c04a9-152">eq, startswith</span></span>|
|<span data-ttu-id="c04a9-153">localização/cidade</span><span class="sxs-lookup"><span data-stu-id="c04a9-153">location/city</span></span>| <span data-ttu-id="c04a9-154">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="c04a9-154">eq, startswith</span></span>|
|<span data-ttu-id="c04a9-155">localização/estado</span><span class="sxs-lookup"><span data-stu-id="c04a9-155">location/state</span></span>| <span data-ttu-id="c04a9-156">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="c04a9-156">eq, startswith</span></span>|
|<span data-ttu-id="c04a9-157">location/countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="c04a9-157">location/countryOrRegion</span></span>| <span data-ttu-id="c04a9-158">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="c04a9-158">eq, startswith</span></span>|
|<span data-ttu-id="c04a9-159">status/errorCode</span><span class="sxs-lookup"><span data-stu-id="c04a9-159">status/errorCode</span></span>|<span data-ttu-id="c04a9-160">eq</span><span class="sxs-lookup"><span data-stu-id="c04a9-160">eq</span></span>|
|<span data-ttu-id="c04a9-161">initiatedBy/user/id</span><span class="sxs-lookup"><span data-stu-id="c04a9-161">initiatedBy/user/id</span></span>|<span data-ttu-id="c04a9-162">eq</span><span class="sxs-lookup"><span data-stu-id="c04a9-162">eq</span></span>|
|<span data-ttu-id="c04a9-163">initiatedBy/user/displayName</span><span class="sxs-lookup"><span data-stu-id="c04a9-163">initiatedBy/user/displayName</span></span>| <span data-ttu-id="c04a9-164">eq</span><span class="sxs-lookup"><span data-stu-id="c04a9-164">eq</span></span>|
|<span data-ttu-id="c04a9-165">initiatedBy/user/userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c04a9-165">initiatedBy/user/userPrincipalName</span></span>| <span data-ttu-id="c04a9-166">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="c04a9-166">eq, startswith</span></span>|
|<span data-ttu-id="c04a9-167">clientAppUsed</span><span class="sxs-lookup"><span data-stu-id="c04a9-167">clientAppUsed</span></span>| <span data-ttu-id="c04a9-168">eq</span><span class="sxs-lookup"><span data-stu-id="c04a9-168">eq</span></span>|
|<span data-ttu-id="c04a9-169">conditionalAccessStatus</span><span class="sxs-lookup"><span data-stu-id="c04a9-169">conditionalAccessStatus</span></span> | <span data-ttu-id="c04a9-170">eq</span><span class="sxs-lookup"><span data-stu-id="c04a9-170">eq</span></span>|
|<span data-ttu-id="c04a9-171">deviceDetail/browser</span><span class="sxs-lookup"><span data-stu-id="c04a9-171">deviceDetail/browser</span></span>| <span data-ttu-id="c04a9-172">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="c04a9-172">eq, startswith</span></span>|
|<span data-ttu-id="c04a9-173">deviceDetail/operatingSystem</span><span class="sxs-lookup"><span data-stu-id="c04a9-173">deviceDetail/operatingSystem</span></span>| <span data-ttu-id="c04a9-174">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="c04a9-174">eq, startswith</span></span>|
|<span data-ttu-id="c04a9-175">correlationId</span><span class="sxs-lookup"><span data-stu-id="c04a9-175">correlationId</span></span>| <span data-ttu-id="c04a9-176">eq</span><span class="sxs-lookup"><span data-stu-id="c04a9-176">eq</span></span>|
|<span data-ttu-id="c04a9-177">riskDetail</span><span class="sxs-lookup"><span data-stu-id="c04a9-177">riskDetail</span></span>| <span data-ttu-id="c04a9-178">eq</span><span class="sxs-lookup"><span data-stu-id="c04a9-178">eq</span></span>|
|<span data-ttu-id="c04a9-179">riskLevelAggregated</span><span class="sxs-lookup"><span data-stu-id="c04a9-179">riskLevelAggregated</span></span>| <span data-ttu-id="c04a9-180">eq</span><span class="sxs-lookup"><span data-stu-id="c04a9-180">eq</span></span>|
|<span data-ttu-id="c04a9-181">riskLevelDuringSignIn</span><span class="sxs-lookup"><span data-stu-id="c04a9-181">riskLevelDuringSignIn</span></span>| <span data-ttu-id="c04a9-182">eq</span><span class="sxs-lookup"><span data-stu-id="c04a9-182">eq</span></span>|
|<span data-ttu-id="c04a9-183">riskEventTypes</span><span class="sxs-lookup"><span data-stu-id="c04a9-183">riskEventTypes</span></span>| <span data-ttu-id="c04a9-184">eq</span><span class="sxs-lookup"><span data-stu-id="c04a9-184">eq</span></span>|
|<span data-ttu-id="c04a9-185">riskState</span><span class="sxs-lookup"><span data-stu-id="c04a9-185">riskState</span></span>| <span data-ttu-id="c04a9-186">eq</span><span class="sxs-lookup"><span data-stu-id="c04a9-186">eq</span></span>|
|<span data-ttu-id="c04a9-187">originalRequestId</span><span class="sxs-lookup"><span data-stu-id="c04a9-187">originalRequestId</span></span>| <span data-ttu-id="c04a9-188">eq</span><span class="sxs-lookup"><span data-stu-id="c04a9-188">eq</span></span>|
|<span data-ttu-id="c04a9-189">tokenIssuerName</span><span class="sxs-lookup"><span data-stu-id="c04a9-189">tokenIssuerName</span></span>| <span data-ttu-id="c04a9-190">eq</span><span class="sxs-lookup"><span data-stu-id="c04a9-190">eq</span></span>|
|<span data-ttu-id="c04a9-191">tokenIssuerType</span><span class="sxs-lookup"><span data-stu-id="c04a9-191">tokenIssuerType</span></span>| <span data-ttu-id="c04a9-192">eq</span><span class="sxs-lookup"><span data-stu-id="c04a9-192">eq</span></span>|
|<span data-ttu-id="c04a9-193">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="c04a9-193">resourceDisplayName</span></span>| <span data-ttu-id="c04a9-194">eq</span><span class="sxs-lookup"><span data-stu-id="c04a9-194">eq</span></span>|
|<span data-ttu-id="c04a9-195">resourceId</span><span class="sxs-lookup"><span data-stu-id="c04a9-195">resourceId</span></span>| <span data-ttu-id="c04a9-196">eq</span><span class="sxs-lookup"><span data-stu-id="c04a9-196">eq</span></span>|


## <a name="response"></a><span data-ttu-id="c04a9-197">Resposta</span><span class="sxs-lookup"><span data-stu-id="c04a9-197">Response</span></span>
<span data-ttu-id="c04a9-198">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos de [logon](../resources/signin.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c04a9-198">If successful, this method returns a `200 OK` response code and collection of [directoryAudit](../resources/signin.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c04a9-199">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c04a9-199">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c04a9-200">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c04a9-200">Request</span></span>
<span data-ttu-id="c04a9-201">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c04a9-201">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_signins"
}-->
```http
GET https://graph.microsoft.com/beta/auditLogs/signIns
```
##### <a name="response"></a><span data-ttu-id="c04a9-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="c04a9-202">Response</span></span>
<span data-ttu-id="c04a9-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c04a9-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
