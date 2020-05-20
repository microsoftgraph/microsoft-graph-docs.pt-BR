---
title: Atualizar guia
description: Atualiza as propriedades da guia especificada.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: d0694e100f36ae6e806bed30c88664cc21becc09
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290241"
---
# <a name="update-tab"></a><span data-ttu-id="5f306-103">Atualizar guia</span><span class="sxs-lookup"><span data-stu-id="5f306-103">Update tab</span></span>

<span data-ttu-id="5f306-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f306-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="5f306-105">Atualiza as propriedades da [guia](../resources/teamstab.md)especificada. Isso pode ser usado para configurar o conteúdo da guia.</span><span class="sxs-lookup"><span data-stu-id="5f306-105">Update the properties of the specified [tab](../resources/teamstab.md). This can be used to configure the content of the tab.</span></span>

## <a name="permissions"></a><span data-ttu-id="5f306-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5f306-106">Permissions</span></span>
<span data-ttu-id="5f306-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f306-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5f306-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5f306-109">Permission type</span></span>      | <span data-ttu-id="5f306-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5f306-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5f306-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5f306-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5f306-112">TeamsTab. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="5f306-112">TeamsTab.ReadWrite.All, Group.ReadWrite.All</span></span> |
|<span data-ttu-id="5f306-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5f306-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f306-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5f306-114">Not supported.</span></span>    |
|<span data-ttu-id="5f306-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5f306-115">Application</span></span>                            | <span data-ttu-id="5f306-116">TeamsTab. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="5f306-116">TeamsTab.ReadWrite.All, Group.ReadWrite.All</span></span> |

<span data-ttu-id="5f306-117">| Delegado (conta corporativa ou de estudante) | TeamsTab. ReadWrite. All, Group. ReadWrite. All, Directory. ReadWrite. All | | Delegado (conta pessoal da Microsoft) | Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5f306-117">|Delegated (work or school account) | TeamsTab.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All | |Delegated (personal Microsoft account) | Not supported.</span></span>    <span data-ttu-id="5f306-118">| | Aplicativo | TeamsTab. Edit. Group ([RSC](https://aka.ms/teams-rsc)), TeamsTab. ReadWrite. All, Group. ReadWrite. All, Directory. ReadWrite. All |</span><span class="sxs-lookup"><span data-stu-id="5f306-118">| |Application | TeamsTab.Edit.Group ([RSC](https://aka.ms/teams-rsc)), TeamsTab.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All |</span></span>

> <span data-ttu-id="5f306-119">**Observação**: esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="5f306-119">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="5f306-120">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="5f306-120">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="5f306-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5f306-121">HTTP request</span></span>
```http
PATCH /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5f306-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5f306-122">Request headers</span></span>
| <span data-ttu-id="5f306-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5f306-123">Header</span></span>       | <span data-ttu-id="5f306-124">Valor</span><span class="sxs-lookup"><span data-stu-id="5f306-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5f306-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="5f306-125">Authorization</span></span>  | <span data-ttu-id="5f306-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5f306-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5f306-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5f306-128">Content-Type</span></span>  | <span data-ttu-id="5f306-129">application/json</span><span class="sxs-lookup"><span data-stu-id="5f306-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5f306-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5f306-130">Request body</span></span>
<span data-ttu-id="5f306-131">No corpo da solicitação, forneça uma representação JSON do objeto [Tab](../resources/teamstab.md) .</span><span class="sxs-lookup"><span data-stu-id="5f306-131">In the request body, supply a JSON representation of [tab](../resources/teamstab.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="5f306-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f306-132">Response</span></span>

<span data-ttu-id="5f306-133">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="5f306-133">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5f306-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5f306-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="5f306-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5f306-135">Request</span></span>
<span data-ttu-id="5f306-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5f306-136">The following is an example of the request.</span></span>
```http
PATCH https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}/tabs/{id}
Content-type: application/json
Content-length: 211

{
  "displayName": "My Contoso Tab - updated"
}
```
#### <a name="response"></a><span data-ttu-id="5f306-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f306-137">Response</span></span>
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

## <a name="see-also"></a><span data-ttu-id="5f306-138">Confira também</span><span class="sxs-lookup"><span data-stu-id="5f306-138">See also</span></span>

[<span data-ttu-id="5f306-139">Configurar tipos de guia internos</span><span class="sxs-lookup"><span data-stu-id="5f306-139">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)

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
