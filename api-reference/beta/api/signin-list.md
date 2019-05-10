---
title: Listar logons
description: Descreve o método de lista o recurso de logon (entidade) do Microsoft Graph API (REST), que ajuda a auditoria das atividades de diretório (locatário) (versão beta).
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fdb1358d36a0e1da34779de5505c5f18f901e681
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638677"
---
# <a name="list-signins"></a><span data-ttu-id="2b544-103">Listar logons</span><span class="sxs-lookup"><span data-stu-id="2b544-103">List signIns</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b544-104">Recupera os logons de usuário do Azure AD para seu locatário.</span><span class="sxs-lookup"><span data-stu-id="2b544-104">Retrieves the Azure AD user sign-ins for your tenant.</span></span> <span data-ttu-id="2b544-105">Entradas que são interativas na natureza (onde um nome de usuário/senha é passado como parte de símbolo de autorização) e entradas federadas bem-sucedida atualmente estão incluídas nos logs de entrada.</span><span class="sxs-lookup"><span data-stu-id="2b544-105">Sign-ins that are interactive in nature (where a username/password is passed as part of authorization token) and successful federated sign-ins are currently included in the sign-in logs.</span></span>  <span data-ttu-id="2b544-106">Os logons mais recentes são retornados primeiro.</span><span class="sxs-lookup"><span data-stu-id="2b544-106">The most recent signIns are returned first.</span></span>

## <a name="permissions"></a><span data-ttu-id="2b544-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="2b544-107">Permissions</span></span>

