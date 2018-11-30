---
title: Adicionar guia ao canal
description: 'Adiciona (pins) uma guia para o canal especificado dentro de uma equipe. '
ms.openlocfilehash: be246b0308be83e0b411fa89fe16034018756829
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034721"
---
# <a name="add-tab-to-channel"></a><span data-ttu-id="bda10-103">Adicionar guia ao canal</span><span class="sxs-lookup"><span data-stu-id="bda10-103">Add tab to channel</span></span>

> <span data-ttu-id="bda10-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bda10-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bda10-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bda10-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bda10-106">Adiciona (pins) um [guia](../resources/teamstab.md) para o [canal](../resources/channel.md) especificado dentro de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="bda10-106">Adds (pins) a [tab](../resources/teamstab.md) to the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> <span data-ttu-id="bda10-107">O aplicativo correspondente já deve estar [instalado na equipe de](../api/teamsappinstallation-add.md).</span><span class="sxs-lookup"><span data-stu-id="bda10-107">The corresponding app must already be [installed in the team](../api/teamsappinstallation-add.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bda10-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="bda10-108">Permissions</span></span>
<span data-ttu-id="bda10-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bda10-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bda10-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bda10-111">Permission type</span></span>      | <span data-ttu-id="bda10-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bda10-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bda10-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bda10-113">Delegated (work or school account)</span></span> | <span data-ttu-id="bda10-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bda10-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="bda10-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bda10-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bda10-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bda10-116">Not supported.</span></span>    |
| <span data-ttu-id="bda10-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bda10-117">Application</span></span>                            | <span data-ttu-id="bda10-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bda10-118">Group.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="bda10-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bda10-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/tabs
```

## <a name="request-headers"></a><span data-ttu-id="bda10-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bda10-120">Request headers</span></span>
| <span data-ttu-id="bda10-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bda10-121">Header</span></span>       | <span data-ttu-id="bda10-122">Valor</span><span class="sxs-lookup"><span data-stu-id="bda10-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bda10-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bda10-123">Authorization</span></span>  | <span data-ttu-id="bda10-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bda10-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bda10-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bda10-126">Request body</span></span>

<span data-ttu-id="bda10-127">Um [teamsTab](../resources/teamstab.md).</span><span class="sxs-lookup"><span data-stu-id="bda10-127">A [teamsTab](../resources/teamstab.md).</span></span>

## <a name="response"></a><span data-ttu-id="bda10-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="bda10-128">Response</span></span>

<span data-ttu-id="bda10-129">Se tiver êxito, este método retornará um código de resposta `201 OK`.</span><span class="sxs-lookup"><span data-stu-id="bda10-129">If successful, this method returns a `201 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="bda10-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bda10-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="bda10-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bda10-131">Request</span></span>

<span data-ttu-id="bda10-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bda10-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs
{
  "name": "My Contoso Tab",
  "teamsApp@odata.bind" : "https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  }
}
```

#### <a name="response"></a><span data-ttu-id="bda10-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="bda10-133">Response</span></span>

<span data-ttu-id="bda10-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bda10-134">The following is an example of the response.</span></span> <span data-ttu-id="bda10-135">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="bda10-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="bda10-136">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bda10-136">All of the properties will be returned from an actual call.</span></span>
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
  "name": "My Contoso Tab",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  },
  "sortOrderIndex": 20,
  "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3afd736d46-51ed-4c0b-9b23-e67ca354bb24?label=my%20%contoso%to%tab"
}
```

## <a name="see-also"></a><span data-ttu-id="bda10-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="bda10-137">See also</span></span>

[<span data-ttu-id="bda10-138">Configurando os tipos de guia interna</span><span class="sxs-lookup"><span data-stu-id="bda10-138">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Add tab to channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
