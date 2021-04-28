---
title: Obter aplicativo instalado na equipe
description: Instale um aplicativo em equipe.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b5fe5ebf8ac0e65c8ffe2be10dee502f1d0ea0fa
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050252"
---
# <a name="get-installed-app-in-team"></a><span data-ttu-id="0d082-103">Obter aplicativo instalado na equipe</span><span class="sxs-lookup"><span data-stu-id="0d082-103">Get installed app in team</span></span>

<span data-ttu-id="0d082-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d082-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0d082-105">Recupere o [aplicativo](../resources/teamsappinstallation.md) instalado na equipe [especificada](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="0d082-105">Retrieve the [app](../resources/teamsappinstallation.md) installed in the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0d082-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0d082-106">Permissions</span></span>

<span data-ttu-id="0d082-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d082-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d082-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0d082-109">Permission type</span></span>      | <span data-ttu-id="0d082-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0d082-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0d082-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0d082-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0d082-112">TeamsAppInstallation.ReadWriteSelfForTeam, TeamsAppInstallation.ReadForUser, TeamsAppInstallation.ReadForTeam, TeamsAppInstallation.ReadWriteForTeam, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d082-112">TeamsAppInstallation.ReadWriteSelfForTeam, TeamsAppInstallation.ReadForUser, TeamsAppInstallation.ReadForTeam, TeamsAppInstallation.ReadWriteForTeam, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="0d082-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0d082-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d082-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d082-114">Not supported.</span></span>    |
|<span data-ttu-id="0d082-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0d082-115">Application</span></span> | <span data-ttu-id="0d082-116">TeamsAppInstallation.ReadWriteSelfForTeam, TeamsAppInstallation.ReadForTeam.All, TeamsAppInstallation.ReadWriteForTeam.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d082-116">TeamsAppInstallation.ReadWriteSelfForTeam, TeamsAppInstallation.ReadForTeam.All, TeamsAppInstallation.ReadWriteForTeam.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d082-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0d082-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/installedApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0d082-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0d082-118">Request headers</span></span>

| <span data-ttu-id="0d082-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0d082-119">Header</span></span>       | <span data-ttu-id="0d082-120">Valor</span><span class="sxs-lookup"><span data-stu-id="0d082-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0d082-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0d082-121">Authorization</span></span>  | <span data-ttu-id="0d082-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0d082-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0d082-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0d082-124">Request body</span></span>

<span data-ttu-id="0d082-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0d082-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d082-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d082-126">Response</span></span>

<span data-ttu-id="0d082-127">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [teamsAppInstallation](../resources/teamsappinstallation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0d082-127">If successful, this method returns a `200 OK` response code and a [teamsAppInstallation](../resources/teamsappinstallation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0d082-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0d082-128">Examples</span></span>

### <a name="example-1-get-the-installed-app"></a><span data-ttu-id="0d082-129">Exemplo 1: Obter o aplicativo instalado</span><span class="sxs-lookup"><span data-stu-id="0d082-129">Example 1: Get the installed app</span></span>

#### <a name="request"></a><span data-ttu-id="0d082-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0d082-130">Request</span></span>

<span data-ttu-id="0d082-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0d082-131">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0d082-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="0d082-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_installed_teams_apps"
}-->

```msgraph-interactive
GET /teams/{id}/installedApps/{id}
```
# <a name="c"></a>[<span data-ttu-id="0d082-133">C#</span><span class="sxs-lookup"><span data-stu-id="0d082-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-installed-teams-apps-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0d082-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0d082-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-installed-teams-apps-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0d082-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0d082-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-installed-teams-apps-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0d082-136">Java</span><span class="sxs-lookup"><span data-stu-id="0d082-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-installed-teams-apps-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0d082-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d082-137">Response</span></span>

<span data-ttu-id="0d082-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0d082-138">The following is an example of the response.</span></span>
><span data-ttu-id="0d082-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0d082-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2-get-the-names-and-other-details-of-the-installed-app"></a><span data-ttu-id="0d082-140">Exemplo 2: Obter os nomes e outros detalhes do aplicativo instalado</span><span class="sxs-lookup"><span data-stu-id="0d082-140">Example 2: Get the names and other details of the installed app</span></span>

#### <a name="requests"></a><span data-ttu-id="0d082-141">Solicitações</span><span class="sxs-lookup"><span data-stu-id="0d082-141">Requests</span></span>

<span data-ttu-id="0d082-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0d082-142">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0d082-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="0d082-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_installed_teams_apps_expand"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{id}/installedApps/{id}?$expand=teamsAppDefinition
```
# <a name="c"></a>[<span data-ttu-id="0d082-144">C#</span><span class="sxs-lookup"><span data-stu-id="0d082-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-installed-teams-apps-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0d082-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0d082-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-installed-teams-apps-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0d082-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0d082-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-installed-teams-apps-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0d082-147">Java</span><span class="sxs-lookup"><span data-stu-id="0d082-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-installed-teams-apps-expand-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0d082-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d082-148">Response</span></span>

<span data-ttu-id="0d082-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0d082-149">The following is an example of the response.</span></span>

><span data-ttu-id="0d082-150">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0d082-150">**Note:** The response object shown here might be shortened for readability.</span></span>
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
                "version": "1.0.0"
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
