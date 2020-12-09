---
title: Guia obter no canal
description: 'Recupere as propriedades e as relações da guia especificada em um canal de uma equipe. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ee05de9b1fcfea9bd08c98ccf3f8a491b34c0399
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607473"
---
# <a name="get-tab-in-channel"></a><span data-ttu-id="d82a5-103">Guia obter no canal</span><span class="sxs-lookup"><span data-stu-id="d82a5-103">Get tab in channel</span></span>

<span data-ttu-id="d82a5-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d82a5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d82a5-105">Recupere as propriedades e as relações da [guia](../resources/teamstab.md) especificada em um [canal](../resources/channel.md) de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="d82a5-105">Retrieve the properties and relationships of the specified [tab](../resources/teamstab.md) in a [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="d82a5-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="d82a5-106">Permissions</span></span>
<span data-ttu-id="d82a5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d82a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d82a5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d82a5-109">Permission type</span></span>      | <span data-ttu-id="d82a5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d82a5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d82a5-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d82a5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d82a5-112">TeamsTab. Read. All, TeamsTab. ReadWriteForTeam, TeamsTab. ReadWrite. All, Group. Read. All, Group. ReadWrite. All, Directory. Read. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="d82a5-112">TeamsTab.Read.All, TeamsTab.ReadWriteForTeam, TeamsTab.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="d82a5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d82a5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d82a5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d82a5-114">Not supported.</span></span>    |
|<span data-ttu-id="d82a5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d82a5-115">Application</span></span> | <span data-ttu-id="d82a5-116">TeamsTab. Read. Group *, TeamsTab. ReadWrite. Group*, TeamsTab. Read. All, TeamsTab. ReadWriteForTeam. All, TeamsTab. ReadWrite. All, Group. Read. All, Group. ReadWrite. All, Directory. Read. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="d82a5-116">TeamsTab.Read.Group *, TeamsTab.ReadWrite.Group*, TeamsTab.Read.All, TeamsTab.ReadWriteForTeam.All, TeamsTab.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="d82a5-117">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="d82a5-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="d82a5-118">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="d82a5-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="d82a5-119">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="d82a5-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="d82a5-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d82a5-120">HTTP request</span></span>
```http
GET /teams/{team-id}/channels/{channel-id}/tabs/{tab-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d82a5-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d82a5-121">Optional query parameters</span></span>

<span data-ttu-id="d82a5-122">Este método dá suporte ao $select e $expand [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d82a5-122">This method supports the $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d82a5-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d82a5-123">Request headers</span></span>
| <span data-ttu-id="d82a5-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d82a5-124">Header</span></span>       | <span data-ttu-id="d82a5-125">Valor</span><span class="sxs-lookup"><span data-stu-id="d82a5-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d82a5-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="d82a5-126">Authorization</span></span>  | <span data-ttu-id="d82a5-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d82a5-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d82a5-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d82a5-129">Request body</span></span>
<span data-ttu-id="d82a5-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d82a5-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d82a5-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d82a5-131">Response</span></span>

<span data-ttu-id="d82a5-132">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [Tab](../resources/teamstab.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d82a5-132">If successful, this method returns a `200 OK` response code and a [tab](../resources/teamstab.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d82a5-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d82a5-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="d82a5-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d82a5-134">Request</span></span>
<span data-ttu-id="d82a5-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d82a5-135">The following is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}?$expand=teamsApp
```
#### <a name="response"></a><span data-ttu-id="d82a5-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d82a5-136">Response</span></span>
<span data-ttu-id="d82a5-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d82a5-137">The following is an example of the response.</span></span> 

><span data-ttu-id="d82a5-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d82a5-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "id": "tabId",
  "displayName": "My Contoso Tab - updated",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  },
  "teamsApp": {
      "id": "0d820ecd-def2-4297-adad-78056cde7c78",
      "externalId": null,
      "displayName": "Contoso",
      "distributionMethod": "store"
  },
  "sortOrderIndex": "20",
  "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3afd736d46-51ed-4c0b-9b23-e67ca354bb24?label=my%20%contoso%to%tab"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get a channel tab",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


