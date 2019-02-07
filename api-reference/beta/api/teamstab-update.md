---
title: Guia de atualização
description: Atualize as propriedades da guia especificada.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 7a87839a1a6a151708b485d8c3fec9657f21f11a
ms.sourcegitcommit: 255061099661a38278140675db4cbadbdca9be7c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/07/2019
ms.locfileid: "29760962"
---
# <a name="update-tab"></a><span data-ttu-id="e7629-103">Guia de atualização</span><span class="sxs-lookup"><span data-stu-id="e7629-103">Update tab</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7629-104">Atualize as propriedades da [guia](../resources/teamstab.md)especificado. Isso pode ser usado para configurar o conteúdo da guia.</span><span class="sxs-lookup"><span data-stu-id="e7629-104">Update the properties of the specified [tab](../resources/teamstab.md). This can be used to configure the content of the tab.</span></span>

## <a name="permissions"></a><span data-ttu-id="e7629-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e7629-105">Permissions</span></span>
<span data-ttu-id="e7629-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7629-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e7629-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e7629-108">Permission type</span></span>      | <span data-ttu-id="e7629-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e7629-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e7629-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e7629-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e7629-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7629-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e7629-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e7629-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7629-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7629-113">Not supported.</span></span>    |
|<span data-ttu-id="e7629-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e7629-114">Application</span></span>                            | <span data-ttu-id="e7629-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7629-115">Group.ReadWrite.All</span></span>                         |

> <span data-ttu-id="e7629-116">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="e7629-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="e7629-117">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="e7629-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="e7629-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e7629-118">HTTP request</span></span>
```http
PATCH /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e7629-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e7629-119">Request headers</span></span>
| <span data-ttu-id="e7629-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e7629-120">Header</span></span>       | <span data-ttu-id="e7629-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e7629-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e7629-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e7629-122">Authorization</span></span>  | <span data-ttu-id="e7629-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e7629-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e7629-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e7629-125">Content-Type</span></span>  | <span data-ttu-id="e7629-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e7629-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e7629-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e7629-127">Request body</span></span>
<span data-ttu-id="e7629-128">No corpo da solicitação, fornece uma representação de JSON do objeto [tab](../resources/teamstab.md) .</span><span class="sxs-lookup"><span data-stu-id="e7629-128">In the request body, supply a JSON representation of [tab](../resources/teamstab.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e7629-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7629-129">Response</span></span>

<span data-ttu-id="e7629-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e7629-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e7629-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e7629-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="e7629-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7629-132">Request</span></span>
<span data-ttu-id="e7629-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e7629-133">The following is an example of the request.</span></span>
```http
PATCH https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}
Content-type: application/json
Content-length: 211

{
  "displayName": "My Contoso Tab - updated"
}
```
#### <a name="response"></a><span data-ttu-id="e7629-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7629-134">Response</span></span>
```http
HTTP/1.1 200 Success
Content-type: application/json

{
  "id": "tabId",
  "displayName": "My Contoso Tab - updated",
  "teamsAppId": "06805b9e-77e3-4b93-ac81-525eb87513b8",
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

## <a name="see-also"></a><span data-ttu-id="e7629-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="e7629-135">See also</span></span>

[<span data-ttu-id="e7629-136">Configurar tipos de guia internos</span><span class="sxs-lookup"><span data-stu-id="e7629-136">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update tab in channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/teamstab-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
