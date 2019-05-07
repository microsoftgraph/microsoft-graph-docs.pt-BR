---
title: Listar aplicativos em equipe
description: Recupere a lista de aplicativos instalados na equipe especificada.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 6de93a0613aa872154e2448450552585d50e6a2e
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33602330"
---
# <a name="list-apps-in-team"></a><span data-ttu-id="6ed1b-103">Listar aplicativos em equipe</span><span class="sxs-lookup"><span data-stu-id="6ed1b-103">List apps in team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ed1b-104">Recupere a lista de [aplicativos instalados](../resources/teamsappinstallation.md) na [equipe](../resources/team.md)especificada.</span><span class="sxs-lookup"><span data-stu-id="6ed1b-104">Retrieve the list of [apps installed](../resources/teamsappinstallation.md) in the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6ed1b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="6ed1b-105">Permissions</span></span>

<span data-ttu-id="6ed1b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ed1b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ed1b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6ed1b-108">Permission type</span></span>      | <span data-ttu-id="6ed1b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6ed1b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6ed1b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6ed1b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6ed1b-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ed1b-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6ed1b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6ed1b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ed1b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6ed1b-113">Not supported.</span></span>    |
|<span data-ttu-id="6ed1b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6ed1b-114">Application</span></span> | <span data-ttu-id="6ed1b-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ed1b-115">Group.Read.All, Group.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="6ed1b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6ed1b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/installedApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6ed1b-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6ed1b-117">Optional query parameters</span></span>

<span data-ttu-id="6ed1b-118">Este método oferece suporte a $filter, $select e $expand [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6ed1b-118">This method supports the $filter, $select, and $expand [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6ed1b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6ed1b-119">Request headers</span></span>

| <span data-ttu-id="6ed1b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6ed1b-120">Header</span></span>       | <span data-ttu-id="6ed1b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6ed1b-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6ed1b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6ed1b-122">Authorization</span></span>  | <span data-ttu-id="6ed1b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6ed1b-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6ed1b-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6ed1b-125">Request body</span></span>

<span data-ttu-id="6ed1b-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6ed1b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6ed1b-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ed1b-127">Response</span></span>

<span data-ttu-id="6ed1b-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [teamsApp](../resources/teamsapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6ed1b-128">If successful, this method returns a `200 OK` response code and collection of [teamsApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ed1b-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6ed1b-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="6ed1b-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6ed1b-130">Request</span></span>

<span data-ttu-id="6ed1b-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6ed1b-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/installedApps
```

### <a name="response"></a><span data-ttu-id="6ed1b-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ed1b-132">Response</span></span>

<span data-ttu-id="6ed1b-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6ed1b-133">The following is an example of the response.</span></span>
><span data-ttu-id="6ed1b-134">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6ed1b-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="6ed1b-135">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6ed1b-135">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="6ed1b-136">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="6ed1b-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6ed1b-137">Basic</span><span class="sxs-lookup"><span data-stu-id="6ed1b-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_owners-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6ed1b-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6ed1b-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_owners-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="example----getting-the-names-of-the-installed-apps"></a><span data-ttu-id="6ed1b-139">Exemplo: obtendo os nomes dos aplicativos instalados</span><span class="sxs-lookup"><span data-stu-id="6ed1b-139">Example -- getting the names of the installed apps</span></span>

### <a name="request"></a><span data-ttu-id="6ed1b-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6ed1b-140">Request</span></span>

<span data-ttu-id="6ed1b-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6ed1b-141">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/installedApps?$expand=teamsAppDefinition
```

### <a name="response"></a><span data-ttu-id="6ed1b-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ed1b-142">Response</span></span>

<span data-ttu-id="6ed1b-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6ed1b-143">The following is an example of the response.</span></span>

><span data-ttu-id="6ed1b-144">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6ed1b-144">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="6ed1b-145">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6ed1b-145">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="6ed1b-146">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="6ed1b-146">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6ed1b-147">Basic</span><span class="sxs-lookup"><span data-stu-id="6ed1b-147">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_owners-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6ed1b-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6ed1b-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_owners-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/teamsappinstallation-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/teamsappinstallation-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/teamsappinstallation-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/teamsappinstallation-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