<span data-ttu-id="2b544-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b544-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b544-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2b544-110">Permission type</span></span>      | <span data-ttu-id="2b544-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2b544-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b544-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2b544-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2b544-113">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b544-113">AuditLog.Read.All</span></span> |
|<span data-ttu-id="2b544-114">Delegado (conta pessoal da conta Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2b544-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b544-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2b544-115">Not supported</span></span>   |
|<span data-ttu-id="2b544-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2b544-116">Application</span></span> | <span data-ttu-id="2b544-117">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b544-117">AuditLog.Read.All</span></span> | 

<span data-ttu-id="2b544-118">Além disso, os aplicativos devem ser [corretamente registrados](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="2b544-118">In addition, apps must be [properly registered](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to Azure AD.</span></span>

## <a name="http-request"></a><span data-ttu-id="2b544-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2b544-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET auditLogs/signIns
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2b544-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2b544-120">Optional query parameters</span></span>
<span data-ttu-id="2b544-121">Este método dá suporte aos seguintes Parâmetros de Consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2b544-121">This method supports the following OData Query Parameters to help customize the response.</span></span> <span data-ttu-id="2b544-122">Para obter detalhes sobre como usar esses parâmetros, confira [Parâmetros de consulta do OData](/graph/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="2b544-122">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

|<span data-ttu-id="2b544-123">Nome</span><span class="sxs-lookup"><span data-stu-id="2b544-123">Name</span></span>     |<span data-ttu-id="2b544-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b544-124">Description</span></span>                            |<span data-ttu-id="2b544-125">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2b544-125">Example</span></span>|
|:--------------------|----------------|------------------------------------------------------------------------|
|[<span data-ttu-id="2b544-126">$filter</span><span class="sxs-lookup"><span data-stu-id="2b544-126">$filter</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#filter-parameter)|<span data-ttu-id="2b544-127">Filtra os resultados (linhas).</span><span class="sxs-lookup"><span data-stu-id="2b544-127">Filters results (rows).</span></span> |`/auditLogs/signIns?&$filter=createdDateTime le 2018-01-24`
|[<span data-ttu-id="2b544-128">$top</span><span class="sxs-lookup"><span data-stu-id="2b544-128">$top</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top-parameter)|<span data-ttu-id="2b544-129">Define o tamanho de página de resultados.</span><span class="sxs-lookup"><span data-stu-id="2b544-129">Sets the page size of results.</span></span>|`/auditLogs/signIns?$top=1`|
|[<span data-ttu-id="2b544-130">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="2b544-130">$skiptoken</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skiptoken-parameter)|<span data-ttu-id="2b544-131">Recupera a próxima página de resultados de conjuntos de resultados que abrangem várias páginas.</span><span class="sxs-lookup"><span data-stu-id="2b544-131">Retrieves the next page of results from result sets that span multiple pages.</span></span>|`/auditLogs/signIns?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1`|

### <a name="list-of-attributes-supported-by-filter-parameter"></a><span data-ttu-id="2b544-132">Lista de atributos com suporte parâmetro $filter</span><span class="sxs-lookup"><span data-stu-id="2b544-132">List of attributes supported by $filter parameter</span></span>
|<span data-ttu-id="2b544-133">Nome do Atributo</span><span class="sxs-lookup"><span data-stu-id="2b544-133">Attribute Name</span></span> |<span data-ttu-id="2b544-134">Operadores com suporte</span><span class="sxs-lookup"><span data-stu-id="2b544-134">Supported operators</span></span>|
|:----------------|:------|
|<span data-ttu-id="2b544-135">id</span><span class="sxs-lookup"><span data-stu-id="2b544-135">id</span></span>|<span data-ttu-id="2b544-136">eq</span><span class="sxs-lookup"><span data-stu-id="2b544-136">eq</span></span>|
|<span data-ttu-id="2b544-137">userId</span><span class="sxs-lookup"><span data-stu-id="2b544-137">userId</span></span>|<span data-ttu-id="2b544-138">eq</span><span class="sxs-lookup"><span data-stu-id="2b544-138">eq</span></span>|
|<span data-ttu-id="2b544-139">appId</span><span class="sxs-lookup"><span data-stu-id="2b544-139">appId</span></span>|<span data-ttu-id="2b544-140">eq</span><span class="sxs-lookup"><span data-stu-id="2b544-140">eq</span></span>|
|<span data-ttu-id="2b544-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2b544-141">createdDateTime</span></span>| <span data-ttu-id="2b544-142">eq, le, ge</span><span class="sxs-lookup"><span data-stu-id="2b544-142">eq, le, ge</span></span>|
|<span data-ttu-id="2b544-143">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="2b544-143">userDisplayName</span></span>| <span data-ttu-id="2b544-144">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="2b544-144">eq, startswith</span></span>|
|<span data-ttu-id="2b544-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2b544-145">userPrincipalName</span></span>| <span data-ttu-id="2b544-146">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="2b544-146">eq, startswith</span></span>|
|<span data-ttu-id="2b544-147">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="2b544-147">appDisplayName</span></span>| <span data-ttu-id="2b544-148">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="2b544-148">eq, startswith</span></span>|
|<span data-ttu-id="2b544-149">ipAddress</span><span class="sxs-lookup"><span data-stu-id="2b544-149">ipAddress</span></span>| <span data-ttu-id="2b544-150">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="2b544-150">eq, startswith</span></span>|
|<span data-ttu-id="2b544-151">localização/cidade</span><span class="sxs-lookup"><span data-stu-id="2b544-151">location/city</span></span>| <span data-ttu-id="2b544-152">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="2b544-152">eq, startswith</span></span>|
|<span data-ttu-id="2b544-153">localização/estado</span><span class="sxs-lookup"><span data-stu-id="2b544-153">location/state</span></span>| <span data-ttu-id="2b544-154">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="2b544-154">eq, startswith</span></span>|
|<span data-ttu-id="2b544-155">location/countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="2b544-155">location/countryOrRegion</span></span>| <span data-ttu-id="2b544-156">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="2b544-156">eq, startswith</span></span>|
|<span data-ttu-id="2b544-157">status/errorCode</span><span class="sxs-lookup"><span data-stu-id="2b544-157">status/errorCode</span></span>|<span data-ttu-id="2b544-158">eq</span><span class="sxs-lookup"><span data-stu-id="2b544-158">eq</span></span>|
|<span data-ttu-id="2b544-159">initiatedBy/user/id</span><span class="sxs-lookup"><span data-stu-id="2b544-159">initiatedBy/user/id</span></span>|<span data-ttu-id="2b544-160">eq</span><span class="sxs-lookup"><span data-stu-id="2b544-160">eq</span></span>|
|<span data-ttu-id="2b544-161">initiatedBy/user/displayName</span><span class="sxs-lookup"><span data-stu-id="2b544-161">initiatedBy/user/displayName</span></span>| <span data-ttu-id="2b544-162">eq</span><span class="sxs-lookup"><span data-stu-id="2b544-162">eq</span></span>|
|<span data-ttu-id="2b544-163">initiatedBy/user/userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2b544-163">initiatedBy/user/userPrincipalName</span></span>| <span data-ttu-id="2b544-164">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="2b544-164">eq, startswith</span></span>|
|<span data-ttu-id="2b544-165">clientAppUsed</span><span class="sxs-lookup"><span data-stu-id="2b544-165">clientAppUsed</span></span>| <span data-ttu-id="2b544-166">eq</span><span class="sxs-lookup"><span data-stu-id="2b544-166">eq</span></span>|
|<span data-ttu-id="2b544-167">conditionalAccessStatus</span><span class="sxs-lookup"><span data-stu-id="2b544-167">conditionalAccessStatus</span></span> | <span data-ttu-id="2b544-168">eq</span><span class="sxs-lookup"><span data-stu-id="2b544-168">eq</span></span>|
|<span data-ttu-id="2b544-169">deviceDetail/browser</span><span class="sxs-lookup"><span data-stu-id="2b544-169">deviceDetail/browser</span></span>| <span data-ttu-id="2b544-170">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="2b544-170">eq, startswith</span></span>|
|<span data-ttu-id="2b544-171">deviceDetail/operatingSystem</span><span class="sxs-lookup"><span data-stu-id="2b544-171">deviceDetail/operatingSystem</span></span>| <span data-ttu-id="2b544-172">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="2b544-172">eq, startswith</span></span>|
|<span data-ttu-id="2b544-173">correlationId</span><span class="sxs-lookup"><span data-stu-id="2b544-173">correlationId</span></span>| <span data-ttu-id="2b544-174">eq</span><span class="sxs-lookup"><span data-stu-id="2b544-174">eq</span></span>|
|<span data-ttu-id="2b544-175">riskDetail</span><span class="sxs-lookup"><span data-stu-id="2b544-175">riskDetail</span></span>| <span data-ttu-id="2b544-176">eq</span><span class="sxs-lookup"><span data-stu-id="2b544-176">eq</span></span>|
|<span data-ttu-id="2b544-177">riskLevelAggregated</span><span class="sxs-lookup"><span data-stu-id="2b544-177">riskLevelAggregated</span></span>| <span data-ttu-id="2b544-178">eq</span><span class="sxs-lookup"><span data-stu-id="2b544-178">eq</span></span>|
|<span data-ttu-id="2b544-179">riskLevelDuringSignIn</span><span class="sxs-lookup"><span data-stu-id="2b544-179">riskLevelDuringSignIn</span></span>| <span data-ttu-id="2b544-180">eq</span><span class="sxs-lookup"><span data-stu-id="2b544-180">eq</span></span>|
|<span data-ttu-id="2b544-181">riskEventTypes</span><span class="sxs-lookup"><span data-stu-id="2b544-181">riskEventTypes</span></span>| <span data-ttu-id="2b544-182">eq</span><span class="sxs-lookup"><span data-stu-id="2b544-182">eq</span></span>|
|<span data-ttu-id="2b544-183">riskState</span><span class="sxs-lookup"><span data-stu-id="2b544-183">riskState</span></span>| <span data-ttu-id="2b544-184">eq</span><span class="sxs-lookup"><span data-stu-id="2b544-184">eq</span></span>|
|<span data-ttu-id="2b544-185">originalRequestId</span><span class="sxs-lookup"><span data-stu-id="2b544-185">originalRequestId</span></span>| <span data-ttu-id="2b544-186">eq</span><span class="sxs-lookup"><span data-stu-id="2b544-186">eq</span></span>|
|<span data-ttu-id="2b544-187">tokenIssuerName</span><span class="sxs-lookup"><span data-stu-id="2b544-187">tokenIssuerName</span></span>| <span data-ttu-id="2b544-188">eq</span><span class="sxs-lookup"><span data-stu-id="2b544-188">eq</span></span>|
|<span data-ttu-id="2b544-189">tokenIssuerType</span><span class="sxs-lookup"><span data-stu-id="2b544-189">tokenIssuerType</span></span>| <span data-ttu-id="2b544-190">eq</span><span class="sxs-lookup"><span data-stu-id="2b544-190">eq</span></span>|
|<span data-ttu-id="2b544-191">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="2b544-191">resourceDisplayName</span></span>| <span data-ttu-id="2b544-192">eq</span><span class="sxs-lookup"><span data-stu-id="2b544-192">eq</span></span>|
|<span data-ttu-id="2b544-193">resourceId</span><span class="sxs-lookup"><span data-stu-id="2b544-193">resourceId</span></span>| <span data-ttu-id="2b544-194">eq</span><span class="sxs-lookup"><span data-stu-id="2b544-194">eq</span></span>|


## <a name="response"></a><span data-ttu-id="2b544-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b544-195">Response</span></span>
<span data-ttu-id="2b544-196">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos de [logon](../resources/signin.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2b544-196">If successful, this method returns a `200 OK` response code and collection of [signIn](../resources/signin.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2b544-197">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2b544-197">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2b544-198">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2b544-198">Request</span></span>
<span data-ttu-id="2b544-199">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2b544-199">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_signins"
}-->
```http
GET https://graph.microsoft.com/beta/auditLogs/signIns
```
##### <a name="response"></a><span data-ttu-id="2b544-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b544-200">Response</span></span>
<span data-ttu-id="2b544-201">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2b544-201">Here is an example of the response.</span></span> 

><span data-ttu-id="2b544-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2b544-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="2b544-204">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="2b544-204">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="2b544-205">C#</span><span class="sxs-lookup"><span data-stu-id="2b544-205">C</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_signins-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2b544-206">Javascript</span><span class="sxs-lookup"><span data-stu-id="2b544-206">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_signins-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
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
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/signin-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/signin-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
