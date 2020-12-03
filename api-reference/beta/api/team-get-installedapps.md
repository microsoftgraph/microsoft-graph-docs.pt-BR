---
title: Obter o aplicativo instalado no Team
description: Obter um aplicativo instalado no Team.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 49903514fb6345978d90ca1df7a8ab5279c61410
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2020
ms.locfileid: "49564137"
---
# <a name="get-installed-app-in-team"></a><span data-ttu-id="c3504-103">Obter o aplicativo instalado no Team</span><span class="sxs-lookup"><span data-stu-id="c3504-103">Get installed app in team</span></span>

<span data-ttu-id="c3504-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3504-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3504-105">Recupere o [aplicativo](../resources/teamsappinstallation.md) instalado na [equipe](../resources/team.md)especificada.</span><span class="sxs-lookup"><span data-stu-id="c3504-105">Retrieve the [app](../resources/teamsappinstallation.md) installed in the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c3504-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="c3504-106">Permissions</span></span>

<span data-ttu-id="c3504-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3504-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3504-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c3504-109">Permission type</span></span>      | <span data-ttu-id="c3504-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c3504-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c3504-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c3504-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c3504-112">TeamsAppInstallation. ReadWriteSelfForTeam, TeamsAppInstallation. ReadForUser, TeamsAppInstallation. ReadForTeam, TeamsAppInstallation. ReadWriteForTeam, Group. Read. All, Group. ReadWrite. All, Directory. Read. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="c3504-112">TeamsAppInstallation.ReadWriteSelfForTeam, TeamsAppInstallation.ReadForUser, TeamsAppInstallation.ReadForTeam, TeamsAppInstallation.ReadWriteForTeam, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="c3504-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c3504-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3504-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c3504-114">Not supported.</span></span>    |
|<span data-ttu-id="c3504-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c3504-115">Application</span></span> | <span data-ttu-id="c3504-116">TeamsAppInstallation. ReadWriteSelfForTeam, TeamsAppInstallation. ReadForTeam. All, TeamsAppInstallation. ReadWriteForTeam. All, Group. Read. All, Group. ReadWrite. All, Directory. Read. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="c3504-116">TeamsAppInstallation.ReadWriteSelfForTeam, TeamsAppInstallation.ReadForTeam.All, TeamsAppInstallation.ReadWriteForTeam.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c3504-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c3504-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/installedApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c3504-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c3504-118">Request headers</span></span>

| <span data-ttu-id="c3504-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c3504-119">Header</span></span>       | <span data-ttu-id="c3504-120">Valor</span><span class="sxs-lookup"><span data-stu-id="c3504-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c3504-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c3504-121">Authorization</span></span>  | <span data-ttu-id="c3504-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c3504-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c3504-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c3504-124">Request body</span></span>

<span data-ttu-id="c3504-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c3504-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c3504-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3504-126">Response</span></span>

<span data-ttu-id="c3504-127">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [teamsAppInstallation](../resources/teamsappinstallation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c3504-127">If successful, this method returns a `200 OK` response code and a [teamsAppInstallation](../resources/teamsappinstallation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c3504-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c3504-128">Examples</span></span>

### <a name="example-1-get-the-installed-app"></a><span data-ttu-id="c3504-129">Exemplo 1: obter o aplicativo instalado</span><span class="sxs-lookup"><span data-stu-id="c3504-129">Example 1: Get the installed app</span></span>
#### <a name="request"></a><span data-ttu-id="c3504-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c3504-130">Request</span></span>

<span data-ttu-id="c3504-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c3504-131">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_installed_teams_apps"
}-->

```msgraph-interactive
GET /teams/{id}/installedApps/{id}
```

---

#### <a name="response"></a><span data-ttu-id="c3504-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3504-132">Response</span></span>

<span data-ttu-id="c3504-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c3504-133">The following is an example of the response.</span></span>
><span data-ttu-id="c3504-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c3504-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_installed_teams_apps",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "isCollection": false
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

### <a name="example-2-get-the-names-and-other-details-of-the-installed-app"></a><span data-ttu-id="c3504-136">Exemplo 2: obter os nomes e outros detalhes do aplicativo instalado</span><span class="sxs-lookup"><span data-stu-id="c3504-136">Example 2: Get the names and other details of the installed app</span></span>

#### <a name="request"></a><span data-ttu-id="c3504-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c3504-137">Request</span></span>

<span data-ttu-id="c3504-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c3504-138">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_installed_teams_apps_expand"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{id}/installedApps/{id}?$expand=teamsAppDefinition
```

---

#### <a name="response"></a><span data-ttu-id="c3504-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3504-139">Response</span></span>

<span data-ttu-id="c3504-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c3504-140">The following is an example of the response.</span></span>

><span data-ttu-id="c3504-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c3504-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_installed_teams_apps_expand",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "isCollection": false
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
                "version": "beta"
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

