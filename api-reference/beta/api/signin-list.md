---
title: Listar logons
description: Descreve o método de lista o recurso de logon (entidade) do Microsoft Graph API (REST), que ajuda a auditoria das atividades de diretório (locatário) (versão beta).
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e352a6ede72ef5e6b2b776e9f177680760bed0de
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271628"
---
# <a name="list-signins"></a><span data-ttu-id="8926a-103">Listar logons</span><span class="sxs-lookup"><span data-stu-id="8926a-103">List signIns</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8926a-104">Recupera os logons de usuário do Azure AD para seu locatário.</span><span class="sxs-lookup"><span data-stu-id="8926a-104">Retrieve the Azure AD user sign-ins for your tenant.</span></span> <span data-ttu-id="8926a-105">Entradas que são interativas na natureza (onde um nome de usuário/senha é passado como parte de símbolo de autorização) e entradas federadas bem-sucedida atualmente estão incluídas nos logs de entrada.</span><span class="sxs-lookup"><span data-stu-id="8926a-105">Sign-ins that are interactive in nature (where a username/password is passed as part of authorization token) and successful federated sign-ins are currently included in the sign-in logs.</span></span>  <span data-ttu-id="8926a-106">Os logons mais recentes são retornados primeiro.</span><span class="sxs-lookup"><span data-stu-id="8926a-106">The most recent signIns are returned first.</span></span>

## <a name="permissions"></a><span data-ttu-id="8926a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="8926a-107">Permissions</span></span>

