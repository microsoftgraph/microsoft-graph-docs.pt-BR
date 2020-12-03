---
title: Listar logons
description: Descreve o método list do recurso de entrada (entidade) da API do Microsoft Graph.
localization_priority: Normal
author: besiler
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a7218b1fb30906c309664464069f2364af29dfde
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523529"
---
# <a name="list-signins"></a><span data-ttu-id="7e50a-103">Listar logons</span><span class="sxs-lookup"><span data-stu-id="7e50a-103">List signIns</span></span>

<span data-ttu-id="7e50a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e50a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7e50a-105">Recupera os logons de usuário do Azure AD para seu locatário.</span><span class="sxs-lookup"><span data-stu-id="7e50a-105">Retrieve the Azure AD user sign-ins for your tenant.</span></span> <span data-ttu-id="7e50a-106">As entradas interativas por natureza (onde um nome de usuário/senha é passado como parte do token de autenticação) e os logins federados bem-sucedidos estão incluídos atualmente nos logs de entrada.</span><span class="sxs-lookup"><span data-stu-id="7e50a-106">Sign-ins that are interactive in nature (where a username/password is passed as part of auth token) and successful federated sign-ins are currently included in the sign-in logs.</span></span>

## <a name="permissions"></a><span data-ttu-id="7e50a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="7e50a-107">Permissions</span></span>

