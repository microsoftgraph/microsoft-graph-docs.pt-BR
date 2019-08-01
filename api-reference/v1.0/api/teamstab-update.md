---
title: Atualizar guia
description: Atualiza as propriedades da guia especificada.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f2b391055dcb17af41f4bf5522b248a00caa9aa2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027164"
---
# <a name="update-tab"></a><span data-ttu-id="0e576-103">Atualizar guia</span><span class="sxs-lookup"><span data-stu-id="0e576-103">Update tab</span></span>


<span data-ttu-id="0e576-104">Atualiza as propriedades da [guia](../resources/teamstab.md)especificada. Isso pode ser usado para configurar o conteúdo da guia.</span><span class="sxs-lookup"><span data-stu-id="0e576-104">Update the properties of the specified [tab](../resources/teamstab.md). This can be used to configure the content of the tab.</span></span>

## <a name="permissions"></a><span data-ttu-id="0e576-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0e576-105">Permissions</span></span>
<span data-ttu-id="0e576-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e576-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="0e576-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0e576-108">Permission type</span></span>      | <span data-ttu-id="0e576-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0e576-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0e576-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0e576-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0e576-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e576-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0e576-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0e576-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e576-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0e576-113">Not supported.</span></span>    |
|<span data-ttu-id="0e576-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0e576-114">Application</span></span>                            | <span data-ttu-id="0e576-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e576-115">Group.ReadWrite.All</span></span>                         |

> <span data-ttu-id="0e576-116">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="0e576-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="0e576-117">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="0e576-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="0e576-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0e576-118">HTTP request</span></span>
```http
PATCH /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0e576-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0e576-119">Request headers</span></span>
| <span data-ttu-id="0e576-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0e576-120">Header</span></span>       | <span data-ttu-id="0e576-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0e576-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0e576-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0e576-122">Authorization</span></span>  | <span data-ttu-id="0e576-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0e576-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0e576-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0e576-125">Content-Type</span></span>  | <span data-ttu-id="0e576-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0e576-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0e576-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0e576-127">Request body</span></span>
<span data-ttu-id="0e576-128">No corpo da solicitação, forneça uma representação JSON do objeto [Tab](../resources/teamstab.md) .</span><span class="sxs-lookup"><span data-stu-id="0e576-128">In the request body, supply a JSON representation of [tab](../resources/teamstab.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="0e576-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e576-129">Response</span></span>

<span data-ttu-id="0e576-130">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="0e576-130">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0e576-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0e576-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="0e576-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0e576-132">Request</span></span>
<span data-ttu-id="0e576-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0e576-133">The following is an example of the request.</span></span>
```http
PATCH https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}/tabs/{id}
Content-type: application/json
Content-length: 211

{
  "displayName": "My Contoso Tab - updated"
}
```
#### <a name="response"></a><span data-ttu-id="0e576-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e576-134">Response</span></span>
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "tabId",
  "displayName": "My Contoso Tab - updated",
  "teamsApp@odata.bind": "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('06805b9e-77e3-4b93-ac81-525eb87513b8')",
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

## <a name="see-also"></a><span data-ttu-id="0e576-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="0e576-135">See also</span></span>

[<span data-ttu-id="0e576-136">Configurar tipos de guia internos</span><span class="sxs-lookup"><span data-stu-id="0e576-136">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update tab in channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->
