---
title: Listar logons
description: Descreve o método list do recurso de entrada (entidade) da API do Microsoft Graph.
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3052ee368667f14932167f5a5d25dd168ab74264
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35279272"
---
# <a name="list-signins"></a><span data-ttu-id="f55a1-103">Listar logons</span><span class="sxs-lookup"><span data-stu-id="f55a1-103">List signIns</span></span>

<span data-ttu-id="f55a1-104">Recupera os logons de usuário do Azure AD para seu locatário.</span><span class="sxs-lookup"><span data-stu-id="f55a1-104">Retrieve the Azure AD user sign-ins for your tenant.</span></span> <span data-ttu-id="f55a1-105">As entradas interativas por natureza (onde um nome de usuário/senha é passado como parte do token de autenticação) e os logins federados bem-sucedidos estão incluídos atualmente nos logs de entrada.</span><span class="sxs-lookup"><span data-stu-id="f55a1-105">Sign-ins that are interactive in nature (where a username/password is passed as part of auth token) and successful federated sign-ins are currently included in the sign-in logs.</span></span>

## <a name="permissions"></a><span data-ttu-id="f55a1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f55a1-106">Permissions</span></span>

<span data-ttu-id="f55a1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="f55a1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="f55a1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f55a1-109">Permission type</span></span>      | <span data-ttu-id="f55a1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f55a1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f55a1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f55a1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f55a1-112">AuditLog. Read. All e Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="f55a1-112">AuditLog.Read.All and Directory.Read.All</span></span> |
|<span data-ttu-id="f55a1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f55a1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f55a1-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f55a1-114">Not supported</span></span>   |
|<span data-ttu-id="f55a1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f55a1-115">Application</span></span> | <span data-ttu-id="f55a1-116">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="f55a1-116">AuditLog.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f55a1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f55a1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET auditLogs/signIns
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f55a1-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f55a1-118">Optional query parameters</span></span>

