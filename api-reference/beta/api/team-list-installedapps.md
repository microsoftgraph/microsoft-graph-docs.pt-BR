---
title: Listar aplicativos em equipe
description: Recupere a lista de aplicativos instalados na equipe especificada.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 870e36160830cd38272791861527bfea2aca2645
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49690715"
---
# <a name="list-apps-in-team"></a><span data-ttu-id="9dfa5-103">Listar aplicativos em equipe</span><span class="sxs-lookup"><span data-stu-id="9dfa5-103">List apps in team</span></span>

<span data-ttu-id="9dfa5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9dfa5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9dfa5-105">Recupere a lista de [aplicativos instalados](../resources/teamsappinstallation.md) na [equipe](../resources/team.md)especificada.</span><span class="sxs-lookup"><span data-stu-id="9dfa5-105">Retrieve the list of [apps installed](../resources/teamsappinstallation.md) in the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9dfa5-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="9dfa5-106">Permissions</span></span>

<span data-ttu-id="9dfa5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9dfa5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9dfa5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9dfa5-109">Permission type</span></span>      | <span data-ttu-id="9dfa5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9dfa5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9dfa5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9dfa5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9dfa5-112">TeamsAppInstallation. ReadForTeam, TeamsAppInstallation. ReadWriteForTeam, Group. Read. All, Group. ReadWrite. All, Directory. Read. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="9dfa5-112">TeamsAppInstallation.ReadForTeam, TeamsAppInstallation.ReadWriteForTeam, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="9dfa5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9dfa5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9dfa5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9dfa5-114">Not supported.</span></span>    |
|<span data-ttu-id="9dfa5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9dfa5-115">Application</span></span> | <span data-ttu-id="9dfa5-116">TeamsAppInstallation. Read. Group \*, TeamsAppInstallation. ReadForTeam. All, TeamsAppInstallation. ReadWriteForTeam. All, Group. Read. All, Group. ReadWrite. All, Directory. Read. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="9dfa5-116">TeamsAppInstallation.Read.Group\*, TeamsAppInstallation.ReadForTeam.All, TeamsAppInstallation.ReadWriteForTeam.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="9dfa5-117">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="9dfa5-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

## <a name="http-request"></a><span data-ttu-id="9dfa5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9dfa5-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{team-id}/installedApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9dfa5-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9dfa5-119">Optional query parameters</span></span>

