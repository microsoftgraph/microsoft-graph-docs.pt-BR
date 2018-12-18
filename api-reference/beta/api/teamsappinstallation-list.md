---
title: Lista de aplicativos na equipe
description: Recupere a lista de aplicativos instalados na equipe de especificado.
author: nkramer
ms.openlocfilehash: d412085663a67a16fe435c8555d802cec662a23e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27357285"
---
# <a name="list-apps-in-team"></a><span data-ttu-id="bae02-103">Lista de aplicativos na equipe</span><span class="sxs-lookup"><span data-stu-id="bae02-103">List apps in team</span></span>

> <span data-ttu-id="bae02-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bae02-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bae02-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bae02-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bae02-106">Recupere a lista de [aplicativos instalados](../resources/teamsappinstallation.md) na [equipe](../resources/team.md)de especificado.</span><span class="sxs-lookup"><span data-stu-id="bae02-106">Retrieve the list of [apps installed](../resources/teamsappinstallation.md) in the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bae02-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="bae02-107">Permissions</span></span>

<span data-ttu-id="bae02-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bae02-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bae02-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bae02-110">Permission type</span></span>      | <span data-ttu-id="bae02-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bae02-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bae02-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bae02-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bae02-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bae02-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="bae02-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bae02-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bae02-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bae02-115">Not supported.</span></span>    |
|<span data-ttu-id="bae02-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bae02-116">Application</span></span> | <span data-ttu-id="bae02-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bae02-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bae02-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bae02-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/installedApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bae02-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bae02-119">Optional query parameters</span></span>

<span data-ttu-id="bae02-120">Este método oferece suporte a $filter, $select, e $expand [OData parâmetros de consulta](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="bae02-120">This method supports the $filter, $select, and $expand [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bae02-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bae02-121">Request headers</span></span>

| <span data-ttu-id="bae02-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bae02-122">Header</span></span>       | <span data-ttu-id="bae02-123">Valor</span><span class="sxs-lookup"><span data-stu-id="bae02-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bae02-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="bae02-124">Authorization</span></span>  | <span data-ttu-id="bae02-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bae02-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bae02-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bae02-127">Request body</span></span>

<span data-ttu-id="bae02-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bae02-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bae02-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="bae02-129">Response</span></span>

<span data-ttu-id="bae02-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos [teamsApp](../resources/teamsapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bae02-130">If successful, this method returns a `200 OK` response code and collection of [teamsApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bae02-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bae02-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="bae02-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bae02-132">Request</span></span>

<span data-ttu-id="bae02-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bae02-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/installedApps
```

### <a name="response"></a><span data-ttu-id="bae02-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="bae02-134">Response</span></span>

<span data-ttu-id="bae02-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bae02-135">The following is an example of the response.</span></span>
><span data-ttu-id="bae02-136">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="bae02-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="bae02-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bae02-137">All the properties will be returned from an actual call.</span></span>
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

## <a name="example----getting-the-names-of-the-installed-apps"></a><span data-ttu-id="bae02-138">Example - obtendo os nomes dos aplicativos instalados</span><span class="sxs-lookup"><span data-stu-id="bae02-138">Example -- getting the names of the installed apps</span></span>

### <a name="request"></a><span data-ttu-id="bae02-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bae02-139">Request</span></span>

<span data-ttu-id="bae02-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bae02-140">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/installedApps?$expand=teamsAppDefinition
```

### <a name="response"></a><span data-ttu-id="bae02-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="bae02-141">Response</span></span>

<span data-ttu-id="bae02-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bae02-142">The following is an example of the response.</span></span>

><span data-ttu-id="bae02-143">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="bae02-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="bae02-144">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bae02-144">All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->