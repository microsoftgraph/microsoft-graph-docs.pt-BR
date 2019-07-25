---
title: Listar logons
description: Descreve o método de lista o recurso de logon (entidade) do Microsoft Graph API (REST), que ajuda a auditoria das atividades de diretório (locatário) (versão beta).
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 658d4abbbdeaff1f6f6de7c01756d821f4d4433b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869739"
---
# <a name="list-signins"></a><span data-ttu-id="0cb12-103">Listar logons</span><span class="sxs-lookup"><span data-stu-id="0cb12-103">List signIns</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0cb12-104">Recupera os logons de usuário do Azure AD para seu locatário.</span><span class="sxs-lookup"><span data-stu-id="0cb12-104">Retrieve the Azure AD user sign-ins for your tenant.</span></span> <span data-ttu-id="0cb12-105">Entradas que são interativas na natureza (onde um nome de usuário/senha é passado como parte de símbolo de autorização) e entradas federadas bem-sucedida atualmente estão incluídas nos logs de entrada.</span><span class="sxs-lookup"><span data-stu-id="0cb12-105">Sign-ins that are interactive in nature (where a username/password is passed as part of authorization token) and successful federated sign-ins are currently included in the sign-in logs.</span></span>  <span data-ttu-id="0cb12-106">Os logons mais recentes são retornados primeiro.</span><span class="sxs-lookup"><span data-stu-id="0cb12-106">The most recent signIns are returned first.</span></span>

## <a name="permissions"></a><span data-ttu-id="0cb12-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="0cb12-107">Permissions</span></span>

<span data-ttu-id="0cb12-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0cb12-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0cb12-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0cb12-110">Permission type</span></span>      | <span data-ttu-id="0cb12-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0cb12-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0cb12-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0cb12-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0cb12-113">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="0cb12-113">AuditLog.Read.All</span></span> |
|<span data-ttu-id="0cb12-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0cb12-114">Delegated (work or school account)</span></span> | <span data-ttu-id="0cb12-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="0cb12-115">Directory.Read.All</span></span> |
|<span data-ttu-id="0cb12-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0cb12-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0cb12-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="0cb12-117">Not supported</span></span>   |
|<span data-ttu-id="0cb12-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0cb12-118">Application</span></span> | <span data-ttu-id="0cb12-119">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="0cb12-119">AuditLog.Read.All</span></span> | 
|<span data-ttu-id="0cb12-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0cb12-120">Application</span></span> | <span data-ttu-id="0cb12-121">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="0cb12-121">Directory.Read.All</span></span>  | 


