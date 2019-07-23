---
title: Listar logons
description: Descreve o método list do recurso de entrada (entidade) da API do Microsoft Graph.
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7e8499538ba5a5fa61159f4c1a5db68454dbf0d7
ms.sourcegitcommit: b198efc2391a12a840e4f1b8c42c18a55b06037f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/23/2019
ms.locfileid: "35820812"
---
# <a name="list-signins"></a><span data-ttu-id="066ba-103">Listar logons</span><span class="sxs-lookup"><span data-stu-id="066ba-103">List signIns</span></span>

<span data-ttu-id="066ba-104">Recupera os logons de usuário do Azure AD para seu locatário.</span><span class="sxs-lookup"><span data-stu-id="066ba-104">Retrieve the Azure AD user sign-ins for your tenant.</span></span> <span data-ttu-id="066ba-105">As entradas interativas por natureza (onde um nome de usuário/senha é passado como parte do token de autenticação) e os logins federados bem-sucedidos estão incluídos atualmente nos logs de entrada.</span><span class="sxs-lookup"><span data-stu-id="066ba-105">Sign-ins that are interactive in nature (where a username/password is passed as part of auth token) and successful federated sign-ins are currently included in the sign-in logs.</span></span>

## <a name="permissions"></a><span data-ttu-id="066ba-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="066ba-106">Permissions</span></span>

