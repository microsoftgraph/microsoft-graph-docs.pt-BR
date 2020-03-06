---
title: Listar logons
description: Descreve o método list do recurso de entrada (entidade) da API do Microsoft Graph.
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7d09129637be85c568b8d99dd57bfd0e35507004
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509812"
---
# <a name="list-signins"></a><span data-ttu-id="08964-103">Listar logons</span><span class="sxs-lookup"><span data-stu-id="08964-103">List signIns</span></span>

<span data-ttu-id="08964-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08964-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="08964-105">Recupera os logons de usuário do Azure AD para seu locatário.</span><span class="sxs-lookup"><span data-stu-id="08964-105">Retrieve the Azure AD user sign-ins for your tenant.</span></span> <span data-ttu-id="08964-106">As entradas interativas por natureza (onde um nome de usuário/senha é passado como parte do token de autenticação) e os logins federados bem-sucedidos estão incluídos atualmente nos logs de entrada.</span><span class="sxs-lookup"><span data-stu-id="08964-106">Sign-ins that are interactive in nature (where a username/password is passed as part of auth token) and successful federated sign-ins are currently included in the sign-in logs.</span></span>

## <a name="permissions"></a><span data-ttu-id="08964-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="08964-107">Permissions</span></span>

<span data-ttu-id="08964-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="08964-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="08964-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="08964-110">Permission type</span></span>      | <span data-ttu-id="08964-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="08964-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08964-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="08964-112">Delegated (work or school account)</span></span> | <span data-ttu-id="08964-113">AuditLog. Read. All e Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="08964-113">AuditLog.Read.All and Directory.Read.All</span></span> |
|<span data-ttu-id="08964-114">Delegado (conta pessoal da conta Microsoft)</span><span class="sxs-lookup"><span data-stu-id="08964-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08964-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="08964-115">Not supported</span></span>   |
|<span data-ttu-id="08964-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="08964-116">Application</span></span> | <span data-ttu-id="08964-117">AuditLog. Read. All e Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="08964-117">AuditLog.Read.All and Directory.Read.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="08964-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="08964-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET auditLogs/signIns
```

## <a name="optional-query-parameters"></a><span data-ttu-id="08964-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="08964-119">Optional query parameters</span></span>

<span data-ttu-id="08964-120">Este método oferece suporte aos seguintes parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="08964-120">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="08964-121">Para obter detalhes sobre como usar esses parâmetros, confira [Parâmetros de consulta do OData](/graph/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="08964-121">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

|<span data-ttu-id="08964-122">Nome</span><span class="sxs-lookup"><span data-stu-id="08964-122">Name</span></span>     |<span data-ttu-id="08964-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="08964-123">Description</span></span>                            |<span data-ttu-id="08964-124">Exemplo</span><span class="sxs-lookup"><span data-stu-id="08964-124">Example</span></span>|
|:--------------------|----------------|------------------------------------------------------------------------|
|[<span data-ttu-id="08964-125">$filter</span><span class="sxs-lookup"><span data-stu-id="08964-125">$filter</span></span>](/graph/query_parameters#filter-parameter)|<span data-ttu-id="08964-126">Filtra os resultados (linhas).</span><span class="sxs-lookup"><span data-stu-id="08964-126">Filters results (rows).</span></span> |`/auditLogs/signIns?&$filter=createdDateTime le 2018-01-24`
|[<span data-ttu-id="08964-127">$top</span><span class="sxs-lookup"><span data-stu-id="08964-127">$top</span></span>](/graph/query_parameters#top-parameter)|<span data-ttu-id="08964-128">Define o tamanho de página de resultados.</span><span class="sxs-lookup"><span data-stu-id="08964-128">Sets the page size of results.</span></span>|`/auditLogs/signIns?$top=1`|
|[<span data-ttu-id="08964-129">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="08964-129">$skiptoken</span></span>](/graph/query_parameters#skiptoken-parameter)|<span data-ttu-id="08964-130">Recupera a próxima página de resultados de conjuntos de resultados que abrangem várias páginas.</span><span class="sxs-lookup"><span data-stu-id="08964-130">Retrieves the next page of results from result sets that span multiple pages.</span></span>|`/auditLogs/signIns?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1`|

### <a name="attributes-supported-by-filter-parameter"></a><span data-ttu-id="08964-131">Atributos com suporte pelo parâmetro $filter</span><span class="sxs-lookup"><span data-stu-id="08964-131">Attributes supported by $filter parameter</span></span>

|<span data-ttu-id="08964-132">Nome do atributo</span><span class="sxs-lookup"><span data-stu-id="08964-132">Attribute name</span></span> |<span data-ttu-id="08964-133">Operadores com suporte</span><span class="sxs-lookup"><span data-stu-id="08964-133">Supported operators</span></span>|
|:----------------|:------|
|<span data-ttu-id="08964-134">id</span><span class="sxs-lookup"><span data-stu-id="08964-134">id</span></span>|<span data-ttu-id="08964-135">eq</span><span class="sxs-lookup"><span data-stu-id="08964-135">eq</span></span>|
|<span data-ttu-id="08964-136">userId</span><span class="sxs-lookup"><span data-stu-id="08964-136">userId</span></span>|<span data-ttu-id="08964-137">eq</span><span class="sxs-lookup"><span data-stu-id="08964-137">eq</span></span>|
|<span data-ttu-id="08964-138">appId</span><span class="sxs-lookup"><span data-stu-id="08964-138">appId</span></span>|<span data-ttu-id="08964-139">eq</span><span class="sxs-lookup"><span data-stu-id="08964-139">eq</span></span>|
|<span data-ttu-id="08964-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="08964-140">createdDateTime</span></span>| <span data-ttu-id="08964-141">eq, le, ge</span><span class="sxs-lookup"><span data-stu-id="08964-141">eq, le, ge</span></span>|
|<span data-ttu-id="08964-142">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="08964-142">userDisplayName</span></span>| <span data-ttu-id="08964-143">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="08964-143">eq, startswith</span></span>|
|<span data-ttu-id="08964-144">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="08964-144">userPrincipalName</span></span>| <span data-ttu-id="08964-145">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="08964-145">eq, startswith</span></span>|
|<span data-ttu-id="08964-146">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="08964-146">appDisplayName</span></span>| <span data-ttu-id="08964-147">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="08964-147">eq, startswith</span></span>|
|<span data-ttu-id="08964-148">ipAddress</span><span class="sxs-lookup"><span data-stu-id="08964-148">ipAddress</span></span>| <span data-ttu-id="08964-149">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="08964-149">eq, startswith</span></span>|
|<span data-ttu-id="08964-150">localização/cidade</span><span class="sxs-lookup"><span data-stu-id="08964-150">location/city</span></span>| <span data-ttu-id="08964-151">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="08964-151">eq, startswith</span></span>|
|<span data-ttu-id="08964-152">localização/estado</span><span class="sxs-lookup"><span data-stu-id="08964-152">location/state</span></span>| <span data-ttu-id="08964-153">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="08964-153">eq, startswith</span></span>|
|<span data-ttu-id="08964-154">location/countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="08964-154">location/countryOrRegion</span></span>| <span data-ttu-id="08964-155">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="08964-155">eq, startswith</span></span>|
|<span data-ttu-id="08964-156">status/errorCode</span><span class="sxs-lookup"><span data-stu-id="08964-156">status/errorCode</span></span>|<span data-ttu-id="08964-157">eq</span><span class="sxs-lookup"><span data-stu-id="08964-157">eq</span></span>|
|<span data-ttu-id="08964-158">initiatedBy/user/id</span><span class="sxs-lookup"><span data-stu-id="08964-158">initiatedBy/user/id</span></span>|<span data-ttu-id="08964-159">eq</span><span class="sxs-lookup"><span data-stu-id="08964-159">eq</span></span>|
|<span data-ttu-id="08964-160">initiatedBy/user/displayName</span><span class="sxs-lookup"><span data-stu-id="08964-160">initiatedBy/user/displayName</span></span>| <span data-ttu-id="08964-161">eq</span><span class="sxs-lookup"><span data-stu-id="08964-161">eq</span></span>|
|<span data-ttu-id="08964-162">initiatedBy/user/userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="08964-162">initiatedBy/user/userPrincipalName</span></span>| <span data-ttu-id="08964-163">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="08964-163">eq, startswith</span></span>|
|<span data-ttu-id="08964-164">clientAppUsed</span><span class="sxs-lookup"><span data-stu-id="08964-164">clientAppUsed</span></span>| <span data-ttu-id="08964-165">eq</span><span class="sxs-lookup"><span data-stu-id="08964-165">eq</span></span>|
|<span data-ttu-id="08964-166">conditionalAccessStatus</span><span class="sxs-lookup"><span data-stu-id="08964-166">conditionalAccessStatus</span></span> | <span data-ttu-id="08964-167">eq</span><span class="sxs-lookup"><span data-stu-id="08964-167">eq</span></span>|
|<span data-ttu-id="08964-168">deviceDetail/browser</span><span class="sxs-lookup"><span data-stu-id="08964-168">deviceDetail/browser</span></span>| <span data-ttu-id="08964-169">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="08964-169">eq, startswith</span></span>|
|<span data-ttu-id="08964-170">deviceDetail/operatingSystem</span><span class="sxs-lookup"><span data-stu-id="08964-170">deviceDetail/operatingSystem</span></span>| <span data-ttu-id="08964-171">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="08964-171">eq, startswith</span></span>|
|<span data-ttu-id="08964-172">correlationId</span><span class="sxs-lookup"><span data-stu-id="08964-172">correlationId</span></span>| <span data-ttu-id="08964-173">eq</span><span class="sxs-lookup"><span data-stu-id="08964-173">eq</span></span>|
|<span data-ttu-id="08964-174">isrisky</span><span class="sxs-lookup"><span data-stu-id="08964-174">isRisky</span></span>| <span data-ttu-id="08964-175">eq</span><span class="sxs-lookup"><span data-stu-id="08964-175">eq</span></span>|

## <a name="response"></a><span data-ttu-id="08964-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="08964-176">Response</span></span>

<span data-ttu-id="08964-177">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos de [logon](../resources/signin.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="08964-177">If successful, this method returns a `200 OK` response code and collection of [signIn](../resources/signin.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08964-178">Exemplo</span><span class="sxs-lookup"><span data-stu-id="08964-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="08964-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="08964-179">Request</span></span>

<span data-ttu-id="08964-180">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="08964-180">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="08964-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="08964-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_signins"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/auditLogs/signIns
```
# <a name="c"></a>[<span data-ttu-id="08964-182">C#</span><span class="sxs-lookup"><span data-stu-id="08964-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-signins-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="08964-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="08964-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-signins-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="08964-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="08964-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-signins-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="08964-185">Java</span><span class="sxs-lookup"><span data-stu-id="08964-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-signins-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="08964-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="08964-186">Response</span></span>

<span data-ttu-id="08964-187">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="08964-187">Here is an example of the response.</span></span>
><span data-ttu-id="08964-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="08964-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
