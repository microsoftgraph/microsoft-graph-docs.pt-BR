---
title: Listar aplicativos em equipe
description: Recupere a lista de aplicativos instalados na equipe especificada.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6c5c6032d05234b38cae01e5be71e5eaf2e80dc4
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44491767"
---
# <a name="list-apps-in-team"></a><span data-ttu-id="1c37c-103">Listar aplicativos em equipe</span><span class="sxs-lookup"><span data-stu-id="1c37c-103">List apps in team</span></span>

<span data-ttu-id="1c37c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c37c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1c37c-105">Recupere a lista de [aplicativos instalados](../resources/teamsappinstallation.md) na [equipe](../resources/team.md)especificada.</span><span class="sxs-lookup"><span data-stu-id="1c37c-105">Retrieve the list of [apps installed](../resources/teamsappinstallation.md) in the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1c37c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1c37c-106">Permissions</span></span>

<span data-ttu-id="1c37c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c37c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c37c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1c37c-109">Permission type</span></span>      | <span data-ttu-id="1c37c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1c37c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1c37c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1c37c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1c37c-112">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c37c-112">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="1c37c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1c37c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c37c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1c37c-114">Not supported.</span></span>    |
|<span data-ttu-id="1c37c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1c37c-115">Application</span></span> | <span data-ttu-id="1c37c-116">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c37c-116">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1c37c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1c37c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/installedApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1c37c-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1c37c-118">Optional query parameters</span></span>

<span data-ttu-id="1c37c-119">Este método oferece suporte a $filter, $select e $expand [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1c37c-119">This method supports the $filter, $select, and $expand [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1c37c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1c37c-120">Request headers</span></span>

| <span data-ttu-id="1c37c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1c37c-121">Header</span></span>       | <span data-ttu-id="1c37c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1c37c-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1c37c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1c37c-123">Authorization</span></span>  | <span data-ttu-id="1c37c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1c37c-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1c37c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1c37c-126">Request body</span></span>

<span data-ttu-id="1c37c-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1c37c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c37c-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c37c-128">Response</span></span>

<span data-ttu-id="1c37c-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [teamsAppInstallation](../resources/teamsappinstallation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1c37c-129">If successful, this method returns a `200 OK` response code and collection of [teamsAppInstallation](../resources/teamsappinstallation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1c37c-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1c37c-130">Examples</span></span>

### <a name="example-1-list-installed-apps"></a><span data-ttu-id="1c37c-131">Exemplo 1: listar aplicativos instalados</span><span class="sxs-lookup"><span data-stu-id="1c37c-131">Example 1: List installed apps</span></span>
#### <a name="request"></a><span data-ttu-id="1c37c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1c37c-132">Request</span></span>

<span data-ttu-id="1c37c-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1c37c-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1c37c-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="1c37c-134">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_installed_teams_apps"
}-->

```msgraph-interactive
GET /teams/{id}/installedApps
```
# <a name="c"></a>[<span data-ttu-id="1c37c-135">C#</span><span class="sxs-lookup"><span data-stu-id="1c37c-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-installed-teams-apps-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1c37c-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1c37c-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-installed-teams-apps-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1c37c-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1c37c-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-installed-teams-apps-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1c37c-138">Java</span><span class="sxs-lookup"><span data-stu-id="1c37c-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-installed-teams-apps-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="1c37c-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c37c-139">Response</span></span>

<span data-ttu-id="1c37c-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1c37c-140">The following is an example of the response.</span></span>
><span data-ttu-id="1c37c-141">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1c37c-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1c37c-142">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1c37c-142">All the properties will be returned from an actual call.</span></span>
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

### <a name="example-2-get-the-names-and-other-details-of-installed-apps"></a><span data-ttu-id="1c37c-143">Exemplo 2: obter os nomes e outros detalhes dos aplicativos instalados</span><span class="sxs-lookup"><span data-stu-id="1c37c-143">Example 2: Get the names and other details of installed apps</span></span>

#### <a name="request"></a><span data-ttu-id="1c37c-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1c37c-144">Request</span></span>

<span data-ttu-id="1c37c-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1c37c-145">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1c37c-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="1c37c-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_installed_teams_apps_expand"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{id}/installedApps?$expand=teamsAppDefinition
```
# <a name="c"></a>[<span data-ttu-id="1c37c-147">C#</span><span class="sxs-lookup"><span data-stu-id="1c37c-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-installed-teams-apps-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1c37c-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1c37c-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-installed-teams-apps-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1c37c-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1c37c-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-installed-teams-apps-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1c37c-150">Java</span><span class="sxs-lookup"><span data-stu-id="1c37c-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-installed-teams-apps-expand-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="1c37c-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c37c-151">Response</span></span>

<span data-ttu-id="1c37c-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1c37c-152">The following is an example of the response.</span></span>

><span data-ttu-id="1c37c-153">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1c37c-153">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1c37c-154">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1c37c-154">All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
