---
title: Lista de aplicativos instalados para o usuário
description: Recupere a lista de aplicativos instalados no escopo pessoal do usuário especificado.
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 3cd4dcfdf792818db2d9f25f0ce260da5cf3a3e0
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52038674"
---
# <a name="list-apps-installed-for-user"></a><span data-ttu-id="2a0fc-103">Lista de aplicativos instalados para o usuário</span><span class="sxs-lookup"><span data-stu-id="2a0fc-103">List apps installed for user</span></span>

<span data-ttu-id="2a0fc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a0fc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2a0fc-105">Recupere a lista de [aplicativos](../resources/teamsappinstallation.md) instalados no escopo pessoal do usuário [especificado](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="2a0fc-105">Retrieve the list of [apps](../resources/teamsappinstallation.md) installed in the personal scope of the specified [user](../resources/user.md).</span></span>

> [!NOTE]
> <span data-ttu-id="2a0fc-106">O `id` de um recurso **teamsAppInstallation** não é o mesmo valor que o `id` do recurso **teamsApp** associado.</span><span class="sxs-lookup"><span data-stu-id="2a0fc-106">The `id` of a **teamsAppInstallation** resource is not the same value as the `id` of the associated **teamsApp** resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="2a0fc-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="2a0fc-107">Permissions</span></span>

<span data-ttu-id="2a0fc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a0fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a0fc-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2a0fc-110">Permission type</span></span>      | <span data-ttu-id="2a0fc-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2a0fc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2a0fc-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2a0fc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2a0fc-113">TeamsAppInstallation.ReadForUser, TeamsAppInstallation.ReadWriteSelfForUser, TeamsAppInstallation.ReadWriteForUser</span><span class="sxs-lookup"><span data-stu-id="2a0fc-113">TeamsAppInstallation.ReadForUser, TeamsAppInstallation.ReadWriteSelfForUser, TeamsAppInstallation.ReadWriteForUser</span></span> |
|<span data-ttu-id="2a0fc-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2a0fc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a0fc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2a0fc-115">Not supported.</span></span>    |
|<span data-ttu-id="2a0fc-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2a0fc-116">Application</span></span> | <span data-ttu-id="2a0fc-117">TeamsAppInstallation.ReadForUser.All, TeamsAppInstallation.ReadWriteSelfForUser.All, TeamsAppInstallation.ReadWriteForUser.All</span><span class="sxs-lookup"><span data-stu-id="2a0fc-117">TeamsAppInstallation.ReadForUser.All, TeamsAppInstallation.ReadWriteSelfForUser.All, TeamsAppInstallation.ReadWriteForUser.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2a0fc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2a0fc-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{user-id}/teamwork/installedApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2a0fc-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2a0fc-119">Optional query parameters</span></span>

<span data-ttu-id="2a0fc-120">Este método suporta o `$filter`, `$select`, e `$expand` [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2a0fc-120">This method supports the `$filter`, `$select`, and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2a0fc-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2a0fc-121">Request headers</span></span>

| <span data-ttu-id="2a0fc-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2a0fc-122">Header</span></span>       | <span data-ttu-id="2a0fc-123">Valor</span><span class="sxs-lookup"><span data-stu-id="2a0fc-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2a0fc-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="2a0fc-124">Authorization</span></span>  | <span data-ttu-id="2a0fc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2a0fc-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2a0fc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2a0fc-127">Request body</span></span>

<span data-ttu-id="2a0fc-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2a0fc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2a0fc-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a0fc-129">Response</span></span>

<span data-ttu-id="2a0fc-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/teamsappinstallation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2a0fc-130">If successful, this method returns a `200 OK` response code and a collection of [teamsAppInstallation](../resources/teamsappinstallation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2a0fc-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2a0fc-131">Examples</span></span>

### <a name="example-1-list-apps-installed-for-the-specified-user"></a><span data-ttu-id="2a0fc-132">Exemplo 1: Listar aplicativos instalados para o usuário especificado</span><span class="sxs-lookup"><span data-stu-id="2a0fc-132">Example 1: List apps installed for the specified user</span></span>

#### <a name="request"></a><span data-ttu-id="2a0fc-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2a0fc-133">Request</span></span>

<span data-ttu-id="2a0fc-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2a0fc-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2a0fc-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="2a0fc-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_list_teamsApps_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/5b649834-7412-4cce-9e69-176e95a394f5/teamwork/installedApps
```
# <a name="c"></a>[<span data-ttu-id="2a0fc-136">C#</span><span class="sxs-lookup"><span data-stu-id="2a0fc-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-list-teamsapps-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2a0fc-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2a0fc-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-list-teamsapps-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2a0fc-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2a0fc-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-list-teamsapps-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2a0fc-139">Java</span><span class="sxs-lookup"><span data-stu-id="2a0fc-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-list-teamsapps-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2a0fc-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a0fc-140">Response</span></span>

<span data-ttu-id="2a0fc-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2a0fc-141">The following is an example of the response.</span></span>
><span data-ttu-id="2a0fc-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2a0fc-142">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "name": "user_list_teamsApps_2",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "YTZiNjMzNjUtMzFhNC00ZjQzLTkyZWMtNzEwYjcxNTU3YWY5IyMwLjk="
    }
  ]
}
```

### <a name="example-2-get-the-names-and-other-details-of-apps-installed-for-the-user"></a><span data-ttu-id="2a0fc-143">Exemplo 2: Obter os nomes e outros detalhes dos aplicativos instalados para o usuário</span><span class="sxs-lookup"><span data-stu-id="2a0fc-143">Example 2: Get the names and other details of apps installed for the user</span></span>

#### <a name="request"></a><span data-ttu-id="2a0fc-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2a0fc-144">Request</span></span>

<span data-ttu-id="2a0fc-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2a0fc-145">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2a0fc-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="2a0fc-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_list_teamsApps_details"
} -->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/5b649834-7412-4cce-9e69-176e95a394f5/teamwork/installedApps?$expand=teamsAppDefinition
```
# <a name="c"></a>[<span data-ttu-id="2a0fc-147">C#</span><span class="sxs-lookup"><span data-stu-id="2a0fc-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-list-teamsapps-details-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2a0fc-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2a0fc-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-list-teamsapps-details-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2a0fc-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2a0fc-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-list-teamsapps-details-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2a0fc-150">Java</span><span class="sxs-lookup"><span data-stu-id="2a0fc-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-list-teamsapps-details-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2a0fc-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a0fc-151">Response</span></span>

<span data-ttu-id="2a0fc-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2a0fc-152">The following is an example of the response.</span></span>

><span data-ttu-id="2a0fc-153">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2a0fc-153">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "name": "user_list_teamsApps_details",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMwZDgyMGVjZC1kZWYyLTQyOTctYWRhZC03ODA1NmNkZTdjNzg=",
            "teamsAppDefinition": {
                "id": "MGQ4MjBlY2QtZGVmMi00Mjk3LWFkYWQtNzgwNTZjZGU3Yzc4IyMxLjAuMA==",
                "teamsAppId": "0d820ecd-def2-4297-adad-78056cde7c78",
                "displayName": "OneNote",
                "version": "1.0.0"
            }
        },
        {
            "id": "NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMwZmQ5MjVhMC0zNTdmLTRkMjUtODQ1Ni1iMzAyMmFhYTQxYTk=",
            "teamsAppDefinition": {
                "id": "MGZkOTI1YTAtMzU3Zi00ZDI1LTg0NTYtYjMwMjJhYWE0MWE5IyMxLjc=",
                "teamsAppId": "0fd925a0-357f-4d25-8456-b3022aaa41a9",
                "displayName": "SurveyMonkey",
                "version": "1.7"
            }
        },
        {
            "id": "NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMyYTUyNzcwMy0xZjZmLTQ1NTktYTMzMi1kOGE3ZDI4OGNkODg=",
            "teamsAppDefinition": {
                "id": "MmE1Mjc3MDMtMWY2Zi00NTU5LWEzMzItZDhhN2QyODhjZDg4IyMxLjA=",
                "teamsAppId": "2a527703-1f6f-4559-a332-d8a7d288cd88",
                "displayName": "SharePoint",
                "version": "1.0"
            }
        }
  ]
}
```

### <a name="example-3-get-the-app-installation-resource-based-on-the-manifest-id-of-the-associated-app"></a><span data-ttu-id="2a0fc-154">Exemplo 3: Obter o recurso de instalação do aplicativo com base na ID de manifesto do aplicativo associado</span><span class="sxs-lookup"><span data-stu-id="2a0fc-154">Example 3: Get the app installation resource based on the manifest ID of the associated app</span></span>

#### <a name="request"></a><span data-ttu-id="2a0fc-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2a0fc-155">Request</span></span>

<span data-ttu-id="2a0fc-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2a0fc-156">The following is an example of the request.</span></span> <span data-ttu-id="2a0fc-157">No exemplo, a ID de manifesto do aplicativo Teams é 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'.</span><span class="sxs-lookup"><span data-stu-id="2a0fc-157">In the example, the manifest ID of the Teams app is 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'.</span></span>

# <a name="http"></a>[<span data-ttu-id="2a0fc-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="2a0fc-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_list_teamsApps_details_filter"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/97a5a533-833d-494b-b543-c0afe026cb96/teamwork/installedApps?$expand=teamsApp,teamsAppDefinition&$filter=teamsApp/externalId eq 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'
```
# <a name="c"></a>[<span data-ttu-id="2a0fc-159">C#</span><span class="sxs-lookup"><span data-stu-id="2a0fc-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-list-teamsapps-details-filter-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2a0fc-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2a0fc-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-list-teamsapps-details-filter-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2a0fc-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2a0fc-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-list-teamsapps-details-filter-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2a0fc-162">Java</span><span class="sxs-lookup"><span data-stu-id="2a0fc-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-list-teamsapps-details-filter-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2a0fc-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a0fc-163">Response</span></span>

<span data-ttu-id="2a0fc-164">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2a0fc-164">The following is an example of the response.</span></span>

><span data-ttu-id="2a0fc-165">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2a0fc-165">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "name": "user_list_teamsApps_details_filter",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.count": 1,
    "value": [
        {
            "id": "NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwMjQwYTM2OC0yNWUwLTQ1NjktOGViZS0xMzYwMWNiNTVhMTg=",
            "teamsApp": {
                "id": "0240a368-25e0-4569-8ebe-13601cb55a18",
                "externalId": "cf1ba4c7-f94e-4d80-ba90-5594b641a8ee",
                "displayName": "YPA",
                "distributionMethod": "sideloaded"
            },
            "teamsAppDefinition": {
                "id": "MDI0MGEzNjgtMjVlMC00NTY5LThlYmUtMTM2MDFjYjU1YTE4IyM2LjAuMA==",
                "teamsAppId": "0240a368-25e0-4569-8ebe-13601cb55a18",
                "azureADAppId": "9fc97ea2-c417-4c76-a2db-197612067b28",
                "displayName": "YPA",
                "version": "6.0.0",
                "requiredResourceSpecificApplicationPermissions": [
                ],
                "publishingState": "published",
                "shortDescription": "A conversational smart assistant from MSX that surfaces real-time insights.",
                "description": "For MSX Users: A conversational role-based smart assistant that will enable Enterprise sellers (AE, ATS, SSP, TSP) to be more productive by surfacing real-time insights, recommendations, actions and notifications, and by automating repetitive tasks.",
                "lastModifiedDateTime": null,
                "createdBy": null
            }
        }
    ]
}
```
## <a name="see-also"></a><span data-ttu-id="2a0fc-166">Confira também</span><span class="sxs-lookup"><span data-stu-id="2a0fc-166">See also</span></span>
- [<span data-ttu-id="2a0fc-167">Listar aplicativos no catálogo</span><span class="sxs-lookup"><span data-stu-id="2a0fc-167">List apps in catalog</span></span>](appcatalogs-list-teamsapps.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "User list teamsAppInstallations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
