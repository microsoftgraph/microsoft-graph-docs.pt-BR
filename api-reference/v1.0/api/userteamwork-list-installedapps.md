---
title: Listar aplicativos instalados para o usuário
description: Recupere a lista de aplicativos instalados no escopo pessoal do usuário especificado.
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 0f44fdc43328507a4cf156ce25d528b1c2bb8d6d
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2020
ms.locfileid: "49564014"
---
# <a name="list-apps-installed-for-user"></a><span data-ttu-id="643ba-103">Listar aplicativos instalados para o usuário</span><span class="sxs-lookup"><span data-stu-id="643ba-103">List apps installed for user</span></span>

<span data-ttu-id="643ba-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="643ba-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="643ba-105">Recupere a lista de [aplicativos](../resources/teamsappinstallation.md) instalados no escopo pessoal do [usuário](../resources/user.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="643ba-105">Retrieve the list of [apps](../resources/teamsappinstallation.md) installed in the personal scope of the specified [user](../resources/user.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="643ba-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="643ba-106">Permissions</span></span>

<span data-ttu-id="643ba-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="643ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="643ba-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="643ba-109">Permission type</span></span>      | <span data-ttu-id="643ba-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="643ba-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="643ba-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="643ba-111">Delegated (work or school account)</span></span> | <span data-ttu-id="643ba-112">TeamsAppInstallation. ReadForUser, TeamsAppInstallation. Read, TeamsAppInstallation. ReadWriteSelfForUser, TeamsAppInstallation. ReadWriteForUser, TeamsAppInstallation. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="643ba-112">TeamsAppInstallation.ReadForUser, TeamsAppInstallation.Read, TeamsAppInstallation.ReadWriteSelfForUser, TeamsAppInstallation.ReadWriteForUser, TeamsAppInstallation.ReadWrite</span></span> |
|<span data-ttu-id="643ba-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="643ba-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="643ba-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="643ba-114">Not supported.</span></span>    |
|<span data-ttu-id="643ba-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="643ba-115">Application</span></span> | <span data-ttu-id="643ba-116">TeamsAppInstallation. ReadForUser. All, TeamsAppInstallation. Read. All, TeamsAppInstallation. ReadWriteSelfForUser. All, TeamsAppInstallation. ReadWriteForUser. All, TeamsAppInstallation. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="643ba-116">TeamsAppInstallation.ReadForUser.All, TeamsAppInstallation.Read.All,TeamsAppInstallation.ReadWriteSelfForUser.All, TeamsAppInstallation.ReadWriteForUser.All, TeamsAppInstallation.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="643ba-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="643ba-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{id}/teamwork/installedApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="643ba-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="643ba-118">Optional query parameters</span></span>

<span data-ttu-id="643ba-119">Este método dá suporte aos [Parâmetros de consulta OData](/graph/query-parameters) $filter, $select e $expand para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="643ba-119">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="643ba-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="643ba-120">Request headers</span></span>

| <span data-ttu-id="643ba-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="643ba-121">Header</span></span>       | <span data-ttu-id="643ba-122">Valor</span><span class="sxs-lookup"><span data-stu-id="643ba-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="643ba-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="643ba-123">Authorization</span></span>  | <span data-ttu-id="643ba-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="643ba-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="643ba-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="643ba-126">Request body</span></span>

<span data-ttu-id="643ba-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="643ba-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="643ba-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="643ba-128">Response</span></span>

<span data-ttu-id="643ba-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [teamsAppInstallation](../resources/teamsappinstallation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="643ba-129">If successful, this method returns a `200 OK` response code and a collection of [teamsAppInstallation](../resources/teamsappinstallation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="643ba-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="643ba-130">Examples</span></span>

### <a name="example-1-list-apps-installed-for-the-specified-user"></a><span data-ttu-id="643ba-131">Exemplo 1: listar aplicativos instalados para o usuário especificado</span><span class="sxs-lookup"><span data-stu-id="643ba-131">Example 1: List apps installed for the specified user</span></span>

#### <a name="request"></a><span data-ttu-id="643ba-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="643ba-132">Request</span></span>

<span data-ttu-id="643ba-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="643ba-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_list_teamsApps"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/5b649834-7412-4cce-9e69-176e95a394f5/teamwork/installedApps
```

#### <a name="response"></a><span data-ttu-id="643ba-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="643ba-134">Response</span></span>

<span data-ttu-id="643ba-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="643ba-135">The following is an example of the response.</span></span>
><span data-ttu-id="643ba-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="643ba-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "user_list_teamsApps",
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
      "id": "YTZiNjMzNjUtMzFhNC00ZjQzLTkyZWMtNzEwYjcxNTU3YWY5IyMwLjk="
    }
  ]
}
```

### <a name="example-2-get-the-names-and-other-details-of-apps-installed-for-the-user"></a><span data-ttu-id="643ba-138">Exemplo 2: obter os nomes e outros detalhes dos aplicativos instalados para o usuário</span><span class="sxs-lookup"><span data-stu-id="643ba-138">Example 2: Get the names and other details of apps installed for the user</span></span>

#### <a name="request"></a><span data-ttu-id="643ba-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="643ba-139">Request</span></span>

<span data-ttu-id="643ba-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="643ba-140">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "user_list_teamsApps_details"
} -->

```http
GET https://graph.microsoft.com/v1.0/users/5b649834-7412-4cce-9e69-176e95a394f5/teamwork/installedApps?$expand=teamsAppDefinition
```

#### <a name="response"></a><span data-ttu-id="643ba-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="643ba-141">Response</span></span>

<span data-ttu-id="643ba-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="643ba-142">The following is an example of the response.</span></span>

><span data-ttu-id="643ba-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="643ba-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "user_list_teamsApps_details",
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
  "description": "User list teamsAppInstallations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