<span data-ttu-id="7e50a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="7e50a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="7e50a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7e50a-110">Permission type</span></span>      | <span data-ttu-id="7e50a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7e50a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7e50a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7e50a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7e50a-113">AuditLog. Read. All e Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="7e50a-113">AuditLog.Read.All and Directory.Read.All</span></span> |
|<span data-ttu-id="7e50a-114">Delegado (conta pessoal da conta Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7e50a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e50a-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7e50a-115">Not supported</span></span>   |
|<span data-ttu-id="7e50a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7e50a-116">Application</span></span> | <span data-ttu-id="7e50a-117">AuditLog. Read. All e Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="7e50a-117">AuditLog.Read.All and Directory.Read.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="7e50a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7e50a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET auditLogs/signIns
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7e50a-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7e50a-119">Optional query parameters</span></span>

<span data-ttu-id="7e50a-120">Este método oferece suporte aos seguintes parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7e50a-120">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="7e50a-121">Para obter detalhes sobre como usar esses parâmetros, confira [Parâmetros de consulta do OData](/graph/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="7e50a-121">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

|<span data-ttu-id="7e50a-122">Nome</span><span class="sxs-lookup"><span data-stu-id="7e50a-122">Name</span></span>     |<span data-ttu-id="7e50a-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e50a-123">Description</span></span>                            |<span data-ttu-id="7e50a-124">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7e50a-124">Example</span></span>|
|:--------------------|----------------|------------------------------------------------------------------------|
|[<span data-ttu-id="7e50a-125">$filter</span><span class="sxs-lookup"><span data-stu-id="7e50a-125">$filter</span></span>](/graph/query_parameters#filter-parameter)|<span data-ttu-id="7e50a-126">Filtra os resultados (linhas).</span><span class="sxs-lookup"><span data-stu-id="7e50a-126">Filters results (rows).</span></span> |`/auditLogs/signIns?&$filter=createdDateTime le 2018-01-24`
|[<span data-ttu-id="7e50a-127">$top</span><span class="sxs-lookup"><span data-stu-id="7e50a-127">$top</span></span>](/graph/query_parameters#top-parameter)|<span data-ttu-id="7e50a-128">Define o tamanho de página de resultados.</span><span class="sxs-lookup"><span data-stu-id="7e50a-128">Sets the page size of results.</span></span>|`/auditLogs/signIns?$top=1`|
|[<span data-ttu-id="7e50a-129">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="7e50a-129">$skiptoken</span></span>](/graph/query_parameters#skiptoken-parameter)|<span data-ttu-id="7e50a-130">Recupera a próxima página de resultados de conjuntos de resultados que abrangem várias páginas.</span><span class="sxs-lookup"><span data-stu-id="7e50a-130">Retrieves the next page of results from result sets that span multiple pages.</span></span>|`/auditLogs/signIns?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1`|

### <a name="attributes-supported-by-filter-parameter"></a><span data-ttu-id="7e50a-131">Atributos com suporte pelo parâmetro $filter</span><span class="sxs-lookup"><span data-stu-id="7e50a-131">Attributes supported by $filter parameter</span></span>

|<span data-ttu-id="7e50a-132">Nome do atributo</span><span class="sxs-lookup"><span data-stu-id="7e50a-132">Attribute name</span></span> |<span data-ttu-id="7e50a-133">Operadores com suporte</span><span class="sxs-lookup"><span data-stu-id="7e50a-133">Supported operators</span></span>|
|:----------------|:------|
|<span data-ttu-id="7e50a-134">id</span><span class="sxs-lookup"><span data-stu-id="7e50a-134">id</span></span>|<span data-ttu-id="7e50a-135">eq</span><span class="sxs-lookup"><span data-stu-id="7e50a-135">eq</span></span>|
|<span data-ttu-id="7e50a-136">userId</span><span class="sxs-lookup"><span data-stu-id="7e50a-136">userId</span></span>|<span data-ttu-id="7e50a-137">eq</span><span class="sxs-lookup"><span data-stu-id="7e50a-137">eq</span></span>|
|<span data-ttu-id="7e50a-138">appId</span><span class="sxs-lookup"><span data-stu-id="7e50a-138">appId</span></span>|<span data-ttu-id="7e50a-139">eq</span><span class="sxs-lookup"><span data-stu-id="7e50a-139">eq</span></span>|
|<span data-ttu-id="7e50a-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7e50a-140">createdDateTime</span></span>| <span data-ttu-id="7e50a-141">eq, le, ge</span><span class="sxs-lookup"><span data-stu-id="7e50a-141">eq, le, ge</span></span>|
|<span data-ttu-id="7e50a-142">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="7e50a-142">userDisplayName</span></span>| <span data-ttu-id="7e50a-143">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="7e50a-143">eq, startswith</span></span>|
|<span data-ttu-id="7e50a-144">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7e50a-144">userPrincipalName</span></span>| <span data-ttu-id="7e50a-145">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="7e50a-145">eq, startswith</span></span>|
|<span data-ttu-id="7e50a-146">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="7e50a-146">appDisplayName</span></span>| <span data-ttu-id="7e50a-147">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="7e50a-147">eq, startswith</span></span>|
|<span data-ttu-id="7e50a-148">ipAddress</span><span class="sxs-lookup"><span data-stu-id="7e50a-148">ipAddress</span></span>| <span data-ttu-id="7e50a-149">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="7e50a-149">eq, startswith</span></span>|
|<span data-ttu-id="7e50a-150">localização/cidade</span><span class="sxs-lookup"><span data-stu-id="7e50a-150">location/city</span></span>| <span data-ttu-id="7e50a-151">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="7e50a-151">eq, startswith</span></span>|
|<span data-ttu-id="7e50a-152">localização/estado</span><span class="sxs-lookup"><span data-stu-id="7e50a-152">location/state</span></span>| <span data-ttu-id="7e50a-153">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="7e50a-153">eq, startswith</span></span>|
|<span data-ttu-id="7e50a-154">location/countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="7e50a-154">location/countryOrRegion</span></span>| <span data-ttu-id="7e50a-155">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="7e50a-155">eq, startswith</span></span>|
|<span data-ttu-id="7e50a-156">status/errorCode</span><span class="sxs-lookup"><span data-stu-id="7e50a-156">status/errorCode</span></span>|<span data-ttu-id="7e50a-157">eq</span><span class="sxs-lookup"><span data-stu-id="7e50a-157">eq</span></span>|
|<span data-ttu-id="7e50a-158">initiatedBy/user/id</span><span class="sxs-lookup"><span data-stu-id="7e50a-158">initiatedBy/user/id</span></span>|<span data-ttu-id="7e50a-159">eq</span><span class="sxs-lookup"><span data-stu-id="7e50a-159">eq</span></span>|
|<span data-ttu-id="7e50a-160">initiatedBy/user/displayName</span><span class="sxs-lookup"><span data-stu-id="7e50a-160">initiatedBy/user/displayName</span></span>| <span data-ttu-id="7e50a-161">eq</span><span class="sxs-lookup"><span data-stu-id="7e50a-161">eq</span></span>|
|<span data-ttu-id="7e50a-162">initiatedBy/user/userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7e50a-162">initiatedBy/user/userPrincipalName</span></span>| <span data-ttu-id="7e50a-163">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="7e50a-163">eq, startswith</span></span>|
|<span data-ttu-id="7e50a-164">clientAppUsed</span><span class="sxs-lookup"><span data-stu-id="7e50a-164">clientAppUsed</span></span>| <span data-ttu-id="7e50a-165">eq</span><span class="sxs-lookup"><span data-stu-id="7e50a-165">eq</span></span>|
|<span data-ttu-id="7e50a-166">conditionalAccessStatus</span><span class="sxs-lookup"><span data-stu-id="7e50a-166">conditionalAccessStatus</span></span> | <span data-ttu-id="7e50a-167">eq</span><span class="sxs-lookup"><span data-stu-id="7e50a-167">eq</span></span>|
|<span data-ttu-id="7e50a-168">deviceDetail/browser</span><span class="sxs-lookup"><span data-stu-id="7e50a-168">deviceDetail/browser</span></span>| <span data-ttu-id="7e50a-169">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="7e50a-169">eq, startswith</span></span>|
|<span data-ttu-id="7e50a-170">deviceDetail/operatingSystem</span><span class="sxs-lookup"><span data-stu-id="7e50a-170">deviceDetail/operatingSystem</span></span>| <span data-ttu-id="7e50a-171">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="7e50a-171">eq, startswith</span></span>|
|<span data-ttu-id="7e50a-172">correlationId</span><span class="sxs-lookup"><span data-stu-id="7e50a-172">correlationId</span></span>| <span data-ttu-id="7e50a-173">eq</span><span class="sxs-lookup"><span data-stu-id="7e50a-173">eq</span></span>|
|<span data-ttu-id="7e50a-174">isrisky</span><span class="sxs-lookup"><span data-stu-id="7e50a-174">isRisky</span></span>| <span data-ttu-id="7e50a-175">eq</span><span class="sxs-lookup"><span data-stu-id="7e50a-175">eq</span></span>|

## <a name="response"></a><span data-ttu-id="7e50a-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e50a-176">Response</span></span>

<span data-ttu-id="7e50a-177">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos de [logon](../resources/signin.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7e50a-177">If successful, this method returns a `200 OK` response code and collection of [signIn](../resources/signin.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e50a-178">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7e50a-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="7e50a-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7e50a-179">Request</span></span>

<span data-ttu-id="7e50a-180">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7e50a-180">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7e50a-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="7e50a-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_signins"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/auditLogs/signIns
```
# <a name="c"></a>[<span data-ttu-id="7e50a-182">C#</span><span class="sxs-lookup"><span data-stu-id="7e50a-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-signins-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7e50a-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7e50a-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-signins-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7e50a-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7e50a-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-signins-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7e50a-185">Java</span><span class="sxs-lookup"><span data-stu-id="7e50a-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-signins-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7e50a-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e50a-186">Response</span></span>

<span data-ttu-id="7e50a-187">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7e50a-187">Here is an example of the response.</span></span>
><span data-ttu-id="7e50a-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7e50a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/auditLogs/signIns?$top=1&$skiptoken=9177f2e3532fcd4c4d225f68f7b9bdf7_1",
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
  "description": "List signIns",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

