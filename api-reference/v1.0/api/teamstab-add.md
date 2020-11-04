---
title: Adicionar uma guia ao canal
description: 'Adiciona (pins) a uma guia para o canal especificado dentro de uma equipe. '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 66ecaf63afe7a5d53915d2a77a72fae73e43483a
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2020
ms.locfileid: "48848707"
---
# <a name="add-tab-to-channel"></a><span data-ttu-id="615c9-103">Adicionar uma guia ao canal</span><span class="sxs-lookup"><span data-stu-id="615c9-103">Add tab to channel</span></span>

<span data-ttu-id="615c9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="615c9-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="615c9-105">Adiciona (pins) a uma [guia](../resources/teamstab.md) para o canal [especificado](../resources/channel.md) dentro de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="615c9-105">Adds (pins) a [tab](../resources/teamstab.md) to the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> <span data-ttu-id="615c9-106">O aplicativo correspondente já deve estar [instalado na equipe](../api/teamsappinstallation-add.md).</span><span class="sxs-lookup"><span data-stu-id="615c9-106">The corresponding app must already be [installed in the team](../api/teamsappinstallation-add.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="615c9-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="615c9-107">Permissions</span></span>
<span data-ttu-id="615c9-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="615c9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="615c9-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="615c9-110">Permission type</span></span>      | <span data-ttu-id="615c9-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="615c9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="615c9-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="615c9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="615c9-113">TeamsTab.Create, TeamsTab.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="615c9-113">TeamsTab.Create, TeamsTab.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="615c9-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="615c9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="615c9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="615c9-115">Not supported.</span></span>    |
| <span data-ttu-id="615c9-116">Application</span><span class="sxs-lookup"><span data-stu-id="615c9-116">Application</span></span>                            | <span data-ttu-id="615c9-117">TeamsTab.Create.Group\*, TeamsTab.Create, TeamsTab.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="615c9-117">TeamsTab.Create.Group\*, TeamsTab.Create, TeamsTab.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="615c9-118">**Observação** : Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="615c9-118">**Note** : Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="615c9-119">**Observação** : esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="615c9-119">**Note** : This API supports admin permissions.</span></span> <span data-ttu-id="615c9-120">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="615c9-120">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="615c9-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="615c9-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/tabs
```

## <a name="request-headers"></a><span data-ttu-id="615c9-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="615c9-122">Request headers</span></span>
| <span data-ttu-id="615c9-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="615c9-123">Header</span></span>       | <span data-ttu-id="615c9-124">Valor</span><span class="sxs-lookup"><span data-stu-id="615c9-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="615c9-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="615c9-125">Authorization</span></span>  | <span data-ttu-id="615c9-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="615c9-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="615c9-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="615c9-128">Request body</span></span>

<span data-ttu-id="615c9-129">Uma [teamsTab](../resources/teamstab.md).</span><span class="sxs-lookup"><span data-stu-id="615c9-129">A [teamsTab](../resources/teamstab.md).</span></span>

## <a name="response"></a><span data-ttu-id="615c9-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="615c9-130">Response</span></span>

<span data-ttu-id="615c9-131">Se tiver êxito, este método retornará um código de resposta `201 Created`.</span><span class="sxs-lookup"><span data-stu-id="615c9-131">If successful, this method returns a `201 Created` response code.</span></span>

## <a name="example"></a><span data-ttu-id="615c9-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="615c9-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="615c9-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="615c9-133">Request</span></span>

<span data-ttu-id="615c9-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="615c9-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}/tabs
{
  "displayName": "My Contoso Tab",
  "teamsApp@odata.bind" : "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  }
}
```

#### <a name="response"></a><span data-ttu-id="615c9-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="615c9-135">Response</span></span>

<span data-ttu-id="615c9-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="615c9-136">The following is an example of the response.</span></span> <span data-ttu-id="615c9-137">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="615c9-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="615c9-138">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="615c9-138">All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="615c9-139">Confira também</span><span class="sxs-lookup"><span data-stu-id="615c9-139">See also</span></span>

[<span data-ttu-id="615c9-140">Configurar tipos de guia internos</span><span class="sxs-lookup"><span data-stu-id="615c9-140">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Add tab to channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->

