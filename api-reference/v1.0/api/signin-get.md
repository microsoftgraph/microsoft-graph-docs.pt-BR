---
title: Obter entrada
description: Descreve o método get do recurso signIn (entidade) da API Graph Microsoft.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: 6c5e3f215409e065ce6548e59827beb8ae1eafdf
ms.sourcegitcommit: 8a9be6f65f62f29973508d82e0348d4142c18f23
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2021
ms.locfileid: "53129458"
---
# <a name="get-signin"></a><span data-ttu-id="215a5-103">Obter entrada</span><span class="sxs-lookup"><span data-stu-id="215a5-103">Get signIn</span></span>

<span data-ttu-id="215a5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="215a5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="215a5-105">Recupere um evento específico de entrada do Azure AD para seu locatário.</span><span class="sxs-lookup"><span data-stu-id="215a5-105">Retrieve a specific Azure AD user sign-in event for your tenant.</span></span> <span data-ttu-id="215a5-106">As inserções interativas de natureza (onde um nome de usuário/senha é passado como parte do token de autenticação) e as inserções federadas bem-sucedidas estão atualmente incluídas nos logs de login.</span><span class="sxs-lookup"><span data-stu-id="215a5-106">Sign-ins that are interactive in nature (where a username/password is passed as part of auth token) and successful federated sign-ins are currently included in the sign-in logs.</span></span>

## <a name="permissions"></a><span data-ttu-id="215a5-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="215a5-107">Permissions</span></span>

<span data-ttu-id="215a5-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="215a5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="215a5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="215a5-110">Permission type</span></span>      | <span data-ttu-id="215a5-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="215a5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="215a5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="215a5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="215a5-113">AuditLog.Read.All e Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="215a5-113">AuditLog.Read.All and Directory.Read.All</span></span> |
|<span data-ttu-id="215a5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="215a5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="215a5-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="215a5-115">Not supported</span></span>   |
|<span data-ttu-id="215a5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="215a5-116">Application</span></span> | <span data-ttu-id="215a5-117">AuditLog.Read.All e Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="215a5-117">AuditLog.Read.All and Directory.Read.All</span></span> |

<span data-ttu-id="215a5-118">Os aplicativos devem [estar registrados corretamente](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="215a5-118">Apps must be [properly registered](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to Azure AD.</span></span>

<span data-ttu-id="215a5-119">Além das permissões delegadas, o usuário inscreveu precisa pertencer a uma das seguintes funções de diretório que permitem ler relatórios de logons.</span><span class="sxs-lookup"><span data-stu-id="215a5-119">In addition to the delegated permissions, the signed-in user needs to belong to one of the following directory roles that allow them to read sign-in reports.</span></span> <span data-ttu-id="215a5-120">Para saber mais sobre funções de diretório, consulte Funções do [Azure AD integrados](/azure/active-directory/roles/permissions-reference):</span><span class="sxs-lookup"><span data-stu-id="215a5-120">To learn more about directory roles, see [Azure AD built-in roles](/azure/active-directory/roles/permissions-reference):</span></span>
+ <span data-ttu-id="215a5-121">Administrador global</span><span class="sxs-lookup"><span data-stu-id="215a5-121">Global Administrator</span></span>
+ <span data-ttu-id="215a5-122">Leitor global</span><span class="sxs-lookup"><span data-stu-id="215a5-122">Global Reader</span></span>
+ <span data-ttu-id="215a5-123">Leitor de Relatórios</span><span class="sxs-lookup"><span data-stu-id="215a5-123">Reports Reader</span></span>
+ <span data-ttu-id="215a5-124">Administrador de Segurança</span><span class="sxs-lookup"><span data-stu-id="215a5-124">Security Administrator</span></span>
+ <span data-ttu-id="215a5-125">Operador de segurança</span><span class="sxs-lookup"><span data-stu-id="215a5-125">Security Operator</span></span>
+ <span data-ttu-id="215a5-126">Leitor de segurança</span><span class="sxs-lookup"><span data-stu-id="215a5-126">Security Reader</span></span>

## <a name="http-request"></a><span data-ttu-id="215a5-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="215a5-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /auditLogs/signIns/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="215a5-128">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="215a5-128">Optional query parameters</span></span>

<span data-ttu-id="215a5-129">Este método dá suporte a Parâmetros de consulta do OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="215a5-129">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="215a5-130">Para obter detalhes sobre como usar esses parâmetros, confira [Parâmetros de consulta do OData](/graph/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="215a5-130">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="215a5-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="215a5-131">Request headers</span></span>

| <span data-ttu-id="215a5-132">Nome</span><span class="sxs-lookup"><span data-stu-id="215a5-132">Name</span></span>      |<span data-ttu-id="215a5-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="215a5-133">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="215a5-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="215a5-134">Authorization</span></span>  | <span data-ttu-id="215a5-135">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="215a5-135">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="215a5-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="215a5-136">Request body</span></span>

<span data-ttu-id="215a5-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="215a5-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="215a5-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="215a5-138">Response</span></span>

<span data-ttu-id="215a5-139">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [signIn](../resources/signin.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="215a5-139">If successful, this method returns a `200 OK` response code and [signIn](../resources/signin.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="215a5-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="215a5-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="215a5-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="215a5-141">Request</span></span>

<span data-ttu-id="215a5-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="215a5-142">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="215a5-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="215a5-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/auditLogs/signIns/66ea54eb-6301-4ee5-be62-ff5a759b0100
```
# <a name="c"></a>[<span data-ttu-id="215a5-144">C#</span><span class="sxs-lookup"><span data-stu-id="215a5-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="215a5-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="215a5-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="215a5-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="215a5-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="215a5-147">Java</span><span class="sxs-lookup"><span data-stu-id="215a5-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="215a5-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="215a5-148">Response</span></span>

<span data-ttu-id="215a5-149">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="215a5-149">Here is an example of the response.</span></span>
><span data-ttu-id="215a5-150">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="215a5-150">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.signIn"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#auditLogs/signIns",
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
  "description": "Get signIn",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

