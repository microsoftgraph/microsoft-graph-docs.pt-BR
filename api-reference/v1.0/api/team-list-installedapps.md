---
title: Listar aplicativos em equipe
description: Recupere uma lista de aplicativos instalados na equipe especificada.
author: akjo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7daf041f27697a99c23ad0dc16c861ea6a8ef10c
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060551"
---
# <a name="list-apps-in-team"></a><span data-ttu-id="c5849-103">Listar aplicativos em equipe</span><span class="sxs-lookup"><span data-stu-id="c5849-103">List apps in team</span></span>

<span data-ttu-id="c5849-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5849-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c5849-105">Recupere uma lista de [aplicativos instalados](../resources/teamsappinstallation.md) na equipe [especificada.](../resources/team.md)</span><span class="sxs-lookup"><span data-stu-id="c5849-105">Retrieve a list of [apps installed](../resources/teamsappinstallation.md) in the specified [team](../resources/team.md).</span></span>


> [!NOTE]
> <span data-ttu-id="c5849-106">O `id` de um recurso **teamsAppInstallation** não é o mesmo valor que o `id` do recurso **teamsApp** associado.</span><span class="sxs-lookup"><span data-stu-id="c5849-106">The `id` of a **teamsAppInstallation** resource is not the same value as the `id` of the associated **teamsApp** resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="c5849-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="c5849-107">Permissions</span></span>

<span data-ttu-id="c5849-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5849-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5849-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c5849-110">Permission type</span></span>      | <span data-ttu-id="c5849-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c5849-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5849-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c5849-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c5849-113">TeamsAppInstallation.ReadForTeam, TeamsAppInstallation.ReadWriteForTeam, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5849-113">TeamsAppInstallation.ReadForTeam, TeamsAppInstallation.ReadWriteForTeam, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="c5849-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c5849-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5849-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5849-115">Not supported.</span></span>    |
|<span data-ttu-id="c5849-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c5849-116">Application</span></span> | <span data-ttu-id="c5849-117">TeamsAppInstallation.Read.Group\*, TeamsAppInstallation.ReadForTeam.All, TeamsAppInstallation.ReadWriteForTeam.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5849-117">TeamsAppInstallation.Read.Group\*, TeamsAppInstallation.ReadForTeam.All, TeamsAppInstallation.ReadWriteForTeam.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="c5849-118">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="c5849-118">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

## <a name="http-request"></a><span data-ttu-id="c5849-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c5849-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{team-id}/installedApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c5849-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c5849-120">Optional query parameters</span></span>

<span data-ttu-id="c5849-121">Este método dá suporte `$filter` aos `$select` parâmetros , e `$expand` [OData Query para](/graph/query-parameters) ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c5849-121">This method supports the `$filter`, `$select`, and `$expand` [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c5849-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c5849-122">Request headers</span></span>

| <span data-ttu-id="c5849-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c5849-123">Header</span></span>       | <span data-ttu-id="c5849-124">Valor</span><span class="sxs-lookup"><span data-stu-id="c5849-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c5849-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="c5849-125">Authorization</span></span>  | <span data-ttu-id="c5849-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c5849-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c5849-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c5849-128">Request body</span></span>

<span data-ttu-id="c5849-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c5849-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5849-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5849-130">Response</span></span>

