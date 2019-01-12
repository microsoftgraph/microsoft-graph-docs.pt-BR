---
title: Obtenha a equipe
description: Recupere as propriedades e relacionamentos da equipe especificado.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 0221983538f14ef3f0c0439f8241974091e8dc0b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27943134"
---
# <a name="get-team"></a><span data-ttu-id="6fb93-103">Obtenha a equipe</span><span class="sxs-lookup"><span data-stu-id="6fb93-103">Get team</span></span>



<span data-ttu-id="6fb93-104">Recupere as propriedades e relacionamentos da [equipe](../resources/team.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="6fb93-104">Retrieve the properties and relationships of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6fb93-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="6fb93-105">Permissions</span></span>
<span data-ttu-id="6fb93-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6fb93-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6fb93-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6fb93-108">Permission type</span></span>      | <span data-ttu-id="6fb93-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6fb93-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6fb93-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6fb93-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6fb93-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fb93-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6fb93-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6fb93-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6fb93-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6fb93-113">Not supported.</span></span>    |
|<span data-ttu-id="6fb93-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6fb93-114">Application</span></span> | <span data-ttu-id="6fb93-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fb93-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="6fb93-116">**Observação**: Esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="6fb93-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="6fb93-117">Administradores globais e administradores de serviço de Teams da Microsoft podem acessar as equipes que eles não serão um membro do.</span><span class="sxs-lookup"><span data-stu-id="6fb93-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="6fb93-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6fb93-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6fb93-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6fb93-119">Optional query parameters</span></span>
<span data-ttu-id="6fb93-120">Este método oferece suporte a $select e $expand [OData parâmetros de consulta](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6fb93-120">This method supports the $select and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6fb93-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6fb93-121">Request headers</span></span>
| <span data-ttu-id="6fb93-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6fb93-122">Header</span></span>       | <span data-ttu-id="6fb93-123">Valor</span><span class="sxs-lookup"><span data-stu-id="6fb93-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6fb93-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="6fb93-124">Authorization</span></span>  | <span data-ttu-id="6fb93-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6fb93-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6fb93-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6fb93-127">Request body</span></span>
<span data-ttu-id="6fb93-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6fb93-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6fb93-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6fb93-129">Response</span></span>

<span data-ttu-id="6fb93-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto de [equipe](../resources/team.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6fb93-130">If successful, this method returns a `200 OK` response code and a [team](../resources/team.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6fb93-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6fb93-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="6fb93-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6fb93-132">Request</span></span>
<span data-ttu-id="6fb93-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6fb93-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
GET https://graph.microsoft.com/v1.0/teams/{id}
```
#### <a name="response"></a><span data-ttu-id="6fb93-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="6fb93-134">Response</span></span>
<span data-ttu-id="6fb93-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6fb93-135">The following is an example of the response.</span></span> 

><span data-ttu-id="6fb93-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6fb93-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
