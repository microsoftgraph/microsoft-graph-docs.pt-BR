---
title: Obter aplicativo instalado na equipe
description: Instale um aplicativo em equipe.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c9096bab3717f7e81130856313da56236d5a0f02
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050819"
---
# <a name="get-installed-app-in-team"></a><span data-ttu-id="bcafe-103">Obter aplicativo instalado na equipe</span><span class="sxs-lookup"><span data-stu-id="bcafe-103">Get installed app in team</span></span>

<span data-ttu-id="bcafe-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bcafe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bcafe-105">Recupere o [aplicativo](../resources/teamsappinstallation.md) instalado na equipe [especificada](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="bcafe-105">Retrieve the [app](../resources/teamsappinstallation.md) installed in the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bcafe-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bcafe-106">Permissions</span></span>

<span data-ttu-id="bcafe-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bcafe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bcafe-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bcafe-109">Permission type</span></span>      | <span data-ttu-id="bcafe-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bcafe-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bcafe-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bcafe-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bcafe-112">TeamsAppInstallation.ReadWriteSelfForTeam, TeamsAppInstallation.ReadForUser, TeamsAppInstallation.ReadForTeam, TeamsAppInstallation.ReadWriteForTeam, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcafe-112">TeamsAppInstallation.ReadWriteSelfForTeam, TeamsAppInstallation.ReadForUser, TeamsAppInstallation.ReadForTeam, TeamsAppInstallation.ReadWriteForTeam, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="bcafe-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bcafe-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bcafe-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bcafe-114">Not supported.</span></span>    |
|<span data-ttu-id="bcafe-115">Application</span><span class="sxs-lookup"><span data-stu-id="bcafe-115">Application</span></span> | <span data-ttu-id="bcafe-116">TeamsAppInstallation.ReadWriteSelfForTeam, TeamsAppInstallation.ReadForTeam.All, TeamsAppInstallation.ReadWriteForTeam.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcafe-116">TeamsAppInstallation.ReadWriteSelfForTeam, TeamsAppInstallation.ReadForTeam.All, TeamsAppInstallation.ReadWriteForTeam.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bcafe-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bcafe-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/installedApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="bcafe-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bcafe-118">Request headers</span></span>

| <span data-ttu-id="bcafe-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bcafe-119">Header</span></span>       | <span data-ttu-id="bcafe-120">Valor</span><span class="sxs-lookup"><span data-stu-id="bcafe-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bcafe-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="bcafe-121">Authorization</span></span>  | <span data-ttu-id="bcafe-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bcafe-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bcafe-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bcafe-124">Request body</span></span>

<span data-ttu-id="bcafe-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bcafe-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bcafe-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="bcafe-126">Response</span></span>

<span data-ttu-id="bcafe-127">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [teamsAppInstallation](../resources/teamsappinstallation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bcafe-127">If successful, this method returns a `200 OK` response code and a [teamsAppInstallation](../resources/teamsappinstallation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bcafe-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="bcafe-128">Examples</span></span>

### <a name="example-1-get-the-installed-app"></a><span data-ttu-id="bcafe-129">Exemplo 1: Obter o aplicativo instalado</span><span class="sxs-lookup"><span data-stu-id="bcafe-129">Example 1: Get the installed app</span></span>
#### <a name="request"></a><span data-ttu-id="bcafe-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bcafe-130">Request</span></span>

<span data-ttu-id="bcafe-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bcafe-131">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="bcafe-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="bcafe-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_installed_teams_apps"
}-->

```msgraph-interactive
GET /teams/{id}/installedApps/{id}
```
# <a name="c"></a>[<span data-ttu-id="bcafe-133">C#</span><span class="sxs-lookup"><span data-stu-id="bcafe-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-installed-teams-apps-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bcafe-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bcafe-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-installed-teams-apps-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bcafe-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bcafe-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-installed-teams-apps-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bcafe-136">Java</span><span class="sxs-lookup"><span data-stu-id="bcafe-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-installed-teams-apps-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="bcafe-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="bcafe-137">Response</span></span>

<span data-ttu-id="bcafe-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bcafe-138">The following is an example of the response.</span></span>
><span data-ttu-id="bcafe-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="bcafe-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2-get-the-names-and-other-details-of-the-installed-app"></a><span data-ttu-id="bcafe-140">Exemplo 2: Obter os nomes e outros detalhes do aplicativo instalado</span><span class="sxs-lookup"><span data-stu-id="bcafe-140">Example 2: Get the names and other details of the installed app</span></span>

#### <a name="request"></a><span data-ttu-id="bcafe-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bcafe-141">Request</span></span>

<span data-ttu-id="bcafe-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bcafe-142">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="bcafe-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="bcafe-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_installed_teams_apps_expand"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{id}/installedApps/{id}?$expand=teamsAppDefinition
```
# <a name="c"></a>[<span data-ttu-id="bcafe-144">C#</span><span class="sxs-lookup"><span data-stu-id="bcafe-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-installed-teams-apps-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bcafe-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bcafe-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-installed-teams-apps-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bcafe-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bcafe-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-installed-teams-apps-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bcafe-147">Java</span><span class="sxs-lookup"><span data-stu-id="bcafe-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-installed-teams-apps-expand-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="bcafe-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="bcafe-148">Response</span></span>

<span data-ttu-id="bcafe-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bcafe-149">The following is an example of the response.</span></span>

><span data-ttu-id="bcafe-150">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="bcafe-150">**Note:** The response object shown here might be shortened for readability.</span></span>
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

