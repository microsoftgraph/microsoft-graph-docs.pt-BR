---
title: Listar guias no canal
description: 'Recupere a lista de guias no canal especificado dentro de uma equipe. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: a5754c443d323dc67b0500f7ad6f198921ed887d
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202230"
---
# <a name="list-tabs-in-channel"></a><span data-ttu-id="4531d-103">Listar guias no canal</span><span class="sxs-lookup"><span data-stu-id="4531d-103">List tabs in channel</span></span>

<span data-ttu-id="4531d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4531d-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="4531d-105">Recupere a lista de [guias](../resources/teamstab.md) no canal [especificado](../resources/channel.md) dentro de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="4531d-105">Retrieve the list of [tabs](../resources/teamstab.md) in the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="4531d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4531d-106">Permissions</span></span>
<span data-ttu-id="4531d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4531d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4531d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4531d-109">Permission type</span></span>      | <span data-ttu-id="4531d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4531d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4531d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4531d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4531d-112">TeamsTab.Read.All, TeamsTab.ReadWriteForTeam, TeamsTab.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4531d-112">TeamsTab.Read.All, TeamsTab.ReadWriteForTeam, TeamsTab.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="4531d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4531d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4531d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4531d-114">Not supported.</span></span>    |
|<span data-ttu-id="4531d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4531d-115">Application</span></span> | <span data-ttu-id="4531d-116">TeamsTab.Read.Group *, TeamsTab.ReadWrite.Group*, TeamsTab.Read.All, TeamsTab.ReadWriteForTeam.All, TeamsTab.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4531d-116">TeamsTab.Read.Group *, TeamsTab.ReadWrite.Group*, TeamsTab.Read.All, TeamsTab.ReadWriteForTeam.All, TeamsTab.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="4531d-117">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="4531d-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="4531d-118">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="4531d-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="4531d-119">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="4531d-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="4531d-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4531d-120">HTTP request</span></span>

```http
GET /teams/{id}/channels/{id}/tabs
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4531d-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4531d-121">Optional query parameters</span></span>

<span data-ttu-id="4531d-122">Este método dá suporte aos [Parâmetros de consulta OData](/graph/query-parameters) $filter, $select e $expand para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4531d-122">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4531d-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4531d-123">Request headers</span></span>
| <span data-ttu-id="4531d-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4531d-124">Header</span></span>       | <span data-ttu-id="4531d-125">Valor</span><span class="sxs-lookup"><span data-stu-id="4531d-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4531d-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="4531d-126">Authorization</span></span>  | <span data-ttu-id="4531d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4531d-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4531d-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4531d-129">Request body</span></span>
<span data-ttu-id="4531d-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4531d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4531d-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="4531d-131">Response</span></span>
<span data-ttu-id="4531d-132">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [tabs](../resources/teamstab.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4531d-132">If successful, this method returns a `200 OK` response code and collection of [tabs](../resources/teamstab.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4531d-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4531d-133">Examples</span></span>

### <a name="example-1-list-all-the-tabs-in-the-channel-along-with-associated-teams-app"></a><span data-ttu-id="4531d-134">Exemplo 1: listar todas as guias do canal juntamente com o aplicativo do Teams associado</span><span class="sxs-lookup"><span data-stu-id="4531d-134">Example 1: List all the tabs in the channel along with associated Teams app</span></span>
#### <a name="request"></a><span data-ttu-id="4531d-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4531d-135">Request</span></span>
<span data-ttu-id="4531d-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4531d-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4531d-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="4531d-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_tabs_in_channel_app_filter_1"
}
-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/6903fa93-605b-43ef-920e-77c4729f8258/channels/19:33b76eea88574bd1969dca37e2b7a819@thread.skype/tabs?$expand=teamsApp
```
# <a name="c"></a>[<span data-ttu-id="4531d-138">C#</span><span class="sxs-lookup"><span data-stu-id="4531d-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-tabs-in-channel-app-filter-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4531d-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4531d-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-tabs-in-channel-app-filter-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4531d-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4531d-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-tabs-in-channel-app-filter-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4531d-141">Java</span><span class="sxs-lookup"><span data-stu-id="4531d-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-tabs-in-channel-app-filter-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4531d-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="4531d-142">Response</span></span>
<span data-ttu-id="4531d-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4531d-143">The following is an example of the response.</span></span>
><span data-ttu-id="4531d-144">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4531d-144">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.teamsTab)"
}
-->