<span data-ttu-id="066ba-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="066ba-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="066ba-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="066ba-109">Permission type</span></span>      | <span data-ttu-id="066ba-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="066ba-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="066ba-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="066ba-111">Delegated (work or school account)</span></span> | <span data-ttu-id="066ba-112">AuditLog. Read. All e Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="066ba-112">AuditLog.Read.All and Directory.Read.All</span></span> |
|<span data-ttu-id="066ba-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="066ba-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="066ba-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="066ba-114">Not supported</span></span>   |
|<span data-ttu-id="066ba-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="066ba-115">Application</span></span> | <span data-ttu-id="066ba-116">AuditLog. Read. All e Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="066ba-116">AuditLog.Read.All and Directory.Read.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="066ba-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="066ba-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET auditLogs/signIns
```

## <a name="optional-query-parameters"></a><span data-ttu-id="066ba-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="066ba-118">Optional query parameters</span></span>

<span data-ttu-id="066ba-119">Este método oferece suporte aos seguintes parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="066ba-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="066ba-120">Para obter detalhes sobre como usar esses parâmetros, confira [Parâmetros de consulta do OData](/graph/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="066ba-120">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

|<span data-ttu-id="066ba-121">Nome</span><span class="sxs-lookup"><span data-stu-id="066ba-121">Name</span></span>     |<span data-ttu-id="066ba-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="066ba-122">Description</span></span>                            |<span data-ttu-id="066ba-123">Exemplo</span><span class="sxs-lookup"><span data-stu-id="066ba-123">Example</span></span>|
|:--------------------|----------------|------------------------------------------------------------------------|
|[<span data-ttu-id="066ba-124">$filter</span><span class="sxs-lookup"><span data-stu-id="066ba-124">$filter</span></span>](/graph/query_parameters#filter-parameter)|<span data-ttu-id="066ba-125">Filtra os resultados (linhas).</span><span class="sxs-lookup"><span data-stu-id="066ba-125">Filters results (rows).</span></span> |`/auditLogs/signIns?&$filter=createdDateTime le 2018-01-24`
|[<span data-ttu-id="066ba-126">$top</span><span class="sxs-lookup"><span data-stu-id="066ba-126">$top</span></span>](/graph/query_parameters#top-parameter)|<span data-ttu-id="066ba-127">Define o tamanho de página de resultados.</span><span class="sxs-lookup"><span data-stu-id="066ba-127">Sets the page size of results.</span></span>|`/auditLogs/signIns?$top=1`|
|[<span data-ttu-id="066ba-128">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="066ba-128">$skiptoken</span></span>](/graph/query_parameters#skiptoken-parameter)|<span data-ttu-id="066ba-129">Recupera a próxima página de resultados de conjuntos de resultados que abrangem várias páginas.</span><span class="sxs-lookup"><span data-stu-id="066ba-129">Retrieves the next page of results from result sets that span multiple pages.</span></span>|`/auditLogs/signIns?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1`|

### <a name="attributes-supported-by-filter-parameter"></a><span data-ttu-id="066ba-130">Atributos com suporte pelo parâmetro $filter</span><span class="sxs-lookup"><span data-stu-id="066ba-130">Attributes supported by $filter parameter</span></span>

|<span data-ttu-id="066ba-131">Nome do atributo</span><span class="sxs-lookup"><span data-stu-id="066ba-131">Attribute name</span></span> |<span data-ttu-id="066ba-132">Operadores com suporte</span><span class="sxs-lookup"><span data-stu-id="066ba-132">Supported operators</span></span>|
|:----------------|:------|
|<span data-ttu-id="066ba-133">id</span><span class="sxs-lookup"><span data-stu-id="066ba-133">id</span></span>|<span data-ttu-id="066ba-134">eq</span><span class="sxs-lookup"><span data-stu-id="066ba-134">eq</span></span>|
|<span data-ttu-id="066ba-135">userId</span><span class="sxs-lookup"><span data-stu-id="066ba-135">userId</span></span>|<span data-ttu-id="066ba-136">eq</span><span class="sxs-lookup"><span data-stu-id="066ba-136">eq</span></span>|
|<span data-ttu-id="066ba-137">appId</span><span class="sxs-lookup"><span data-stu-id="066ba-137">appId</span></span>|<span data-ttu-id="066ba-138">eq</span><span class="sxs-lookup"><span data-stu-id="066ba-138">eq</span></span>|
|<span data-ttu-id="066ba-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="066ba-139">createdDateTime</span></span>| <span data-ttu-id="066ba-140">eq, le, ge</span><span class="sxs-lookup"><span data-stu-id="066ba-140">eq, le, ge</span></span>|
|<span data-ttu-id="066ba-141">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="066ba-141">userDisplayName</span></span>| <span data-ttu-id="066ba-142">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="066ba-142">eq, startswith</span></span>|
|<span data-ttu-id="066ba-143">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="066ba-143">userPrincipalName</span></span>| <span data-ttu-id="066ba-144">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="066ba-144">eq, startswith</span></span>|
|<span data-ttu-id="066ba-145">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="066ba-145">appDisplayName</span></span>| <span data-ttu-id="066ba-146">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="066ba-146">eq, startswith</span></span>|
|<span data-ttu-id="066ba-147">ipAddress</span><span class="sxs-lookup"><span data-stu-id="066ba-147">ipAddress</span></span>| <span data-ttu-id="066ba-148">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="066ba-148">eq, startswith</span></span>|
|<span data-ttu-id="066ba-149">localização/cidade</span><span class="sxs-lookup"><span data-stu-id="066ba-149">location/city</span></span>| <span data-ttu-id="066ba-150">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="066ba-150">eq, startswith</span></span>|
|<span data-ttu-id="066ba-151">localização/estado</span><span class="sxs-lookup"><span data-stu-id="066ba-151">location/state</span></span>| <span data-ttu-id="066ba-152">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="066ba-152">eq, startswith</span></span>|
|<span data-ttu-id="066ba-153">location/countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="066ba-153">location/countryOrRegion</span></span>| <span data-ttu-id="066ba-154">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="066ba-154">eq, startswith</span></span>|
|<span data-ttu-id="066ba-155">status/errorCode</span><span class="sxs-lookup"><span data-stu-id="066ba-155">status/errorCode</span></span>|<span data-ttu-id="066ba-156">eq</span><span class="sxs-lookup"><span data-stu-id="066ba-156">eq</span></span>|
|<span data-ttu-id="066ba-157">initiatedBy/user/id</span><span class="sxs-lookup"><span data-stu-id="066ba-157">initiatedBy/user/id</span></span>|<span data-ttu-id="066ba-158">eq</span><span class="sxs-lookup"><span data-stu-id="066ba-158">eq</span></span>|
|<span data-ttu-id="066ba-159">initiatedBy/user/displayName</span><span class="sxs-lookup"><span data-stu-id="066ba-159">initiatedBy/user/displayName</span></span>| <span data-ttu-id="066ba-160">eq</span><span class="sxs-lookup"><span data-stu-id="066ba-160">eq</span></span>|
|<span data-ttu-id="066ba-161">initiatedBy/user/userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="066ba-161">initiatedBy/user/userPrincipalName</span></span>| <span data-ttu-id="066ba-162">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="066ba-162">eq, startswith</span></span>|
|<span data-ttu-id="066ba-163">clientAppUsed</span><span class="sxs-lookup"><span data-stu-id="066ba-163">clientAppUsed</span></span>| <span data-ttu-id="066ba-164">eq</span><span class="sxs-lookup"><span data-stu-id="066ba-164">eq</span></span>|
|<span data-ttu-id="066ba-165">conditionalAccessStatus</span><span class="sxs-lookup"><span data-stu-id="066ba-165">conditionalAccessStatus</span></span> | <span data-ttu-id="066ba-166">eq</span><span class="sxs-lookup"><span data-stu-id="066ba-166">eq</span></span>|
|<span data-ttu-id="066ba-167">deviceDetail/browser</span><span class="sxs-lookup"><span data-stu-id="066ba-167">deviceDetail/browser</span></span>| <span data-ttu-id="066ba-168">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="066ba-168">eq, startswith</span></span>|
|<span data-ttu-id="066ba-169">deviceDetail/operatingSystem</span><span class="sxs-lookup"><span data-stu-id="066ba-169">deviceDetail/operatingSystem</span></span>| <span data-ttu-id="066ba-170">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="066ba-170">eq, startswith</span></span>|
|<span data-ttu-id="066ba-171">correlationId</span><span class="sxs-lookup"><span data-stu-id="066ba-171">correlationId</span></span>| <span data-ttu-id="066ba-172">eq</span><span class="sxs-lookup"><span data-stu-id="066ba-172">eq</span></span>|
|<span data-ttu-id="066ba-173">isrisky</span><span class="sxs-lookup"><span data-stu-id="066ba-173">isRisky</span></span>| <span data-ttu-id="066ba-174">eq</span><span class="sxs-lookup"><span data-stu-id="066ba-174">eq</span></span>|

## <a name="response"></a><span data-ttu-id="066ba-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="066ba-175">Response</span></span>

<span data-ttu-id="066ba-176">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos de [logon](../resources/signin.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="066ba-176">If successful, this method returns a `200 OK` response code and collection of [signIn](../resources/signin.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="066ba-177">Exemplo</span><span class="sxs-lookup"><span data-stu-id="066ba-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="066ba-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="066ba-178">Request</span></span>

<span data-ttu-id="066ba-179">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="066ba-179">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="066ba-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="066ba-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_signins"
}-->
```http
GET https://graph.microsoft.com/v1.0/auditLogs/signIns
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="066ba-181">C#</span><span class="sxs-lookup"><span data-stu-id="066ba-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-signins-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="066ba-182">Javascript</span><span class="sxs-lookup"><span data-stu-id="066ba-182">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-signins-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="066ba-183">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="066ba-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-signins-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="066ba-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="066ba-184">Response</span></span>

<span data-ttu-id="066ba-185">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="066ba-185">Here is an example of the response.</span></span>
><span data-ttu-id="066ba-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="066ba-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  ]
}-->