<span data-ttu-id="c5849-131">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [teamsAppInstallation](../resources/teamsappinstallation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c5849-131">If successful, this method returns a `200 OK` response code and collection of [teamsAppInstallation](../resources/teamsappinstallation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c5849-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c5849-132">Examples</span></span>

### <a name="example-1-list-installed-apps"></a><span data-ttu-id="c5849-133">Exemplo 1: Listar aplicativos instalados</span><span class="sxs-lookup"><span data-stu-id="c5849-133">Example 1: List installed apps</span></span>
#### <a name="request"></a><span data-ttu-id="c5849-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c5849-134">Request</span></span>

<span data-ttu-id="c5849-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c5849-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c5849-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="c5849-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_installed_apps_in_team"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/6903fa93-605b-43ef-920e-77c4729f8258/installedApps
```
# <a name="c"></a>[<span data-ttu-id="c5849-137">C#</span><span class="sxs-lookup"><span data-stu-id="c5849-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-installed-apps-in-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c5849-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c5849-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-installed-apps-in-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c5849-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c5849-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-installed-apps-in-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c5849-140">Java</span><span class="sxs-lookup"><span data-stu-id="c5849-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-installed-apps-in-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c5849-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5849-141">Response</span></span>

<span data-ttu-id="c5849-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c5849-142">The following is an example of the response.</span></span>
><span data-ttu-id="c5849-143">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c5849-143">**Note:** The response object shown here might be shortened for readability.</span></span>
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
   "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#teams('6903fa93-605b-43ef-920e-77c4729f8258')/installedApps",
   "@odata.count":3,
   "value":[
      {
         "id":"NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwMDAwMTAxNi1kZTA1LTQ5MmUtOTEwNi00ODI4ZmM4YTg2ODc="
      },
      {
         "id":"NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwYWUzNWIzNi0wZmQ3LTQyMmUtODA1Yi1kNTNhZjE1NzkwOTM="
      },
      {
         "id":"NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwZDgyMGVjZC1kZWYyLTQyOTctYWRhZC03ODA1NmNkZTdjNzg="
      }
   ]
}
```

### <a name="example-2-get-the-names-and-other-details-of-installed-apps"></a><span data-ttu-id="c5849-144">Exemplo 2: Obter os nomes e outros detalhes de aplicativos instalados</span><span class="sxs-lookup"><span data-stu-id="c5849-144">Example 2: Get the names and other details of installed apps</span></span>

#### <a name="request"></a><span data-ttu-id="c5849-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c5849-145">Request</span></span>

<span data-ttu-id="c5849-146">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c5849-146">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c5849-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="c5849-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_installed_teams_apps_expand"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/6903fa93-605b-43ef-920e-77c4729f8258/installedApps?$expand=teamsAppDefinition
```
# <a name="c"></a>[<span data-ttu-id="c5849-148">C#</span><span class="sxs-lookup"><span data-stu-id="c5849-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-installed-teams-apps-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c5849-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c5849-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-installed-teams-apps-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c5849-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c5849-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-installed-teams-apps-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c5849-151">Java</span><span class="sxs-lookup"><span data-stu-id="c5849-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-installed-teams-apps-expand-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c5849-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5849-152">Response</span></span>

<span data-ttu-id="c5849-153">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c5849-153">The following is an example of the response.</span></span>

><span data-ttu-id="c5849-154">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c5849-154">**Note:** The response object shown here might be shortened for readability.</span></span>
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
   "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#teams('6903fa93-605b-43ef-920e-77c4729f8258')/installedApps(teamsAppDefinition())",
   "@odata.count":3,
   "value":[
      {
         "id":"NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwMDAwMTAxNi1kZTA1LTQ5MmUtOTEwNi00ODI4ZmM4YTg2ODc=",
         "teamsAppDefinition":{
            "id":"MDAwMDEwMTYtZGUwNS00OTJlLTkxMDYtNDgyOGZjOGE4Njg3IyMxLjAuMg==",
            "teamsAppId":"00001016-de05-492e-9106-4828fc8a8687",
            "azureADAppId":"7df0a125-d3be-4c96-aa54-591f83ff541c",
            "displayName":"Power Automate Actions",
            "version":"1.0.2",
            "requiredResourceSpecificApplicationPermissions":[
               
            ],
            "publishingState":"published",
            "shortDescription":"Be more productive with Microsoft Flow",
            "description":"Automate time-consuming and repetitive tasks by integrating your favorite apps and services with Microsoft Power Automate.",
            "lastModifiedDateTime":null,
            "createdBy":null
         }
      },
      {
         "id":"NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwYWUzNWIzNi0wZmQ3LTQyMmUtODA1Yi1kNTNhZjE1NzkwOTM=",
         "teamsAppDefinition":{
            "id":"MGFlMzViMzYtMGZkNy00MjJlLTgwNWItZDUzYWYxNTc5MDkzIyMxLjI=",
            "teamsAppId":"0ae35b36-0fd7-422e-805b-d53af1579093",
            "azureADAppId":"00000003-0000-0ff1-ce00-000000000000",
            "displayName":"SharePoint Pages",
            "version":"1.2",
            "requiredResourceSpecificApplicationPermissions":[
               
            ],
            "publishingState":"published",
            "shortDescription":"Add a tab for a SharePoint news article or page.",
            "description":"This app allows you to tab intranet pages from any SharePoint site so that they can be viewed by your team inside Teams channels.",
            "lastModifiedDateTime":null,
            "createdBy":null
         }
      },
      {
         "id":"NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwZDgyMGVjZC1kZWYyLTQyOTctYWRhZC03ODA1NmNkZTdjNzg=",
         "teamsAppDefinition":{
            "id":"MGQ4MjBlY2QtZGVmMi00Mjk3LWFkYWQtNzgwNTZjZGU3Yzc4IyMxLjAuMA==",
            "teamsAppId":"0d820ecd-def2-4297-adad-78056cde7c78",
            "azureADAppId":"2d4d3d8e-2be3-4bef-9f87-7875a61c29de",
            "displayName":"OneNote",
            "version":"1.0.0",
            "requiredResourceSpecificApplicationPermissions":[
               
            ],
            "publishingState":"published",
            "shortDescription":"Capture and share ideas, to-do lists and other notes with your team.",
            "description":"Capture and share ideas, to-do lists and other thoughts with your team. You can also co-author anytime.",
            "lastModifiedDateTime":null,
            "createdBy":null
         }
      }
   ]
}
```

### <a name="example-3-get-the-app-installation-resource-based-on-the-manifest-id-of-the-associated-app"></a><span data-ttu-id="c5849-155">Exemplo 3: Obter o recurso de instalação do aplicativo com base na ID de manifesto do aplicativo associado</span><span class="sxs-lookup"><span data-stu-id="c5849-155">Example 3: Get the app installation resource based on the manifest ID of the associated app</span></span>

#### <a name="request"></a><span data-ttu-id="c5849-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c5849-156">Request</span></span>

<span data-ttu-id="c5849-157">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c5849-157">The following is an example of the request.</span></span> <span data-ttu-id="c5849-158">No exemplo, a ID de manifesto do aplicativo Teams é 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'.</span><span class="sxs-lookup"><span data-stu-id="c5849-158">In the example, the manifest ID of the Teams app is 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'.</span></span>

# <a name="http"></a>[<span data-ttu-id="c5849-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="c5849-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_installed_apps_in_team_expand_filter_externalid"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/acda442c-78d2-491b-8204-4ef5019c0193/installedApps?$expand=teamsApp,teamsAppDefinition&$filter=teamsApp/externalId eq 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'
```
# <a name="c"></a>[<span data-ttu-id="c5849-160">C#</span><span class="sxs-lookup"><span data-stu-id="c5849-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-installed-apps-in-team-expand-filter-externalid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c5849-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c5849-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-installed-apps-in-team-expand-filter-externalid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c5849-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c5849-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-installed-apps-in-team-expand-filter-externalid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c5849-163">Java</span><span class="sxs-lookup"><span data-stu-id="c5849-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-installed-apps-in-team-expand-filter-externalid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c5849-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5849-164">Response</span></span>

<span data-ttu-id="c5849-165">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c5849-165">The following is an example of the response.</span></span>

><span data-ttu-id="c5849-166">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c5849-166">**Note:** The response object shown here might be shortened for readability.</span></span>
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
   "@odata.count":1,
   "value":[
      {
         "id":"NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwMjQwYTM2OC0yNWUwLTQ1NjktOGViZS0xMzYwMWNiNTVhMTg=",
         "teamsApp":{
            "id":"0240a368-25e0-4569-8ebe-13601cb55a18",
            "externalId":"cf1ba4c7-f94e-4d80-ba90-5594b641a8ee",
            "displayName":"YPA",
            "distributionMethod":"sideloaded"
         },
         "teamsAppDefinition":{
            "id":"MDI0MGEzNjgtMjVlMC00NTY5LThlYmUtMTM2MDFjYjU1YTE4IyM2LjAuMA==",
            "teamsAppId":"0240a368-25e0-4569-8ebe-13601cb55a18",
            "azureADAppId":"9fc97ea2-c417-4c76-a2db-197612067b28",
            "displayName":"YPA",
            "version":"6.0.0",
            "requiredResourceSpecificApplicationPermissions":[
               
            ],
            "publishingState":"published",
            "shortDescription":"A conversational smart assistant from MSX that surfaces real-time insights.",
            "description":"For MSX Users: A conversational role-based smart assistant that will enable Enterprise sellers (AE, ATS, SSP, TSP) to be more productive by surfacing real-time insights, recommendations, actions and notifications, and by automating repetitive tasks.",
            "lastModifiedDateTime":null,
            "createdBy":null
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

## <a name="see-also"></a><span data-ttu-id="c5849-167">Confira também</span><span class="sxs-lookup"><span data-stu-id="c5849-167">See also</span></span>
- [<span data-ttu-id="c5849-168">Listar aplicativos no catálogo</span><span class="sxs-lookup"><span data-stu-id="c5849-168">List apps in catalog</span></span>](appcatalogs-list-teamsapps.md)
