---
title: Adicionar uma guia ao canal
description: 'Adiciona (pins) a uma guia para o canal especificado dentro de uma equipe. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5575c4ae9267a968c7381ba4a89b66f9e0e7698d
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047536"
---
# <a name="add-tab-to-channel"></a><span data-ttu-id="08316-103">Adicionar uma guia ao canal</span><span class="sxs-lookup"><span data-stu-id="08316-103">Add tab to channel</span></span>

<span data-ttu-id="08316-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08316-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08316-105">Adiciona (pins) a uma [guia](../resources/teamstab.md) para o canal [especificado](../resources/channel.md) dentro de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="08316-105">Adds (pins) a [tab](../resources/teamstab.md) to the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> <span data-ttu-id="08316-106">O aplicativo correspondente já deve estar [instalado na equipe](../api/team-list-installedapps.md).</span><span class="sxs-lookup"><span data-stu-id="08316-106">The corresponding app must already be [installed in the team](../api/team-list-installedapps.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="08316-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="08316-107">Permissions</span></span>
<span data-ttu-id="08316-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08316-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08316-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="08316-110">Permission type</span></span>      | <span data-ttu-id="08316-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="08316-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08316-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="08316-112">Delegated (work or school account)</span></span> | <span data-ttu-id="08316-113">TeamsTab.Create, TeamsTab.ReadWriteForTeam, TeamsTab.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08316-113">TeamsTab.Create, TeamsTab.ReadWriteForTeam, TeamsTab.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="08316-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="08316-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08316-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="08316-115">Not supported.</span></span>    |
| <span data-ttu-id="08316-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="08316-116">Application</span></span>   | <span data-ttu-id="08316-117">TeamsTab.Create.Group\*, TeamsTab.Create, TeamsTab.ReadWriteForTeam.All, TeamsTab.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08316-117">TeamsTab.Create.Group\*, TeamsTab.Create, TeamsTab.ReadWriteForTeam.All, TeamsTab.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="08316-118">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="08316-118">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="08316-119">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="08316-119">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="08316-120">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="08316-120">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="08316-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="08316-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/tabs
```

## <a name="request-headers"></a><span data-ttu-id="08316-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="08316-122">Request headers</span></span>
| <span data-ttu-id="08316-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="08316-123">Header</span></span>       | <span data-ttu-id="08316-124">Valor</span><span class="sxs-lookup"><span data-stu-id="08316-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="08316-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="08316-125">Authorization</span></span>  | <span data-ttu-id="08316-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="08316-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="08316-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="08316-128">Request body</span></span>

<span data-ttu-id="08316-129">Uma [teamsTab](../resources/teamstab.md).</span><span class="sxs-lookup"><span data-stu-id="08316-129">A [teamsTab](../resources/teamstab.md).</span></span>

## <a name="response"></a><span data-ttu-id="08316-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="08316-130">Response</span></span>

<span data-ttu-id="08316-131">Se tiver êxito, este método retornará um código de resposta `201 Created`.</span><span class="sxs-lookup"><span data-stu-id="08316-131">If successful, this method returns a `201 Created` response code.</span></span>

## <a name="example"></a><span data-ttu-id="08316-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="08316-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="08316-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="08316-133">Request</span></span>

<span data-ttu-id="08316-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="08316-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs
{
  "displayName": "My Contoso Tab",
  "teamsApp@odata.bind" : "https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  }
}
```

#### <a name="response"></a><span data-ttu-id="08316-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="08316-135">Response</span></span>

<span data-ttu-id="08316-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="08316-136">The following is an example of the response.</span></span> <span data-ttu-id="08316-137">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="08316-137">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "794f0e4e-4d10-4bb5-9079-3a465a629eff",
  "displayName": "My Contoso Tab",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  },
  "sortOrderIndex": "20",
  "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3afd736d46-51ed-4c0b-9b23-e67ca354bb24?label=my%20%contoso%to%tab"
}
```

## <a name="see-also"></a><span data-ttu-id="08316-138">Confira também</span><span class="sxs-lookup"><span data-stu-id="08316-138">See also</span></span>

- [<span data-ttu-id="08316-139">Configurando os tipos de guia buit-in</span><span class="sxs-lookup"><span data-stu-id="08316-139">Configuring the buit-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
- [<span data-ttu-id="08316-140">Adicionar aplicativo à equipe</span><span class="sxs-lookup"><span data-stu-id="08316-140">Add app to team</span></span>](team-post-installedapps.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Add tab to channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


