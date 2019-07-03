---
title: Listar aplicativos em equipe
description: Recupere a lista de aplicativos instalados na equipe especificada.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 30e729b2418ab93b35d33739459b3c75a6705c51
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35451469"
---
# <a name="list-apps-in-team"></a><span data-ttu-id="0b8af-103">Listar aplicativos em equipe</span><span class="sxs-lookup"><span data-stu-id="0b8af-103">List apps in team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b8af-104">Recupere a lista de [aplicativos instalados](../resources/teamsappinstallation.md) na [equipe](../resources/team.md)especificada.</span><span class="sxs-lookup"><span data-stu-id="0b8af-104">Retrieve the list of [apps installed](../resources/teamsappinstallation.md) in the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0b8af-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0b8af-105">Permissions</span></span>

<span data-ttu-id="0b8af-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b8af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b8af-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0b8af-108">Permission type</span></span>      | <span data-ttu-id="0b8af-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0b8af-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b8af-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0b8af-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0b8af-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b8af-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0b8af-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0b8af-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b8af-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0b8af-113">Not supported.</span></span>    |
|<span data-ttu-id="0b8af-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0b8af-114">Application</span></span> | <span data-ttu-id="0b8af-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b8af-115">Group.Read.All, Group.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="0b8af-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0b8af-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/installedApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0b8af-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0b8af-117">Optional query parameters</span></span>

<span data-ttu-id="0b8af-118">Este método oferece suporte a $filter, $select e $expand [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0b8af-118">This method supports the $filter, $select, and $expand [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0b8af-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0b8af-119">Request headers</span></span>

| <span data-ttu-id="0b8af-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0b8af-120">Header</span></span>       | <span data-ttu-id="0b8af-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0b8af-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0b8af-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0b8af-122">Authorization</span></span>  | <span data-ttu-id="0b8af-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0b8af-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0b8af-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0b8af-125">Request body</span></span>

<span data-ttu-id="0b8af-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0b8af-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b8af-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b8af-127">Response</span></span>

<span data-ttu-id="0b8af-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [teamsApp](../resources/teamsapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0b8af-128">If successful, this method returns a `200 OK` response code and collection of [teamsApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b8af-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0b8af-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="0b8af-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0b8af-130">Request</span></span>

<span data-ttu-id="0b8af-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0b8af-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0b8af-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b8af-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/installedApps
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0b8af-133">C#</span><span class="sxs-lookup"><span data-stu-id="0b8af-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0b8af-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="0b8af-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0b8af-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="0b8af-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0b8af-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b8af-136">Response</span></span>

<span data-ttu-id="0b8af-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0b8af-137">The following is an example of the response.</span></span>
><span data-ttu-id="0b8af-138">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0b8af-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0b8af-139">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0b8af-139">All the properties will be returned from an actual call.</span></span>
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

## <a name="example----getting-the-names-of-the-installed-apps"></a><span data-ttu-id="0b8af-140">Exemplo: obtendo os nomes dos aplicativos instalados</span><span class="sxs-lookup"><span data-stu-id="0b8af-140">Example -- getting the names of the installed apps</span></span>

### <a name="request"></a><span data-ttu-id="0b8af-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0b8af-141">Request</span></span>

<span data-ttu-id="0b8af-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0b8af-142">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0b8af-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b8af-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/installedApps?$expand=teamsAppDefinition
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0b8af-144">C#</span><span class="sxs-lookup"><span data-stu-id="0b8af-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0b8af-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="0b8af-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0b8af-146">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="0b8af-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0b8af-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b8af-147">Response</span></span>

<span data-ttu-id="0b8af-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0b8af-148">The following is an example of the response.</span></span>

><span data-ttu-id="0b8af-149">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0b8af-149">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0b8af-150">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0b8af-150">All the properties will be returned from an actual call.</span></span>
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
