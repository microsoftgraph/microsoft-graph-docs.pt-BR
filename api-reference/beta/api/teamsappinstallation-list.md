---
title: Listar aplicativos em equipe
description: Recupere a lista de aplicativos instalados na equipe especificada.
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: ab4c453b289165a24afcc8d19244e31263abf3d4
ms.sourcegitcommit: 82b73552fff79a4ef7a2ee57fc2d1b3286b5bd4c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/26/2019
ms.locfileid: "35908352"
---
# <a name="list-apps-in-team"></a><span data-ttu-id="7fe09-103">Listar aplicativos em equipe</span><span class="sxs-lookup"><span data-stu-id="7fe09-103">List apps in team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7fe09-104">Recupere a lista de [aplicativos instalados](../resources/teamsappinstallation.md) na [equipe](../resources/team.md)especificada.</span><span class="sxs-lookup"><span data-stu-id="7fe09-104">Retrieve the list of [apps installed](../resources/teamsappinstallation.md) in the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7fe09-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="7fe09-105">Permissions</span></span>

<span data-ttu-id="7fe09-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7fe09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7fe09-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7fe09-108">Permission type</span></span>      | <span data-ttu-id="7fe09-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7fe09-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7fe09-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7fe09-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7fe09-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7fe09-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7fe09-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7fe09-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7fe09-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7fe09-113">Not supported.</span></span>    |
|<span data-ttu-id="7fe09-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7fe09-114">Application</span></span> | <span data-ttu-id="7fe09-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7fe09-115">Group.Read.All, Group.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="7fe09-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7fe09-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/installedApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7fe09-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7fe09-117">Optional query parameters</span></span>

<span data-ttu-id="7fe09-118">Este método oferece suporte a $filter, $select e $expand [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7fe09-118">This method supports the $filter, $select, and $expand [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7fe09-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7fe09-119">Request headers</span></span>

| <span data-ttu-id="7fe09-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7fe09-120">Header</span></span>       | <span data-ttu-id="7fe09-121">Valor</span><span class="sxs-lookup"><span data-stu-id="7fe09-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7fe09-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7fe09-122">Authorization</span></span>  | <span data-ttu-id="7fe09-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7fe09-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7fe09-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7fe09-125">Request body</span></span>

<span data-ttu-id="7fe09-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7fe09-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7fe09-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="7fe09-127">Response</span></span>

<span data-ttu-id="7fe09-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [teamsAppInstallation](../resources/teamsappinstallation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7fe09-128">If successful, this method returns a `200 OK` response code and collection of [teamsAppInstallation](../resources/teamsappinstallation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7fe09-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7fe09-129">Examples</span></span>

### <a name="example-1-list-installed-apps"></a><span data-ttu-id="7fe09-130">Exemplo 1: listar aplicativos instalados</span><span class="sxs-lookup"><span data-stu-id="7fe09-130">Example 1: List installed apps</span></span>

#### <a name="request"></a><span data-ttu-id="7fe09-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7fe09-131">Request</span></span>

<span data-ttu-id="7fe09-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7fe09-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7fe09-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="7fe09-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_installed_teams_apps"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/installedApps
```

# <a name="ctabcsharp"></a>[<span data-ttu-id="7fe09-134">C#</span><span class="sxs-lookup"><span data-stu-id="7fe09-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-installed-teams-apps-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7fe09-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="7fe09-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-installed-teams-apps-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7fe09-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="7fe09-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-installed-teams-apps-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7fe09-137">Java</span><span class="sxs-lookup"><span data-stu-id="7fe09-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-installed-teams-apps-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="7fe09-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="7fe09-138">Response</span></span>

<span data-ttu-id="7fe09-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7fe09-139">The following is an example of the response.</span></span>
><span data-ttu-id="7fe09-140">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7fe09-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7fe09-141">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7fe09-141">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_installed_teams_apps",
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
      "id": "id-value"
    }
  ]
}
```

### <a name="example-2-get-the-names-and-other-details-of-installed-apps"></a><span data-ttu-id="7fe09-142">Exemplo 2: obter os nomes e outros detalhes dos aplicativos instalados</span><span class="sxs-lookup"><span data-stu-id="7fe09-142">Example 2: Get the names and other details of installed apps</span></span>

#### <a name="request"></a><span data-ttu-id="7fe09-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7fe09-143">Request</span></span>

<span data-ttu-id="7fe09-144">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7fe09-144">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7fe09-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="7fe09-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_installed_teams_apps_expand"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/installedApps?$expand=teamsAppDefinition
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7fe09-146">C#</span><span class="sxs-lookup"><span data-stu-id="7fe09-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-installed-teams-apps-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7fe09-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="7fe09-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-installed-teams-apps-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7fe09-148">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="7fe09-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-installed-teams-apps-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7fe09-149">Java</span><span class="sxs-lookup"><span data-stu-id="7fe09-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-installed-teams-apps-expand-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7fe09-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="7fe09-150">Response</span></span>

<span data-ttu-id="7fe09-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7fe09-151">The following is an example of the response.</span></span>

><span data-ttu-id="7fe09-152">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7fe09-152">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7fe09-153">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7fe09-153">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_installed_teams_apps_expand",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
