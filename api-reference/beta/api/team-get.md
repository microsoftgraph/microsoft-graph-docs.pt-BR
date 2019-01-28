---
title: Obter equipe
description: Recupere as propriedades e relações da equipe especificada.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: a9da6ea1bc1570f40fe4159d9c62951fca539cb5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517845"
---
# <a name="get-team"></a><span data-ttu-id="83d76-103">Obter equipe</span><span class="sxs-lookup"><span data-stu-id="83d76-103">Get team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83d76-104">Recupere as propriedades e relações da [equipe](../resources/team.md) especificada.</span><span class="sxs-lookup"><span data-stu-id="83d76-104">Retrieve the properties and relationships of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="83d76-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="83d76-105">Permissions</span></span>
<span data-ttu-id="83d76-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83d76-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83d76-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="83d76-108">Permission type</span></span>      | <span data-ttu-id="83d76-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="83d76-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="83d76-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="83d76-110">Delegated (work or school account)</span></span> | <span data-ttu-id="83d76-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83d76-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="83d76-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="83d76-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83d76-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="83d76-113">Not supported.</span></span>    |
|<span data-ttu-id="83d76-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="83d76-114">Application</span></span> | <span data-ttu-id="83d76-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83d76-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="83d76-116">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="83d76-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="83d76-117">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="83d76-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="83d76-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="83d76-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="83d76-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="83d76-119">Optional query parameters</span></span>
<span data-ttu-id="83d76-120">Este método dá suporte aos [Parâmetros de consulta OData](/graph/query-parameters) $select e $expand para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="83d76-120">This method supports the $select and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="83d76-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="83d76-121">Request headers</span></span>
| <span data-ttu-id="83d76-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="83d76-122">Header</span></span>       | <span data-ttu-id="83d76-123">Valor</span><span class="sxs-lookup"><span data-stu-id="83d76-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="83d76-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="83d76-124">Authorization</span></span>  | <span data-ttu-id="83d76-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="83d76-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="83d76-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="83d76-127">Request body</span></span>
<span data-ttu-id="83d76-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="83d76-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="83d76-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="83d76-129">Response</span></span>

<span data-ttu-id="83d76-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [team](../resources/team.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="83d76-130">If successful, this method returns a `200 OK` response code and a [deviceManagementExchangeConnector](../resources/team.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="83d76-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="83d76-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="83d76-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="83d76-132">Request</span></span>
<span data-ttu-id="83d76-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="83d76-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}
```
#### <a name="response"></a><span data-ttu-id="83d76-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="83d76-134">Response</span></span>
<span data-ttu-id="83d76-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="83d76-135">The following is an example of the response.</span></span> 

><span data-ttu-id="83d76-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="83d76-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/team-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
