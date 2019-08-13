---
title: Listar aplicativos em equipe
description: Recupere a lista de aplicativos instalados na equipe especificada.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: d0679985448af9b18b32dc3298fb7cff92df925e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36362843"
---
# <a name="list-apps-in-team"></a><span data-ttu-id="327aa-103">Listar aplicativos em equipe</span><span class="sxs-lookup"><span data-stu-id="327aa-103">List apps in team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="327aa-104">Recupere a lista de [aplicativos instalados](../resources/teamsappinstallation.md) na [equipe](../resources/team.md)especificada.</span><span class="sxs-lookup"><span data-stu-id="327aa-104">Retrieve the list of [apps installed](../resources/teamsappinstallation.md) in the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="327aa-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="327aa-105">Permissions</span></span>

<span data-ttu-id="327aa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="327aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="327aa-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="327aa-108">Permission type</span></span>      | <span data-ttu-id="327aa-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="327aa-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="327aa-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="327aa-110">Delegated (work or school account)</span></span> | <span data-ttu-id="327aa-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="327aa-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="327aa-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="327aa-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="327aa-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="327aa-113">Not supported.</span></span>    |
|<span data-ttu-id="327aa-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="327aa-114">Application</span></span> | <span data-ttu-id="327aa-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="327aa-115">Group.Read.All, Group.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="327aa-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="327aa-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/installedApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="327aa-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="327aa-117">Optional query parameters</span></span>

<span data-ttu-id="327aa-118">Este método oferece suporte a $filter, $select e $expand [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="327aa-118">This method supports the $filter, $select, and $expand [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="327aa-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="327aa-119">Request headers</span></span>

| <span data-ttu-id="327aa-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="327aa-120">Header</span></span>       | <span data-ttu-id="327aa-121">Valor</span><span class="sxs-lookup"><span data-stu-id="327aa-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="327aa-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="327aa-122">Authorization</span></span>  | <span data-ttu-id="327aa-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="327aa-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="327aa-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="327aa-125">Request body</span></span>

<span data-ttu-id="327aa-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="327aa-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="327aa-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="327aa-127">Response</span></span>

<span data-ttu-id="327aa-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [teamsAppInstallation](../resources/teamsappinstallation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="327aa-128">If successful, this method returns a `200 OK` response code and collection of [teamsAppInstallation](../resources/teamsappinstallation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="327aa-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="327aa-129">Examples</span></span>

### <a name="example-1-list-installed-apps"></a><span data-ttu-id="327aa-130">Exemplo 1: listar aplicativos instalados</span><span class="sxs-lookup"><span data-stu-id="327aa-130">Example 1: List installed apps</span></span>

#### <a name="request"></a><span data-ttu-id="327aa-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="327aa-131">Request</span></span>

<span data-ttu-id="327aa-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="327aa-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="327aa-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="327aa-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_installed_teams_apps"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/installedApps
```

# <a name="ctabcsharp"></a>[<span data-ttu-id="327aa-134">C#</span><span class="sxs-lookup"><span data-stu-id="327aa-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-installed-teams-apps-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="327aa-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="327aa-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-installed-teams-apps-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="327aa-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="327aa-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-installed-teams-apps-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="327aa-137">Java</span><span class="sxs-lookup"><span data-stu-id="327aa-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-installed-teams-apps-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="327aa-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="327aa-138">Response</span></span>

<span data-ttu-id="327aa-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="327aa-139">The following is an example of the response.</span></span>
><span data-ttu-id="327aa-140">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="327aa-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="327aa-141">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="327aa-141">All the properties will be returned from an actual call.</span></span>
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

### <a name="example-2-get-the-names-and-other-details-of-installed-apps"></a><span data-ttu-id="327aa-142">Exemplo 2: obter os nomes e outros detalhes dos aplicativos instalados</span><span class="sxs-lookup"><span data-stu-id="327aa-142">Example 2: Get the names and other details of installed apps</span></span>

#### <a name="request"></a><span data-ttu-id="327aa-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="327aa-143">Request</span></span>

<span data-ttu-id="327aa-144">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="327aa-144">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="327aa-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="327aa-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_installed_teams_apps_expand"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/installedApps?$expand=teamsAppDefinition
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="327aa-146">C#</span><span class="sxs-lookup"><span data-stu-id="327aa-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-installed-teams-apps-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="327aa-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="327aa-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-installed-teams-apps-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="327aa-148">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="327aa-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-installed-teams-apps-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="327aa-149">Java</span><span class="sxs-lookup"><span data-stu-id="327aa-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-installed-teams-apps-expand-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="327aa-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="327aa-150">Response</span></span>

<span data-ttu-id="327aa-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="327aa-151">The following is an example of the response.</span></span>

><span data-ttu-id="327aa-152">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="327aa-152">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="327aa-153">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="327aa-153">All the properties will be returned from an actual call.</span></span>
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