<span data-ttu-id="8926a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8926a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8926a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8926a-110">Permission type</span></span>      | <span data-ttu-id="8926a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8926a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8926a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8926a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8926a-113">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="8926a-113">AuditLog.Read.All</span></span> |
|<span data-ttu-id="8926a-114">Delegado (conta pessoal da conta Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8926a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8926a-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="8926a-115">Not supported</span></span>   |
|<span data-ttu-id="8926a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8926a-116">Application</span></span> | <span data-ttu-id="8926a-117">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="8926a-117">AuditLog.Read.All</span></span> | 

<span data-ttu-id="8926a-118">Além disso, os aplicativos devem ser [corretamente registrados](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8926a-118">In addition, apps must be [properly registered](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to Azure AD.</span></span>

## <a name="http-request"></a><span data-ttu-id="8926a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8926a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET auditLogs/signIns
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8926a-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8926a-120">Optional query parameters</span></span>
<span data-ttu-id="8926a-121">Este método dá suporte aos seguintes Parâmetros de Consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8926a-121">This method supports the following OData Query Parameters to help customize the response.</span></span> <span data-ttu-id="8926a-122">Para obter detalhes sobre como usar esses parâmetros, confira [Parâmetros de consulta do OData](/graph/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="8926a-122">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

|<span data-ttu-id="8926a-123">Nome</span><span class="sxs-lookup"><span data-stu-id="8926a-123">Name</span></span>     |<span data-ttu-id="8926a-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="8926a-124">Description</span></span>                            |<span data-ttu-id="8926a-125">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8926a-125">Example</span></span>|
|:--------------------|----------------|------------------------------------------------------------------------|
|[<span data-ttu-id="8926a-126">$filter</span><span class="sxs-lookup"><span data-stu-id="8926a-126">$filter</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#filter-parameter)|<span data-ttu-id="8926a-127">Filtra os resultados (linhas).</span><span class="sxs-lookup"><span data-stu-id="8926a-127">Filters results (rows).</span></span> |`/auditLogs/signIns?&$filter=createdDateTime le 2018-01-24`
|[<span data-ttu-id="8926a-128">$top</span><span class="sxs-lookup"><span data-stu-id="8926a-128">$top</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top-parameter)|<span data-ttu-id="8926a-129">Define o tamanho de página de resultados.</span><span class="sxs-lookup"><span data-stu-id="8926a-129">Sets the page size of results.</span></span>|`/auditLogs/signIns?$top=1`|
|[<span data-ttu-id="8926a-130">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="8926a-130">$skiptoken</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skiptoken-parameter)|<span data-ttu-id="8926a-131">Recupera a próxima página de resultados de conjuntos de resultados que abrangem várias páginas.</span><span class="sxs-lookup"><span data-stu-id="8926a-131">Retrieves the next page of results from result sets that span multiple pages.</span></span>|`/auditLogs/signIns?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1`|

### <a name="list-of-attributes-supported-by-filter-parameter"></a><span data-ttu-id="8926a-132">Lista de atributos com suporte parâmetro $filter</span><span class="sxs-lookup"><span data-stu-id="8926a-132">List of attributes supported by $filter parameter</span></span>
|<span data-ttu-id="8926a-133">Nome do Atributo</span><span class="sxs-lookup"><span data-stu-id="8926a-133">Attribute Name</span></span> |<span data-ttu-id="8926a-134">Operadores com suporte</span><span class="sxs-lookup"><span data-stu-id="8926a-134">Supported operators</span></span>|
|:----------------|:------|
|<span data-ttu-id="8926a-135">id</span><span class="sxs-lookup"><span data-stu-id="8926a-135">id</span></span>|<span data-ttu-id="8926a-136">eq</span><span class="sxs-lookup"><span data-stu-id="8926a-136">eq</span></span>|
|<span data-ttu-id="8926a-137">userId</span><span class="sxs-lookup"><span data-stu-id="8926a-137">userId</span></span>|<span data-ttu-id="8926a-138">eq</span><span class="sxs-lookup"><span data-stu-id="8926a-138">eq</span></span>|
|<span data-ttu-id="8926a-139">appId</span><span class="sxs-lookup"><span data-stu-id="8926a-139">appId</span></span>|<span data-ttu-id="8926a-140">eq</span><span class="sxs-lookup"><span data-stu-id="8926a-140">eq</span></span>|
|<span data-ttu-id="8926a-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8926a-141">createdDateTime</span></span>| <span data-ttu-id="8926a-142">eq, le, ge</span><span class="sxs-lookup"><span data-stu-id="8926a-142">eq, le, ge</span></span>|
|<span data-ttu-id="8926a-143">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="8926a-143">userDisplayName</span></span>| <span data-ttu-id="8926a-144">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="8926a-144">eq, startswith</span></span>|
|<span data-ttu-id="8926a-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8926a-145">userPrincipalName</span></span>| <span data-ttu-id="8926a-146">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="8926a-146">eq, startswith</span></span>|
|<span data-ttu-id="8926a-147">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="8926a-147">appDisplayName</span></span>| <span data-ttu-id="8926a-148">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="8926a-148">eq, startswith</span></span>|
|<span data-ttu-id="8926a-149">ipAddress</span><span class="sxs-lookup"><span data-stu-id="8926a-149">ipAddress</span></span>| <span data-ttu-id="8926a-150">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="8926a-150">eq, startswith</span></span>|
|<span data-ttu-id="8926a-151">localização/cidade</span><span class="sxs-lookup"><span data-stu-id="8926a-151">location/city</span></span>| <span data-ttu-id="8926a-152">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="8926a-152">eq, startswith</span></span>|
|<span data-ttu-id="8926a-153">localização/estado</span><span class="sxs-lookup"><span data-stu-id="8926a-153">location/state</span></span>| <span data-ttu-id="8926a-154">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="8926a-154">eq, startswith</span></span>|
|<span data-ttu-id="8926a-155">location/countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="8926a-155">location/countryOrRegion</span></span>| <span data-ttu-id="8926a-156">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="8926a-156">eq, startswith</span></span>|
|<span data-ttu-id="8926a-157">status/errorCode</span><span class="sxs-lookup"><span data-stu-id="8926a-157">status/errorCode</span></span>|<span data-ttu-id="8926a-158">eq</span><span class="sxs-lookup"><span data-stu-id="8926a-158">eq</span></span>|
|<span data-ttu-id="8926a-159">initiatedBy/user/id</span><span class="sxs-lookup"><span data-stu-id="8926a-159">initiatedBy/user/id</span></span>|<span data-ttu-id="8926a-160">eq</span><span class="sxs-lookup"><span data-stu-id="8926a-160">eq</span></span>|
|<span data-ttu-id="8926a-161">initiatedBy/user/displayName</span><span class="sxs-lookup"><span data-stu-id="8926a-161">initiatedBy/user/displayName</span></span>| <span data-ttu-id="8926a-162">eq</span><span class="sxs-lookup"><span data-stu-id="8926a-162">eq</span></span>|
|<span data-ttu-id="8926a-163">initiatedBy/user/userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8926a-163">initiatedBy/user/userPrincipalName</span></span>| <span data-ttu-id="8926a-164">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="8926a-164">eq, startswith</span></span>|
|<span data-ttu-id="8926a-165">clientAppUsed</span><span class="sxs-lookup"><span data-stu-id="8926a-165">clientAppUsed</span></span>| <span data-ttu-id="8926a-166">eq</span><span class="sxs-lookup"><span data-stu-id="8926a-166">eq</span></span>|
|<span data-ttu-id="8926a-167">conditionalAccessStatus</span><span class="sxs-lookup"><span data-stu-id="8926a-167">conditionalAccessStatus</span></span> | <span data-ttu-id="8926a-168">eq</span><span class="sxs-lookup"><span data-stu-id="8926a-168">eq</span></span>|
|<span data-ttu-id="8926a-169">deviceDetail/browser</span><span class="sxs-lookup"><span data-stu-id="8926a-169">deviceDetail/browser</span></span>| <span data-ttu-id="8926a-170">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="8926a-170">eq, startswith</span></span>|
|<span data-ttu-id="8926a-171">deviceDetail/operatingSystem</span><span class="sxs-lookup"><span data-stu-id="8926a-171">deviceDetail/operatingSystem</span></span>| <span data-ttu-id="8926a-172">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="8926a-172">eq, startswith</span></span>|
|<span data-ttu-id="8926a-173">correlationId</span><span class="sxs-lookup"><span data-stu-id="8926a-173">correlationId</span></span>| <span data-ttu-id="8926a-174">eq</span><span class="sxs-lookup"><span data-stu-id="8926a-174">eq</span></span>|
|<span data-ttu-id="8926a-175">riskDetail</span><span class="sxs-lookup"><span data-stu-id="8926a-175">riskDetail</span></span>| <span data-ttu-id="8926a-176">eq</span><span class="sxs-lookup"><span data-stu-id="8926a-176">eq</span></span>|
|<span data-ttu-id="8926a-177">riskLevelAggregated</span><span class="sxs-lookup"><span data-stu-id="8926a-177">riskLevelAggregated</span></span>| <span data-ttu-id="8926a-178">eq</span><span class="sxs-lookup"><span data-stu-id="8926a-178">eq</span></span>|
|<span data-ttu-id="8926a-179">riskLevelDuringSignIn</span><span class="sxs-lookup"><span data-stu-id="8926a-179">riskLevelDuringSignIn</span></span>| <span data-ttu-id="8926a-180">eq</span><span class="sxs-lookup"><span data-stu-id="8926a-180">eq</span></span>|
|<span data-ttu-id="8926a-181">riskEventTypes</span><span class="sxs-lookup"><span data-stu-id="8926a-181">riskEventTypes</span></span>| <span data-ttu-id="8926a-182">eq</span><span class="sxs-lookup"><span data-stu-id="8926a-182">eq</span></span>|
|<span data-ttu-id="8926a-183">riskState</span><span class="sxs-lookup"><span data-stu-id="8926a-183">riskState</span></span>| <span data-ttu-id="8926a-184">eq</span><span class="sxs-lookup"><span data-stu-id="8926a-184">eq</span></span>|
|<span data-ttu-id="8926a-185">originalRequestId</span><span class="sxs-lookup"><span data-stu-id="8926a-185">originalRequestId</span></span>| <span data-ttu-id="8926a-186">eq</span><span class="sxs-lookup"><span data-stu-id="8926a-186">eq</span></span>|
|<span data-ttu-id="8926a-187">tokenIssuerName</span><span class="sxs-lookup"><span data-stu-id="8926a-187">tokenIssuerName</span></span>| <span data-ttu-id="8926a-188">eq</span><span class="sxs-lookup"><span data-stu-id="8926a-188">eq</span></span>|
|<span data-ttu-id="8926a-189">tokenIssuerType</span><span class="sxs-lookup"><span data-stu-id="8926a-189">tokenIssuerType</span></span>| <span data-ttu-id="8926a-190">eq</span><span class="sxs-lookup"><span data-stu-id="8926a-190">eq</span></span>|
|<span data-ttu-id="8926a-191">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="8926a-191">resourceDisplayName</span></span>| <span data-ttu-id="8926a-192">eq</span><span class="sxs-lookup"><span data-stu-id="8926a-192">eq</span></span>|
|<span data-ttu-id="8926a-193">resourceId</span><span class="sxs-lookup"><span data-stu-id="8926a-193">resourceId</span></span>| <span data-ttu-id="8926a-194">eq</span><span class="sxs-lookup"><span data-stu-id="8926a-194">eq</span></span>|


## <a name="response"></a><span data-ttu-id="8926a-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="8926a-195">Response</span></span>
<span data-ttu-id="8926a-196">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos de [logon](../resources/signin.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8926a-196">If successful, this method returns a `200 OK` response code and collection of [signIn](../resources/signin.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8926a-197">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8926a-197">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8926a-198">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8926a-198">Request</span></span>
<span data-ttu-id="8926a-199">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8926a-199">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_signins"
}-->
```http
GET https://graph.microsoft.com/beta/auditLogs/signIns
```
##### <a name="response"></a><span data-ttu-id="8926a-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="8926a-200">Response</span></span>
<span data-ttu-id="8926a-201">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8926a-201">Here is an example of the response.</span></span> 

><span data-ttu-id="8926a-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8926a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="8926a-204">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="8926a-204">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8926a-205">C#</span><span class="sxs-lookup"><span data-stu-id="8926a-205">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_signins-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8926a-206">Javascript</span><span class="sxs-lookup"><span data-stu-id="8926a-206">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_signins-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="8926a-207">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="8926a-207">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_signins-Objective-C-snippets.md)]
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
    "Error: /api-reference/beta/api/signin-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/signin-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/signin-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