<span data-ttu-id="0cb12-122">Além disso, os aplicativos devem ser [corretamente registrados](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0cb12-122">In addition, apps must be [properly registered](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to Azure AD.</span></span>

## <a name="http-request"></a><span data-ttu-id="0cb12-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0cb12-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET auditLogs/signIns
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0cb12-124">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0cb12-124">Optional query parameters</span></span>
<span data-ttu-id="0cb12-125">Este método dá suporte aos seguintes Parâmetros de Consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0cb12-125">This method supports the following OData Query Parameters to help customize the response.</span></span> <span data-ttu-id="0cb12-126">Para obter detalhes sobre como usar esses parâmetros, confira [Parâmetros de consulta do OData](/graph/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="0cb12-126">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

|<span data-ttu-id="0cb12-127">Nome</span><span class="sxs-lookup"><span data-stu-id="0cb12-127">Name</span></span>     |<span data-ttu-id="0cb12-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="0cb12-128">Description</span></span>                            |<span data-ttu-id="0cb12-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0cb12-129">Example</span></span>|
|:--------------------|----------------|------------------------------------------------------------------------|
|[<span data-ttu-id="0cb12-130">$filter</span><span class="sxs-lookup"><span data-stu-id="0cb12-130">$filter</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#filter-parameter)|<span data-ttu-id="0cb12-131">Filtra os resultados (linhas).</span><span class="sxs-lookup"><span data-stu-id="0cb12-131">Filters results (rows).</span></span> |`/auditLogs/signIns?&$filter=createdDateTime le 2018-01-24`
|[<span data-ttu-id="0cb12-132">$top</span><span class="sxs-lookup"><span data-stu-id="0cb12-132">$top</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top-parameter)|<span data-ttu-id="0cb12-133">Define o tamanho de página de resultados.</span><span class="sxs-lookup"><span data-stu-id="0cb12-133">Sets the page size of results.</span></span>|`/auditLogs/signIns?$top=1`|
|[<span data-ttu-id="0cb12-134">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="0cb12-134">$skiptoken</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skiptoken-parameter)|<span data-ttu-id="0cb12-135">Recupera a próxima página de resultados de conjuntos de resultados que abrangem várias páginas.</span><span class="sxs-lookup"><span data-stu-id="0cb12-135">Retrieves the next page of results from result sets that span multiple pages.</span></span>|`/auditLogs/signIns?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1`|

### <a name="list-of-attributes-supported-by-filter-parameter"></a><span data-ttu-id="0cb12-136">Lista de atributos com suporte parâmetro $filter</span><span class="sxs-lookup"><span data-stu-id="0cb12-136">List of attributes supported by $filter parameter</span></span>
|<span data-ttu-id="0cb12-137">Nome do Atributo</span><span class="sxs-lookup"><span data-stu-id="0cb12-137">Attribute Name</span></span> |<span data-ttu-id="0cb12-138">Operadores com suporte</span><span class="sxs-lookup"><span data-stu-id="0cb12-138">Supported operators</span></span>|
|:----------------|:------|
|<span data-ttu-id="0cb12-139">id</span><span class="sxs-lookup"><span data-stu-id="0cb12-139">id</span></span>|<span data-ttu-id="0cb12-140">eq</span><span class="sxs-lookup"><span data-stu-id="0cb12-140">eq</span></span>|
|<span data-ttu-id="0cb12-141">userId</span><span class="sxs-lookup"><span data-stu-id="0cb12-141">userId</span></span>|<span data-ttu-id="0cb12-142">eq</span><span class="sxs-lookup"><span data-stu-id="0cb12-142">eq</span></span>|
|<span data-ttu-id="0cb12-143">appId</span><span class="sxs-lookup"><span data-stu-id="0cb12-143">appId</span></span>|<span data-ttu-id="0cb12-144">eq</span><span class="sxs-lookup"><span data-stu-id="0cb12-144">eq</span></span>|
|<span data-ttu-id="0cb12-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0cb12-145">createdDateTime</span></span>| <span data-ttu-id="0cb12-146">eq, le, ge</span><span class="sxs-lookup"><span data-stu-id="0cb12-146">eq, le, ge</span></span>|
|<span data-ttu-id="0cb12-147">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="0cb12-147">userDisplayName</span></span>| <span data-ttu-id="0cb12-148">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="0cb12-148">eq, startswith</span></span>|
|<span data-ttu-id="0cb12-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0cb12-149">userPrincipalName</span></span>| <span data-ttu-id="0cb12-150">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="0cb12-150">eq, startswith</span></span>|
|<span data-ttu-id="0cb12-151">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="0cb12-151">appDisplayName</span></span>| <span data-ttu-id="0cb12-152">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="0cb12-152">eq, startswith</span></span>|
|<span data-ttu-id="0cb12-153">ipAddress</span><span class="sxs-lookup"><span data-stu-id="0cb12-153">ipAddress</span></span>| <span data-ttu-id="0cb12-154">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="0cb12-154">eq, startswith</span></span>|
|<span data-ttu-id="0cb12-155">localização/cidade</span><span class="sxs-lookup"><span data-stu-id="0cb12-155">location/city</span></span>| <span data-ttu-id="0cb12-156">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="0cb12-156">eq, startswith</span></span>|
|<span data-ttu-id="0cb12-157">localização/estado</span><span class="sxs-lookup"><span data-stu-id="0cb12-157">location/state</span></span>| <span data-ttu-id="0cb12-158">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="0cb12-158">eq, startswith</span></span>|
|<span data-ttu-id="0cb12-159">location/countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="0cb12-159">location/countryOrRegion</span></span>| <span data-ttu-id="0cb12-160">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="0cb12-160">eq, startswith</span></span>|
|<span data-ttu-id="0cb12-161">status/errorCode</span><span class="sxs-lookup"><span data-stu-id="0cb12-161">status/errorCode</span></span>|<span data-ttu-id="0cb12-162">eq</span><span class="sxs-lookup"><span data-stu-id="0cb12-162">eq</span></span>|
|<span data-ttu-id="0cb12-163">initiatedBy/user/id</span><span class="sxs-lookup"><span data-stu-id="0cb12-163">initiatedBy/user/id</span></span>|<span data-ttu-id="0cb12-164">eq</span><span class="sxs-lookup"><span data-stu-id="0cb12-164">eq</span></span>|
|<span data-ttu-id="0cb12-165">initiatedBy/user/displayName</span><span class="sxs-lookup"><span data-stu-id="0cb12-165">initiatedBy/user/displayName</span></span>| <span data-ttu-id="0cb12-166">eq</span><span class="sxs-lookup"><span data-stu-id="0cb12-166">eq</span></span>|
|<span data-ttu-id="0cb12-167">initiatedBy/user/userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0cb12-167">initiatedBy/user/userPrincipalName</span></span>| <span data-ttu-id="0cb12-168">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="0cb12-168">eq, startswith</span></span>|
|<span data-ttu-id="0cb12-169">clientAppUsed</span><span class="sxs-lookup"><span data-stu-id="0cb12-169">clientAppUsed</span></span>| <span data-ttu-id="0cb12-170">eq</span><span class="sxs-lookup"><span data-stu-id="0cb12-170">eq</span></span>|
|<span data-ttu-id="0cb12-171">conditionalAccessStatus</span><span class="sxs-lookup"><span data-stu-id="0cb12-171">conditionalAccessStatus</span></span> | <span data-ttu-id="0cb12-172">eq</span><span class="sxs-lookup"><span data-stu-id="0cb12-172">eq</span></span>|
|<span data-ttu-id="0cb12-173">deviceDetail/browser</span><span class="sxs-lookup"><span data-stu-id="0cb12-173">deviceDetail/browser</span></span>| <span data-ttu-id="0cb12-174">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="0cb12-174">eq, startswith</span></span>|
|<span data-ttu-id="0cb12-175">deviceDetail/operatingSystem</span><span class="sxs-lookup"><span data-stu-id="0cb12-175">deviceDetail/operatingSystem</span></span>| <span data-ttu-id="0cb12-176">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="0cb12-176">eq, startswith</span></span>|
|<span data-ttu-id="0cb12-177">correlationId</span><span class="sxs-lookup"><span data-stu-id="0cb12-177">correlationId</span></span>| <span data-ttu-id="0cb12-178">eq</span><span class="sxs-lookup"><span data-stu-id="0cb12-178">eq</span></span>|
|<span data-ttu-id="0cb12-179">riskDetail</span><span class="sxs-lookup"><span data-stu-id="0cb12-179">riskDetail</span></span>| <span data-ttu-id="0cb12-180">eq</span><span class="sxs-lookup"><span data-stu-id="0cb12-180">eq</span></span>|
|<span data-ttu-id="0cb12-181">riskLevelAggregated</span><span class="sxs-lookup"><span data-stu-id="0cb12-181">riskLevelAggregated</span></span>| <span data-ttu-id="0cb12-182">eq</span><span class="sxs-lookup"><span data-stu-id="0cb12-182">eq</span></span>|
|<span data-ttu-id="0cb12-183">riskLevelDuringSignIn</span><span class="sxs-lookup"><span data-stu-id="0cb12-183">riskLevelDuringSignIn</span></span>| <span data-ttu-id="0cb12-184">eq</span><span class="sxs-lookup"><span data-stu-id="0cb12-184">eq</span></span>|
|<span data-ttu-id="0cb12-185">riskEventTypes</span><span class="sxs-lookup"><span data-stu-id="0cb12-185">riskEventTypes</span></span>| <span data-ttu-id="0cb12-186">eq</span><span class="sxs-lookup"><span data-stu-id="0cb12-186">eq</span></span>|
|<span data-ttu-id="0cb12-187">riskState</span><span class="sxs-lookup"><span data-stu-id="0cb12-187">riskState</span></span>| <span data-ttu-id="0cb12-188">eq</span><span class="sxs-lookup"><span data-stu-id="0cb12-188">eq</span></span>|
|<span data-ttu-id="0cb12-189">originalRequestId</span><span class="sxs-lookup"><span data-stu-id="0cb12-189">originalRequestId</span></span>| <span data-ttu-id="0cb12-190">eq</span><span class="sxs-lookup"><span data-stu-id="0cb12-190">eq</span></span>|
|<span data-ttu-id="0cb12-191">tokenIssuerName</span><span class="sxs-lookup"><span data-stu-id="0cb12-191">tokenIssuerName</span></span>| <span data-ttu-id="0cb12-192">eq</span><span class="sxs-lookup"><span data-stu-id="0cb12-192">eq</span></span>|
|<span data-ttu-id="0cb12-193">tokenIssuerType</span><span class="sxs-lookup"><span data-stu-id="0cb12-193">tokenIssuerType</span></span>| <span data-ttu-id="0cb12-194">eq</span><span class="sxs-lookup"><span data-stu-id="0cb12-194">eq</span></span>|
|<span data-ttu-id="0cb12-195">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="0cb12-195">resourceDisplayName</span></span>| <span data-ttu-id="0cb12-196">eq</span><span class="sxs-lookup"><span data-stu-id="0cb12-196">eq</span></span>|
|<span data-ttu-id="0cb12-197">resourceId</span><span class="sxs-lookup"><span data-stu-id="0cb12-197">resourceId</span></span>| <span data-ttu-id="0cb12-198">eq</span><span class="sxs-lookup"><span data-stu-id="0cb12-198">eq</span></span>|


## <a name="response"></a><span data-ttu-id="0cb12-199">Resposta</span><span class="sxs-lookup"><span data-stu-id="0cb12-199">Response</span></span>
<span data-ttu-id="0cb12-200">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos de [logon](../resources/signin.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0cb12-200">If successful, this method returns a `200 OK` response code and collection of [signIn](../resources/signin.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0cb12-201">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0cb12-201">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0cb12-202">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0cb12-202">Request</span></span>
<span data-ttu-id="0cb12-203">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0cb12-203">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0cb12-204">HTTP</span><span class="sxs-lookup"><span data-stu-id="0cb12-204">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signins"
}-->
```http
GET https://graph.microsoft.com/beta/auditLogs/signIns
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0cb12-205">C#</span><span class="sxs-lookup"><span data-stu-id="0cb12-205">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signins-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0cb12-206">Javascript</span><span class="sxs-lookup"><span data-stu-id="0cb12-206">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signins-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0cb12-207">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="0cb12-207">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signins-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0cb12-208">Java</span><span class="sxs-lookup"><span data-stu-id="0cb12-208">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signins-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0cb12-209">Resposta</span><span class="sxs-lookup"><span data-stu-id="0cb12-209">Response</span></span>
<span data-ttu-id="0cb12-210">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0cb12-210">Here is an example of the response.</span></span> 

><span data-ttu-id="0cb12-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0cb12-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
