---
title: Obter equipe
description: Recupere as propriedades e relações da equipe especificada.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: bcf63579b4ade651df30e4ace287aaa15baae6e4
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202209"
---
# <a name="get-team"></a><span data-ttu-id="1de24-103">Obter equipe</span><span class="sxs-lookup"><span data-stu-id="1de24-103">Get team</span></span>

<span data-ttu-id="1de24-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1de24-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="1de24-105">Recupere as propriedades e relações da [equipe](../resources/team.md) especificada.</span><span class="sxs-lookup"><span data-stu-id="1de24-105">Retrieve the properties and relationships of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1de24-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1de24-106">Permissions</span></span>
<span data-ttu-id="1de24-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1de24-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1de24-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1de24-109">Permission type</span></span>      | <span data-ttu-id="1de24-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1de24-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1de24-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1de24-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1de24-112">Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1de24-112">Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="1de24-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1de24-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1de24-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1de24-114">Not supported.</span></span>    |
|<span data-ttu-id="1de24-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1de24-115">Application</span></span> | <span data-ttu-id="1de24-116">TeamSettings.Read.Group *, TeamSettings.ReadWrite.Group*, Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1de24-116">TeamSettings.Read.Group *, TeamSettings.ReadWrite.Group*, Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="1de24-117">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="1de24-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="1de24-118">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="1de24-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="1de24-119">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="1de24-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="1de24-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1de24-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /teams/{team-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1de24-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1de24-121">Optional query parameters</span></span>
<span data-ttu-id="1de24-122">Este método dá suporte aos [Parâmetros de consulta OData](/graph/query-parameters) $select e $expand para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1de24-122">This method supports the $select and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1de24-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1de24-123">Request headers</span></span>
| <span data-ttu-id="1de24-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1de24-124">Header</span></span>       | <span data-ttu-id="1de24-125">Valor</span><span class="sxs-lookup"><span data-stu-id="1de24-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1de24-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="1de24-126">Authorization</span></span>  | <span data-ttu-id="1de24-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1de24-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1de24-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1de24-129">Request body</span></span>
<span data-ttu-id="1de24-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1de24-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1de24-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="1de24-131">Response</span></span>

<span data-ttu-id="1de24-132">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [team](../resources/team.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1de24-132">If successful, this method returns a `200 OK` response code and a [team](../resources/team.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1de24-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1de24-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="1de24-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1de24-134">Request</span></span>
<span data-ttu-id="1de24-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1de24-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_team"
}-->
```http
GET https://graph.microsoft.com/v1.0/teams/893075dd-2487-4122-925f-022c42e20265
```


#### <a name="response"></a><span data-ttu-id="1de24-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="1de24-136">Response</span></span>
<span data-ttu-id="1de24-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1de24-137">The following is an example of the response.</span></span> 

><span data-ttu-id="1de24-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1de24-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "isArchived": false,
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
<!-- {
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

