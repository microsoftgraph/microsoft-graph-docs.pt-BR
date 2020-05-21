---
title: Adicionar uma guia ao canal
description: 'Adiciona (pins) a uma guia para o canal especificado dentro de uma equipe. '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: cd4b91dc2a1083f880cd0db7db595cc939f22db8
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290592"
---
# <a name="add-tab-to-channel"></a><span data-ttu-id="1c86f-103">Adicionar uma guia ao canal</span><span class="sxs-lookup"><span data-stu-id="1c86f-103">Add tab to channel</span></span>

<span data-ttu-id="1c86f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c86f-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="1c86f-105">Adiciona (pins) a uma [guia](../resources/teamstab.md) para o canal [especificado](../resources/channel.md) dentro de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="1c86f-105">Adds (pins) a [tab](../resources/teamstab.md) to the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> <span data-ttu-id="1c86f-106">O aplicativo correspondente já deve estar [instalado na equipe](../api/teamsappinstallation-add.md).</span><span class="sxs-lookup"><span data-stu-id="1c86f-106">The corresponding app must already be [installed in the team](../api/teamsappinstallation-add.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1c86f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="1c86f-107">Permissions</span></span>
<span data-ttu-id="1c86f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c86f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c86f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1c86f-110">Permission type</span></span>      | <span data-ttu-id="1c86f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1c86f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1c86f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1c86f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1c86f-113">TeamsTab. Create, TeamsTab. ReadWrite. All, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="1c86f-113">TeamsTab.Create, TeamsTab.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="1c86f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1c86f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c86f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1c86f-115">Not supported.</span></span>    |
| <span data-ttu-id="1c86f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1c86f-116">Application</span></span>                            | <span data-ttu-id="1c86f-117">TeamsTab. Create. Group ([RSC](https://aka.ms/teams-rsc)), TeamsTab. Create, TeamsTab. ReadWrite. All, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="1c86f-117">TeamsTab.Create.Group ([RSC](https://aka.ms/teams-rsc)), TeamsTab.Create, TeamsTab.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="1c86f-118">**Observação**: esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="1c86f-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="1c86f-119">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="1c86f-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="1c86f-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1c86f-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/tabs
```

## <a name="request-headers"></a><span data-ttu-id="1c86f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1c86f-121">Request headers</span></span>
| <span data-ttu-id="1c86f-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1c86f-122">Header</span></span>       | <span data-ttu-id="1c86f-123">Valor</span><span class="sxs-lookup"><span data-stu-id="1c86f-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1c86f-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="1c86f-124">Authorization</span></span>  | <span data-ttu-id="1c86f-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1c86f-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1c86f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1c86f-127">Request body</span></span>

<span data-ttu-id="1c86f-128">Uma [teamsTab](../resources/teamstab.md).</span><span class="sxs-lookup"><span data-stu-id="1c86f-128">A [teamsTab](../resources/teamstab.md).</span></span>

## <a name="response"></a><span data-ttu-id="1c86f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c86f-129">Response</span></span>

<span data-ttu-id="1c86f-130">Se tiver êxito, este método retornará um código de resposta `201 Created`.</span><span class="sxs-lookup"><span data-stu-id="1c86f-130">If successful, this method returns a `201 Created` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1c86f-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1c86f-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="1c86f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1c86f-132">Request</span></span>

<span data-ttu-id="1c86f-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1c86f-133">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="1c86f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c86f-134">Response</span></span>

<span data-ttu-id="1c86f-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1c86f-135">The following is an example of the response.</span></span> <span data-ttu-id="1c86f-136">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="1c86f-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="1c86f-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1c86f-137">All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="1c86f-138">Confira também</span><span class="sxs-lookup"><span data-stu-id="1c86f-138">See also</span></span>

[<span data-ttu-id="1c86f-139">Configurar tipos de guia internos</span><span class="sxs-lookup"><span data-stu-id="1c86f-139">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)

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
