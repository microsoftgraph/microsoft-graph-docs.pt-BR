---
title: Lista de aplicativos na equipe
description: Recupere a lista de aplicativos instalados na equipe de especificado.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: fe3ba5cd3be91c7e69b77f67cb53ab702741c6f5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524608"
---
# <a name="list-apps-in-team"></a><span data-ttu-id="3051a-103">Lista de aplicativos na equipe</span><span class="sxs-lookup"><span data-stu-id="3051a-103">List apps in team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3051a-104">Recupere a lista de [aplicativos instalados](../resources/teamsappinstallation.md) na [equipe](../resources/team.md)de especificado.</span><span class="sxs-lookup"><span data-stu-id="3051a-104">Retrieve the list of [apps installed](../resources/teamsappinstallation.md) in the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3051a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3051a-105">Permissions</span></span>

<span data-ttu-id="3051a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3051a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3051a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3051a-108">Permission type</span></span>      | <span data-ttu-id="3051a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3051a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3051a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3051a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3051a-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3051a-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3051a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3051a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3051a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3051a-113">Not supported.</span></span>    |
|<span data-ttu-id="3051a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3051a-114">Application</span></span> | <span data-ttu-id="3051a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3051a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3051a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3051a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/installedApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3051a-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3051a-117">Optional query parameters</span></span>

<span data-ttu-id="3051a-118">Este método oferece suporte a $filter, $select, e $expand [OData parâmetros de consulta](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3051a-118">This method supports the $filter, $select, and $expand [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3051a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3051a-119">Request headers</span></span>

| <span data-ttu-id="3051a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3051a-120">Header</span></span>       | <span data-ttu-id="3051a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3051a-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3051a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3051a-122">Authorization</span></span>  | <span data-ttu-id="3051a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3051a-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3051a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3051a-125">Request body</span></span>

<span data-ttu-id="3051a-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3051a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3051a-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="3051a-127">Response</span></span>

<span data-ttu-id="3051a-128">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos [teamsApp](../resources/teamsapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3051a-128">If successful, this method returns a `200 OK` response code and collection of [teamsApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3051a-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3051a-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="3051a-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3051a-130">Request</span></span>

<span data-ttu-id="3051a-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3051a-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/installedApps
```

### <a name="response"></a><span data-ttu-id="3051a-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="3051a-132">Response</span></span>

<span data-ttu-id="3051a-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3051a-133">The following is an example of the response.</span></span>
><span data-ttu-id="3051a-134">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3051a-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3051a-135">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3051a-135">All the properties will be returned from an actual call.</span></span>
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

## <a name="example----getting-the-names-of-the-installed-apps"></a><span data-ttu-id="3051a-136">Example - obtendo os nomes dos aplicativos instalados</span><span class="sxs-lookup"><span data-stu-id="3051a-136">Example -- getting the names of the installed apps</span></span>

### <a name="request"></a><span data-ttu-id="3051a-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3051a-137">Request</span></span>

<span data-ttu-id="3051a-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3051a-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/installedApps?$expand=teamsAppDefinition
```

### <a name="response"></a><span data-ttu-id="3051a-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="3051a-139">Response</span></span>

<span data-ttu-id="3051a-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3051a-140">The following is an example of the response.</span></span>

><span data-ttu-id="3051a-141">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3051a-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3051a-142">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3051a-142">All the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/teamsappinstallation-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
