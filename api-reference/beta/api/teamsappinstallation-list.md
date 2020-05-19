---
title: Listar aplicativos em equipe
description: Recupere a lista de aplicativos instalados na equipe especificada.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ae4e60a824189e24f8347d352c5f6f5b42528eeb
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289923"
---
# <a name="list-apps-in-team"></a><span data-ttu-id="67ad4-103">Listar aplicativos em equipe</span><span class="sxs-lookup"><span data-stu-id="67ad4-103">List apps in team</span></span>

<span data-ttu-id="67ad4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67ad4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67ad4-105">Recupere a lista de [aplicativos instalados](../resources/teamsappinstallation.md) na [equipe](../resources/team.md)especificada.</span><span class="sxs-lookup"><span data-stu-id="67ad4-105">Retrieve the list of [apps installed](../resources/teamsappinstallation.md) in the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="67ad4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="67ad4-106">Permissions</span></span>

<span data-ttu-id="67ad4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67ad4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67ad4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="67ad4-109">Permission type</span></span>      | <span data-ttu-id="67ad4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="67ad4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="67ad4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="67ad4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="67ad4-112">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67ad4-112">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="67ad4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="67ad4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67ad4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67ad4-114">Not supported.</span></span>    |
|<span data-ttu-id="67ad4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="67ad4-115">Application</span></span> | <span data-ttu-id="67ad4-116">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67ad4-116">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="67ad4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="67ad4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/installedApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="67ad4-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="67ad4-118">Optional query parameters</span></span>

<span data-ttu-id="67ad4-119">Este método oferece suporte a $filter, $select e $expand [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="67ad4-119">This method supports the $filter, $select, and $expand [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="67ad4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="67ad4-120">Request headers</span></span>

| <span data-ttu-id="67ad4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="67ad4-121">Header</span></span>       | <span data-ttu-id="67ad4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="67ad4-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="67ad4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="67ad4-123">Authorization</span></span>  | <span data-ttu-id="67ad4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="67ad4-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="67ad4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="67ad4-126">Request body</span></span>

<span data-ttu-id="67ad4-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="67ad4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="67ad4-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="67ad4-128">Response</span></span>

<span data-ttu-id="67ad4-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [teamsAppInstallation](../resources/teamsappinstallation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="67ad4-129">If successful, this method returns a `200 OK` response code and collection of [teamsAppInstallation](../resources/teamsappinstallation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="67ad4-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="67ad4-130">Examples</span></span>

### <a name="example-1-list-installed-apps"></a><span data-ttu-id="67ad4-131">Exemplo 1: listar aplicativos instalados</span><span class="sxs-lookup"><span data-stu-id="67ad4-131">Example 1: List installed apps</span></span>

#### <a name="request"></a><span data-ttu-id="67ad4-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="67ad4-132">Request</span></span>

<span data-ttu-id="67ad4-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="67ad4-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="67ad4-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="67ad4-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_installed_teams_apps"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{id}/installedApps
```

# <a name="c"></a>[<span data-ttu-id="67ad4-135">C#</span><span class="sxs-lookup"><span data-stu-id="67ad4-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-installed-teams-apps-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="67ad4-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="67ad4-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-installed-teams-apps-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="67ad4-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="67ad4-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-installed-teams-apps-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="67ad4-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="67ad4-138">Response</span></span>

<span data-ttu-id="67ad4-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="67ad4-139">The following is an example of the response.</span></span>
><span data-ttu-id="67ad4-140">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="67ad4-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="67ad4-141">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="67ad4-141">All the properties will be returned from an actual call.</span></span>
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

### <a name="example-2-get-the-names-and-other-details-of-installed-apps"></a><span data-ttu-id="67ad4-142">Exemplo 2: obter os nomes e outros detalhes dos aplicativos instalados</span><span class="sxs-lookup"><span data-stu-id="67ad4-142">Example 2: Get the names and other details of installed apps</span></span>

#### <a name="request"></a><span data-ttu-id="67ad4-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="67ad4-143">Request</span></span>

<span data-ttu-id="67ad4-144">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="67ad4-144">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="67ad4-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="67ad4-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_installed_teams_apps_expand"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{id}/installedApps?$expand=teamsAppDefinition
```
# <a name="c"></a>[<span data-ttu-id="67ad4-146">C#</span><span class="sxs-lookup"><span data-stu-id="67ad4-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-installed-teams-apps-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="67ad4-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="67ad4-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-installed-teams-apps-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="67ad4-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="67ad4-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-installed-teams-apps-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="67ad4-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="67ad4-149">Response</span></span>

<span data-ttu-id="67ad4-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="67ad4-150">The following is an example of the response.</span></span>

><span data-ttu-id="67ad4-151">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="67ad4-151">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="67ad4-152">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="67ad4-152">All the properties will be returned from an actual call.</span></span>
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
