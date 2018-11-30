---
title: Adicionar guia ao canal
description: 'Adiciona (pins) uma guia para o canal especificado dentro de uma equipe. '
ms.openlocfilehash: 1bf2021438cc9c0c74a2a4133e54a4fbc42fdf4d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005510"
---
# <a name="add-tab-to-channel"></a><span data-ttu-id="9757d-103">Adicionar guia ao canal</span><span class="sxs-lookup"><span data-stu-id="9757d-103">Add tab to channel</span></span>



<span data-ttu-id="9757d-104">Adiciona (pins) um [guia](../resources/teamstab.md) para o [canal](../resources/channel.md) especificado dentro de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="9757d-104">Adds (pins) a [tab](../resources/teamstab.md) to the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> <span data-ttu-id="9757d-105">O aplicativo correspondente já deve estar [instalado na equipe de](../api/teamsappinstallation-add.md).</span><span class="sxs-lookup"><span data-stu-id="9757d-105">The corresponding app must already be [installed in the team](../api/teamsappinstallation-add.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9757d-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="9757d-106">Permissions</span></span>
<span data-ttu-id="9757d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9757d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9757d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9757d-109">Permission type</span></span>      | <span data-ttu-id="9757d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9757d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9757d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9757d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9757d-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9757d-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9757d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9757d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9757d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9757d-114">Not supported.</span></span>    |
| <span data-ttu-id="9757d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9757d-115">Application</span></span>                            | <span data-ttu-id="9757d-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9757d-116">Group.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="9757d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9757d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/tabs
```

## <a name="request-headers"></a><span data-ttu-id="9757d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9757d-118">Request headers</span></span>
| <span data-ttu-id="9757d-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9757d-119">Header</span></span>       | <span data-ttu-id="9757d-120">Valor</span><span class="sxs-lookup"><span data-stu-id="9757d-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9757d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9757d-121">Authorization</span></span>  | <span data-ttu-id="9757d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9757d-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9757d-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9757d-124">Request body</span></span>

<span data-ttu-id="9757d-125">Um [teamsTab](../resources/teamstab.md).</span><span class="sxs-lookup"><span data-stu-id="9757d-125">A [teamsTab](../resources/teamstab.md).</span></span>

## <a name="response"></a><span data-ttu-id="9757d-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="9757d-126">Response</span></span>

<span data-ttu-id="9757d-127">Se tiver êxito, este método retornará um código de resposta `201 OK`.</span><span class="sxs-lookup"><span data-stu-id="9757d-127">If successful, this method returns a `201 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9757d-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9757d-128">Example</span></span>

#### <a name="request"></a><span data-ttu-id="9757d-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9757d-129">Request</span></span>

<span data-ttu-id="9757d-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9757d-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs
{
  "name": "My Contoso Tab",
  "teamsApp@odata.bind" : "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  }
}
```

#### <a name="response"></a><span data-ttu-id="9757d-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="9757d-131">Response</span></span>

<span data-ttu-id="9757d-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9757d-132">The following is an example of the response.</span></span> <span data-ttu-id="9757d-133">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="9757d-133">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="9757d-134">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9757d-134">All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="9757d-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="9757d-135">See also</span></span>

[<span data-ttu-id="9757d-136">Configurando os tipos de guia interna</span><span class="sxs-lookup"><span data-stu-id="9757d-136">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Add tab to channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
