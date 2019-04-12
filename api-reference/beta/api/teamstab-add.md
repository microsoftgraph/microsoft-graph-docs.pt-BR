---
title: Adicionar uma guia ao canal
description: 'Adiciona (pins) a uma guia para o canal especificado dentro de uma equipe. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 8a1caf00f16fc1f4384977913073623b02d2a33a
ms.sourcegitcommit: 0a673c6f4ad7aed12fb0e69608c0f73957bae10e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/12/2019
ms.locfileid: "31824413"
---
# <a name="add-tab-to-channel"></a><span data-ttu-id="97805-103">Adicionar uma guia ao canal</span><span class="sxs-lookup"><span data-stu-id="97805-103">Add tab to channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97805-104">Adiciona (pins) a uma [guia](../resources/teamstab.md) para o canal [especificado](../resources/channel.md) dentro de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="97805-104">Adds (pins) a [tab](../resources/teamstab.md) to the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> <span data-ttu-id="97805-105">O aplicativo correspondente já deve estar [instalado na equipe](../api/teamsappinstallation-add.md).</span><span class="sxs-lookup"><span data-stu-id="97805-105">The corresponding app must already be [installed in the team](../api/teamsappinstallation-add.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="97805-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="97805-106">Permissions</span></span>
<span data-ttu-id="97805-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97805-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97805-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="97805-109">Permission type</span></span>      | <span data-ttu-id="97805-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="97805-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="97805-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="97805-111">Delegated (work or school account)</span></span> | <span data-ttu-id="97805-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97805-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="97805-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="97805-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97805-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97805-114">Not supported.</span></span>    |
| <span data-ttu-id="97805-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="97805-115">Application</span></span>                            | <span data-ttu-id="97805-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97805-116">Group.ReadWrite.All</span></span>                         |

> <span data-ttu-id="97805-117">**Observação**: esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="97805-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="97805-118">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="97805-118">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="97805-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="97805-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/tabs
```

## <a name="request-headers"></a><span data-ttu-id="97805-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="97805-120">Request headers</span></span>
| <span data-ttu-id="97805-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="97805-121">Header</span></span>       | <span data-ttu-id="97805-122">Valor</span><span class="sxs-lookup"><span data-stu-id="97805-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="97805-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="97805-123">Authorization</span></span>  | <span data-ttu-id="97805-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97805-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="97805-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="97805-126">Request body</span></span>

<span data-ttu-id="97805-127">Uma [teamsTab](../resources/teamstab.md).</span><span class="sxs-lookup"><span data-stu-id="97805-127">A [teamsTab](../resources/teamstab.md).</span></span>

## <a name="response"></a><span data-ttu-id="97805-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="97805-128">Response</span></span>

<span data-ttu-id="97805-129">Se tiver êxito, este método retornará um código de resposta `201 Created`.</span><span class="sxs-lookup"><span data-stu-id="97805-129">If successful, this method returns a `201 Created` response code.</span></span>

## <a name="example"></a><span data-ttu-id="97805-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="97805-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="97805-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97805-131">Request</span></span>

<span data-ttu-id="97805-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="97805-132">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="97805-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="97805-133">Response</span></span>

<span data-ttu-id="97805-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="97805-134">The following is an example of the response.</span></span> <span data-ttu-id="97805-135">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="97805-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="97805-136">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="97805-136">All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="97805-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="97805-137">See also</span></span>

[<span data-ttu-id="97805-138">Configurar tipos de guia internos</span><span class="sxs-lookup"><span data-stu-id="97805-138">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Add tab to channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/teamstab-add.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