<span data-ttu-id="f55a1-119">Este método oferece suporte aos seguintes parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f55a1-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="f55a1-120">Para obter detalhes sobre como usar esses parâmetros, confira [Parâmetros de consulta do OData](/graph/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="f55a1-120">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

|<span data-ttu-id="f55a1-121">Nome</span><span class="sxs-lookup"><span data-stu-id="f55a1-121">Name</span></span>     |<span data-ttu-id="f55a1-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f55a1-122">Description</span></span>                            |<span data-ttu-id="f55a1-123">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f55a1-123">Example</span></span>|
|:--------------------|----------------|------------------------------------------------------------------------|
|[<span data-ttu-id="f55a1-124">$filter</span><span class="sxs-lookup"><span data-stu-id="f55a1-124">$filter</span></span>](/graph/query_parameters#filter-parameter)|<span data-ttu-id="f55a1-125">Filtra os resultados (linhas).</span><span class="sxs-lookup"><span data-stu-id="f55a1-125">Filters results (rows).</span></span> |`/auditLogs/signIns?&$filter=createdDateTime le 2018-01-24`
|[<span data-ttu-id="f55a1-126">$top</span><span class="sxs-lookup"><span data-stu-id="f55a1-126">$top</span></span>](/graph/query_parameters#top-parameter)|<span data-ttu-id="f55a1-127">Define o tamanho de página de resultados.</span><span class="sxs-lookup"><span data-stu-id="f55a1-127">Sets the page size of results.</span></span>|`/auditLogs/signIns?$top=1`|
|[<span data-ttu-id="f55a1-128">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="f55a1-128">$skiptoken</span></span>](/graph/query_parameters#skiptoken-parameter)|<span data-ttu-id="f55a1-129">Recupera a próxima página de resultados de conjuntos de resultados que abrangem várias páginas.</span><span class="sxs-lookup"><span data-stu-id="f55a1-129">Retrieves the next page of results from result sets that span multiple pages.</span></span>|`/auditLogs/signIns?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1`|

### <a name="attributes-supported-by-filter-parameter"></a><span data-ttu-id="f55a1-130">Atributos com suporte pelo parâmetro $filter</span><span class="sxs-lookup"><span data-stu-id="f55a1-130">Attributes supported by $filter parameter</span></span>

|<span data-ttu-id="f55a1-131">Nome do atributo</span><span class="sxs-lookup"><span data-stu-id="f55a1-131">Attribute name</span></span> |<span data-ttu-id="f55a1-132">Operadores com suporte</span><span class="sxs-lookup"><span data-stu-id="f55a1-132">Supported operators</span></span>|
|:----------------|:------|
|<span data-ttu-id="f55a1-133">id</span><span class="sxs-lookup"><span data-stu-id="f55a1-133">id</span></span>|<span data-ttu-id="f55a1-134">eq</span><span class="sxs-lookup"><span data-stu-id="f55a1-134">eq</span></span>|
|<span data-ttu-id="f55a1-135">userId</span><span class="sxs-lookup"><span data-stu-id="f55a1-135">userId</span></span>|<span data-ttu-id="f55a1-136">eq</span><span class="sxs-lookup"><span data-stu-id="f55a1-136">eq</span></span>|
|<span data-ttu-id="f55a1-137">appId</span><span class="sxs-lookup"><span data-stu-id="f55a1-137">appId</span></span>|<span data-ttu-id="f55a1-138">eq</span><span class="sxs-lookup"><span data-stu-id="f55a1-138">eq</span></span>|
|<span data-ttu-id="f55a1-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f55a1-139">createdDateTime</span></span>| <span data-ttu-id="f55a1-140">eq, le, ge</span><span class="sxs-lookup"><span data-stu-id="f55a1-140">eq, le, ge</span></span>|
|<span data-ttu-id="f55a1-141">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="f55a1-141">userDisplayName</span></span>| <span data-ttu-id="f55a1-142">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="f55a1-142">eq, startswith</span></span>|
|<span data-ttu-id="f55a1-143">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f55a1-143">userPrincipalName</span></span>| <span data-ttu-id="f55a1-144">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="f55a1-144">eq, startswith</span></span>|
|<span data-ttu-id="f55a1-145">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="f55a1-145">appDisplayName</span></span>| <span data-ttu-id="f55a1-146">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="f55a1-146">eq, startswith</span></span>|
|<span data-ttu-id="f55a1-147">ipAddress</span><span class="sxs-lookup"><span data-stu-id="f55a1-147">ipAddress</span></span>| <span data-ttu-id="f55a1-148">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="f55a1-148">eq, startswith</span></span>|
|<span data-ttu-id="f55a1-149">localização/cidade</span><span class="sxs-lookup"><span data-stu-id="f55a1-149">location/city</span></span>| <span data-ttu-id="f55a1-150">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="f55a1-150">eq, startswith</span></span>|
|<span data-ttu-id="f55a1-151">localização/estado</span><span class="sxs-lookup"><span data-stu-id="f55a1-151">location/state</span></span>| <span data-ttu-id="f55a1-152">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="f55a1-152">eq, startswith</span></span>|
|<span data-ttu-id="f55a1-153">location/countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="f55a1-153">location/countryOrRegion</span></span>| <span data-ttu-id="f55a1-154">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="f55a1-154">eq, startswith</span></span>|
|<span data-ttu-id="f55a1-155">status/errorCode</span><span class="sxs-lookup"><span data-stu-id="f55a1-155">status/errorCode</span></span>|<span data-ttu-id="f55a1-156">eq</span><span class="sxs-lookup"><span data-stu-id="f55a1-156">eq</span></span>|
|<span data-ttu-id="f55a1-157">initiatedBy/user/id</span><span class="sxs-lookup"><span data-stu-id="f55a1-157">initiatedBy/user/id</span></span>|<span data-ttu-id="f55a1-158">eq</span><span class="sxs-lookup"><span data-stu-id="f55a1-158">eq</span></span>|
|<span data-ttu-id="f55a1-159">initiatedBy/user/displayName</span><span class="sxs-lookup"><span data-stu-id="f55a1-159">initiatedBy/user/displayName</span></span>| <span data-ttu-id="f55a1-160">eq</span><span class="sxs-lookup"><span data-stu-id="f55a1-160">eq</span></span>|
|<span data-ttu-id="f55a1-161">initiatedBy/user/userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f55a1-161">initiatedBy/user/userPrincipalName</span></span>| <span data-ttu-id="f55a1-162">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="f55a1-162">eq, startswith</span></span>|
|<span data-ttu-id="f55a1-163">clientAppUsed</span><span class="sxs-lookup"><span data-stu-id="f55a1-163">clientAppUsed</span></span>| <span data-ttu-id="f55a1-164">eq</span><span class="sxs-lookup"><span data-stu-id="f55a1-164">eq</span></span>|
|<span data-ttu-id="f55a1-165">conditionalAccessStatus</span><span class="sxs-lookup"><span data-stu-id="f55a1-165">conditionalAccessStatus</span></span> | <span data-ttu-id="f55a1-166">eq</span><span class="sxs-lookup"><span data-stu-id="f55a1-166">eq</span></span>|
|<span data-ttu-id="f55a1-167">deviceDetails/navegador</span><span class="sxs-lookup"><span data-stu-id="f55a1-167">deviceDetails/browser</span></span>| <span data-ttu-id="f55a1-168">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="f55a1-168">eq, startswith</span></span>|
|<span data-ttu-id="f55a1-169">deviceDetails/operatingSystem</span><span class="sxs-lookup"><span data-stu-id="f55a1-169">deviceDetails/operatingSystem</span></span>| <span data-ttu-id="f55a1-170">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="f55a1-170">eq, startswith</span></span>|
|<span data-ttu-id="f55a1-171">correlationId</span><span class="sxs-lookup"><span data-stu-id="f55a1-171">correlationId</span></span>| <span data-ttu-id="f55a1-172">eq</span><span class="sxs-lookup"><span data-stu-id="f55a1-172">eq</span></span>|
|<span data-ttu-id="f55a1-173">isrisky</span><span class="sxs-lookup"><span data-stu-id="f55a1-173">isRisky</span></span>| <span data-ttu-id="f55a1-174">eq</span><span class="sxs-lookup"><span data-stu-id="f55a1-174">eq</span></span>|

## <a name="response"></a><span data-ttu-id="f55a1-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="f55a1-175">Response</span></span>

<span data-ttu-id="f55a1-176">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos de [logon](../resources/signin.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f55a1-176">If successful, this method returns a `200 OK` response code and collection of [signIn](../resources/signin.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f55a1-177">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f55a1-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="f55a1-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f55a1-178">Request</span></span>

<span data-ttu-id="f55a1-179">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f55a1-179">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_signins"
}-->
```http
GET https://graph.microsoft.com/v1.0/auditLogs/signIns
```

### <a name="response"></a><span data-ttu-id="f55a1-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="f55a1-180">Response</span></span>

<span data-ttu-id="f55a1-181">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f55a1-181">Here is an example of the response.</span></span>
><span data-ttu-id="f55a1-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f55a1-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="f55a1-184">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="f55a1-184">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f55a1-185">C#</span><span class="sxs-lookup"><span data-stu-id="f55a1-185">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/list_signins-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f55a1-186">Javascript</span><span class="sxs-lookup"><span data-stu-id="f55a1-186">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/list_signins-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="f55a1-187">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="f55a1-187">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/list_signins-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

```json
{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#auditLogs/signIns",
    "value": [{
        "id": "id",
        "appId": "d3590ed6-52b3-4102-aeff-aad2292ab01c",
        "appDisplayName": "Azure",
        "createdDateTime": "2018-01-09T21:17:21.5077253Z",
        "clientAppUsed": null,
        "conditionalAccessApplied": true,
        "conditionalAccessPolicies": [{
            "id": "26490ed6-52b3-4102-aeff-aad2292abacf",
            "displayName": "capPolicy",
            "enforcedAccessControls": ["MFA", "TOU"],
            "enforcedSessionControls": ["CloudAppSecurity"],
            "result": "success"
        }],
        "correlationId": "17444d3c-563d-4b08-ac20-815892b87e42",
        "deviceDetail": {
            "deviceId": "34390ed6-52b3-4102-aeff-aad2292abac3",
            "displayName": "DeviceName",
            "operatingSystem": "Windows 10",
            "browser": "Rich Client v3.14.1592.7",
            "isCompliant": true,
            "isManaged": true,
            "trustType": ""
        },
        "ipAddress": "127.0.0.1",
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
        "status": {
            "errorCode": 0,
            "failureReason": null,
            "additionalDetails": "SignIn Success & CA Success"
        },
        "userDisplayName": "Jamie Doe",
        "userPrincipalName": "jdoe@wingtiptoys.com",
        "userId": "bbb3b4b5-e6e6-f7f5-f7f5-090805040302"
    }]
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
    "Error: /api-reference/v1.0/api/signin-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/signin-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/signin-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