<span data-ttu-id="9dfa5-120">Este método suporta o `$filter`, `$select`, e `$expand` [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9dfa5-120">This method supports the `$filter`, `$select`, and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9dfa5-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9dfa5-121">Request headers</span></span>

| <span data-ttu-id="9dfa5-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9dfa5-122">Header</span></span>       | <span data-ttu-id="9dfa5-123">Valor</span><span class="sxs-lookup"><span data-stu-id="9dfa5-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9dfa5-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="9dfa5-124">Authorization</span></span>  | <span data-ttu-id="9dfa5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9dfa5-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9dfa5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9dfa5-127">Request body</span></span>

<span data-ttu-id="9dfa5-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9dfa5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9dfa5-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="9dfa5-129">Response</span></span>

<span data-ttu-id="9dfa5-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [teamsAppInstallation](../resources/teamsappinstallation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9dfa5-130">If successful, this method returns a `200 OK` response code and collection of [teamsAppInstallation](../resources/teamsappinstallation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9dfa5-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9dfa5-131">Examples</span></span>

### <a name="example-1-list-installed-apps"></a><span data-ttu-id="9dfa5-132">Exemplo 1: listar aplicativos instalados</span><span class="sxs-lookup"><span data-stu-id="9dfa5-132">Example 1: List installed apps</span></span>
#### <a name="request"></a><span data-ttu-id="9dfa5-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9dfa5-133">Request</span></span>

<span data-ttu-id="9dfa5-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9dfa5-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9dfa5-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="9dfa5-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_installed_apps_in_team"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/6903fa93-605b-43ef-920e-77c4729f8258/installedApps
```
# <a name="c"></a>[<span data-ttu-id="9dfa5-136">C#</span><span class="sxs-lookup"><span data-stu-id="9dfa5-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-installed-apps-in-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9dfa5-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9dfa5-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-installed-apps-in-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9dfa5-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9dfa5-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-installed-apps-in-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9dfa5-139">Java</span><span class="sxs-lookup"><span data-stu-id="9dfa5-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-installed-apps-in-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9dfa5-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="9dfa5-140">Response</span></span>

<span data-ttu-id="9dfa5-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9dfa5-141">The following is an example of the response.</span></span>
><span data-ttu-id="9dfa5-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9dfa5-142">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "name": "list_installed_apps_in_team",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('6903fa93-605b-43ef-920e-77c4729f8258')/installedApps",
    "@odata.count": 3,
    "value": [
        {
            "id": "NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwMDAwMTAxNi1kZTA1LTQ5MmUtOTEwNi00ODI4ZmM4YTg2ODc="
        },
        {
            "id": "NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwYWUzNWIzNi0wZmQ3LTQyMmUtODA1Yi1kNTNhZjE1NzkwOTM="
        },
        {
            "id": "NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwZDgyMGVjZC1kZWYyLTQyOTctYWRhZC03ODA1NmNkZTdjNzg="
        }
  ]
}
```

### <a name="example-2-get-the-names-and-other-details-of-installed-apps"></a><span data-ttu-id="9dfa5-143">Exemplo 2: obter os nomes e outros detalhes dos aplicativos instalados</span><span class="sxs-lookup"><span data-stu-id="9dfa5-143">Example 2: Get the names and other details of installed apps</span></span>

#### <a name="request"></a><span data-ttu-id="9dfa5-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9dfa5-144">Request</span></span>

<span data-ttu-id="9dfa5-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9dfa5-145">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9dfa5-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="9dfa5-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_installed_teams_apps_expand"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/6903fa93-605b-43ef-920e-77c4729f8258/installedApps?$expand=teamsAppDefinition
```
# <a name="c"></a>[<span data-ttu-id="9dfa5-147">C#</span><span class="sxs-lookup"><span data-stu-id="9dfa5-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-installed-teams-apps-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9dfa5-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9dfa5-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-installed-teams-apps-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9dfa5-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9dfa5-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-installed-teams-apps-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9dfa5-150">Java</span><span class="sxs-lookup"><span data-stu-id="9dfa5-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-installed-teams-apps-expand-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9dfa5-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="9dfa5-151">Response</span></span>

<span data-ttu-id="9dfa5-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9dfa5-152">The following is an example of the response.</span></span>

><span data-ttu-id="9dfa5-153">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9dfa5-153">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "name": "list_installed_teams_apps_expand",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('6903fa93-605b-43ef-920e-77c4729f8258')/installedApps(teamsAppDefinition())",
    "@odata.count": 3,
    "value": [
        {
            "id": "NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwMDAwMTAxNi1kZTA1LTQ5MmUtOTEwNi00ODI4ZmM4YTg2ODc=",
            "teamsAppDefinition": {
                "id": "MDAwMDEwMTYtZGUwNS00OTJlLTkxMDYtNDgyOGZjOGE4Njg3IyMxLjAuMg==",
                "teamsAppId": "00001016-de05-492e-9106-4828fc8a8687",
                "azureADAppId": "7df0a125-d3be-4c96-aa54-591f83ff541c",
                "displayName": "Power Automate Actions",
                "version": "1.0.2",
                "requiredResourceSpecificApplicationPermissions": [],
                "publishingState": "published",
                "shortdescription": "Be more productive with Microsoft Flow",
                "description": "Automate time-consuming and repetitive tasks by integrating your favorite apps and services with Microsoft Power Automate.",
                "lastModifiedDateTime": null,
                "createdBy": null
            }
        },
        {
            "id": "NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwYWUzNWIzNi0wZmQ3LTQyMmUtODA1Yi1kNTNhZjE1NzkwOTM=",
            "teamsAppDefinition": {
                "id": "MGFlMzViMzYtMGZkNy00MjJlLTgwNWItZDUzYWYxNTc5MDkzIyMxLjI=",
                "teamsAppId": "0ae35b36-0fd7-422e-805b-d53af1579093",
                "azureADAppId": "00000003-0000-0ff1-ce00-000000000000",
                "displayName": "SharePoint Pages",
                "version": "1.2",
                "requiredResourceSpecificApplicationPermissions": [],
                "publishingState": "published",
                "shortdescription": "Add a tab for a SharePoint news article or page.",
                "description": "This app allows you to tab intranet pages from any SharePoint site so that they can be viewed by your team inside Teams channels.",
                "lastModifiedDateTime": null,
                "createdBy": null
            }
        },
        {
            "id": "NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwZDgyMGVjZC1kZWYyLTQyOTctYWRhZC03ODA1NmNkZTdjNzg=",
            "teamsAppDefinition": {
                "id": "MGQ4MjBlY2QtZGVmMi00Mjk3LWFkYWQtNzgwNTZjZGU3Yzc4IyMxLjAuMA==",
                "teamsAppId": "0d820ecd-def2-4297-adad-78056cde7c78",
                "azureADAppId": "2d4d3d8e-2be3-4bef-9f87-7875a61c29de",
                "displayName": "OneNote",
                "version": "1.0.0",
                "requiredResourceSpecificApplicationPermissions": [],
                "publishingState": "published",
                "shortdescription": "Capture and share ideas, to-do lists and other notes with your team.",
                "description": "Capture and share ideas, to-do lists and other thoughts with your team. You can also co-author anytime.",
                "lastModifiedDateTime": null,
                "createdBy": null
            }
        }
  ]
}
```

### <a name="example-3-get-the-app-installation-resource-based-on-the-manifest-id-of-the-associated-app"></a><span data-ttu-id="9dfa5-154">Exemplo 3: obter o recurso de instalação de aplicativo com base na ID de manifesto do aplicativo associado</span><span class="sxs-lookup"><span data-stu-id="9dfa5-154">Example 3: Get the app installation resource based on the manifest ID of the associated app</span></span>

#### <a name="request"></a><span data-ttu-id="9dfa5-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9dfa5-155">Request</span></span>

<span data-ttu-id="9dfa5-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9dfa5-156">The following is an example of the request.</span></span> <span data-ttu-id="9dfa5-157">No exemplo, a ID de manifesto do aplicativo Teams é `cf1ba4c7-f94e-4d80-ba90-5594b641a8ee` .</span><span class="sxs-lookup"><span data-stu-id="9dfa5-157">In the example, the manifest ID of the Teams app is `cf1ba4c7-f94e-4d80-ba90-5594b641a8ee`.</span></span>

# <a name="http"></a>[<span data-ttu-id="9dfa5-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="9dfa5-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_installed_apps_in_team_expand_filter_externalid"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/acda442c-78d2-491b-8204-4ef5019c0193/installedApps?$expand=teamsApp,teamsAppDefinition&$filter=teamsApp/externalId eq 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'
```
# <a name="c"></a>[<span data-ttu-id="9dfa5-159">C#</span><span class="sxs-lookup"><span data-stu-id="9dfa5-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-installed-apps-in-team-expand-filter-externalid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9dfa5-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9dfa5-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-installed-apps-in-team-expand-filter-externalid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9dfa5-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9dfa5-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-installed-apps-in-team-expand-filter-externalid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9dfa5-162">Java</span><span class="sxs-lookup"><span data-stu-id="9dfa5-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-installed-apps-in-team-expand-filter-externalid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9dfa5-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="9dfa5-163">Response</span></span>

<span data-ttu-id="9dfa5-164">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9dfa5-164">The following is an example of the response.</span></span>

><span data-ttu-id="9dfa5-165">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9dfa5-165">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "name": "list_installed_apps_in_team_expand_filter_externalid",
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
                "shortdescription": "A conversational smart assistant from MSX that surfaces real-time insights.",
                "description": "For MSX Users: A conversational role-based smart assistant that will enable Enterprise sellers (AE, ATS, SSP, TSP) to be more productive by surfacing real-time insights, recommendations, actions and notifications, and by automating repetitive tasks.",
                "lastModifiedDateTime": null,
                "createdBy": null
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

