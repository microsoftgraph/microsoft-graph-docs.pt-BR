---
title: Obter equipe
description: Recupere as propriedades e relações da equipe especificada.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c8d1129c57444d95a1a3a46ee58590e102056a98
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290094"
---
# <a name="get-team"></a><span data-ttu-id="33401-103">Obter equipe</span><span class="sxs-lookup"><span data-stu-id="33401-103">Get team</span></span>

<span data-ttu-id="33401-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33401-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33401-105">Recupere as propriedades e relações da [equipe](../resources/team.md) especificada.</span><span class="sxs-lookup"><span data-stu-id="33401-105">Retrieve the properties and relationships of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="33401-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="33401-106">Permissions</span></span>
<span data-ttu-id="33401-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33401-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33401-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="33401-109">Permission type</span></span>      | <span data-ttu-id="33401-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="33401-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="33401-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="33401-111">Delegated (work or school account)</span></span> | <span data-ttu-id="33401-112">Team. ReadBasic. All, TeamSettings. Read. All, TeamSettings. ReadWrite. All, Group. Read. All, Group. ReadWrite. All, Directory. Read. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="33401-112">Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="33401-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="33401-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33401-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="33401-114">Not supported.</span></span>    |
|<span data-ttu-id="33401-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="33401-115">Application</span></span> | <span data-ttu-id="33401-116">TeamSettings. Read. Group ([RSC](https://aka.ms/teams-rsc)), Team. ReadBasic. All, TeamSettings. Read. All, TeamSettings. ReadWrite. All, TeamSettings. Edit. Group ([RSC](https://aka.ms/teams-rsc)), Group. Read. All, Group. ReadWrite. All, Directory. Read. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="33401-116">TeamSettings.Read.Group ([RSC](https://aka.ms/teams-rsc)), Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, TeamSettings.Edit.Group ([RSC](https://aka.ms/teams-rsc)), Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span>    |

> <span data-ttu-id="33401-117">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="33401-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="33401-118">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="33401-118">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="33401-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="33401-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="33401-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="33401-120">Optional query parameters</span></span>
<span data-ttu-id="33401-121">Este método dá suporte aos [Parâmetros de consulta OData](/graph/query-parameters) $select e $expand para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="33401-121">This method supports the $select and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="33401-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="33401-122">Request headers</span></span>
| <span data-ttu-id="33401-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="33401-123">Header</span></span>       | <span data-ttu-id="33401-124">Valor</span><span class="sxs-lookup"><span data-stu-id="33401-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="33401-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="33401-125">Authorization</span></span>  | <span data-ttu-id="33401-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="33401-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="33401-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="33401-128">Request body</span></span>
<span data-ttu-id="33401-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="33401-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="33401-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="33401-130">Response</span></span>

<span data-ttu-id="33401-131">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [team](../resources/team.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="33401-131">If successful, this method returns a `200 OK` response code and a [team](../resources/team.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="33401-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="33401-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="33401-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="33401-133">Request</span></span>
<span data-ttu-id="33401-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="33401-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}
```
#### <a name="response"></a><span data-ttu-id="33401-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="33401-135">Response</span></span>
<span data-ttu-id="33401-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="33401-136">The following is an example of the response.</span></span> 

><span data-ttu-id="33401-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="33401-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "isArchived" : false,
  "memberSettings": {
    "allowCreateUpdateChannels": true,
    "allowDeleteChannels": true,
    "allowAddRemoveApps": true,
    "allowCreateUpdateRemoveTabs": true,
    "allowCreateUpdateRemoveConnectors": true    
  },
  "guestSettings": {
    "allowCreateUpdateChannels": true,
    "allowDeleteChannels": true 
  },
  "messagingSettings": {
    "allowUserEditMessages": true,
    "allowUserDeleteMessages": true,
    "allowOwnerDeleteMessages": true,
    "allowTeamMentions": true,
    "allowChannelMentions": true    
  },
  "funSettings": {
    "allowGiphy": true,
    "giphyContentRating": "strict",
    "allowStickersAndMemes": true,
    "allowCustomMemes": true
  },
  "discoverySettings": {
    "showInTeamsSearchAndSuggestions": true
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