```http
HTTP/1.1 200 Success
Content-type: application/json

{
  "value": [
    {
      "id": "794f0e4e-4d10-4bb5-9079-3a465a629eff",
      "displayName": "My Contoso Tab - updated",
      "configuration": {
        "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
        "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
        "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
        "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
      },
      "sortOrderIndex": "20",
      "teamsApp": {
        "id": "06805b9e-77e3-4b93-ac81-525eb87513b8",
        "displayName": "Contoso",
        "distributionMethod": "store"
      },
      "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3afd736d46-51ed-4c0b-9b23-e67ca354bb24?label=my%20%contoso%to%tab"
    },
    {
      "id": "b5d5f001-0471-49a5-aac4-04ef96683be0",
      "displayName": "My Planner Tab",
      "configuration": null,
      "sortOrderIndex": "21",
      "teamsApp": {
        "id": "com.microsoft.teamspace.tab.planner",
        "displayName": "Microsoft Planner",
        "distributionMethod": "store"
      },
      "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3a3709b35c-a0ba-467c-8001-0f66895fb9d3?label=My%20Planner%Tab"
    }
  ]
}
```

### <a name="example-2-list-all-the-tabs-belonging-to-a-specific-app-in-a-channel"></a><span data-ttu-id="4531d-145">Exemplo 2: listar todas as guias pertencentes a um aplicativo específico em um canal</span><span class="sxs-lookup"><span data-stu-id="4531d-145">Example 2: List all the tabs belonging to a specific app in a channel</span></span>
#### <a name="request"></a><span data-ttu-id="4531d-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4531d-146">Request</span></span>
<span data-ttu-id="4531d-147">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4531d-147">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4531d-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="4531d-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_tabs_in_channel_app_filter_2"
}
-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/6903fa93-605b-43ef-920e-77c4729f8258/channels/19:33b76eea88574bd1969dca37e2b7a819@thread.skype/tabs?$expand=teamsApp&$filter=teamsApp/id eq 'com.microsoft.teamspace.tab.planner'
```
# <a name="c"></a>[<span data-ttu-id="4531d-149">C#</span><span class="sxs-lookup"><span data-stu-id="4531d-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-tabs-in-channel-app-filter-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4531d-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4531d-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-tabs-in-channel-app-filter-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4531d-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4531d-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-tabs-in-channel-app-filter-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4531d-152">Java</span><span class="sxs-lookup"><span data-stu-id="4531d-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-tabs-in-channel-app-filter-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4531d-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="4531d-153">Response</span></span>
<span data-ttu-id="4531d-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4531d-154">The following is an example of the response.</span></span>
><span data-ttu-id="4531d-155">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4531d-155">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.teamsTab)"
}
-->

```http
HTTP/1.1 200 Success
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('6903fa93-605b-43ef-920e-77c4729f8258')/channels('19%3A33b76eea88574bd1969dca37e2b7a819%40thread.skype')/tabs(teamsApp())",
  "@odata.count": 1,
  "value": [
    {
      "id": "b5d5f001-0471-49a5-aac4-04ef96683be0",
      "displayName": "My Planner Tab",
      "configuration": null,
      "sortOrderIndex": "21",
      "teamsApp": {
        "id": "com.microsoft.teamspace.tab.planner",
        "displayName": "Microsoft Planner",
        "distributionMethod": "store"
      },
      "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3a3709b35c-a0ba-467c-8001-0f66895fb9d3?label=My%20Planner%Tab"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List all tabs in channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->

