---
title: Criar equipe
description: Crie uma nova equipe em um grupo.
ms.openlocfilehash: d7afffb331bf4a1714083ebb5f95147ec48a65d0
ms.sourcegitcommit: 72d4da2a6bfaf99fa4edaf6ce3b97b1a6d96d874
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2018
ms.locfileid: "27222545"
---
# <a name="create-team"></a><span data-ttu-id="31150-103">Criar equipe</span><span class="sxs-lookup"><span data-stu-id="31150-103">Create team</span></span>



<span data-ttu-id="31150-104">Crie uma nova [equipe](../resources/team.md) em um [grupo](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="31150-104">Create a new [team](../resources/team.md) under a [group](../resources/group.md).</span></span>

<span data-ttu-id="31150-105">Para criar uma equipe, o grupo deve ter um mínimo de um proprietário.</span><span class="sxs-lookup"><span data-stu-id="31150-105">In order to create a team, the group must have a least one owner.</span></span>

<span data-ttu-id="31150-106">Se o grupo foi criado há menos de 15 minutos, é possível para a chamada de equipe criar falha com um código de 404 erro devido aos atrasos de replicação.</span><span class="sxs-lookup"><span data-stu-id="31150-106">If the group was created less than 15 minutes ago, it's possible for the Create team call to fail with a 404 error code due to replication delays.</span></span> <span data-ttu-id="31150-107">O padrão recomendado é repetir a chamada de equipe criar três vezes, com um atraso de segunda 10 entre chamadas.</span><span class="sxs-lookup"><span data-stu-id="31150-107">The recommended pattern is to retry the Create team call three times, with a 10 second delay between calls.</span></span>

## <a name="permissions"></a><span data-ttu-id="31150-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="31150-108">Permissions</span></span>

<span data-ttu-id="31150-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31150-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31150-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="31150-111">Permission type</span></span>      | <span data-ttu-id="31150-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="31150-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="31150-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="31150-113">Delegated (work or school account)</span></span> | <span data-ttu-id="31150-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31150-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="31150-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="31150-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31150-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="31150-116">Not supported.</span></span>    |
|<span data-ttu-id="31150-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="31150-117">Application</span></span> | <span data-ttu-id="31150-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31150-118">Group.ReadWrite.All</span></span> |

> <span data-ttu-id="31150-119">**Observação**: Esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="31150-119">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="31150-120">Administradores globais e administradores de serviço de Teams da Microsoft podem acessar que eles não são membros de grupos.</span><span class="sxs-lookup"><span data-stu-id="31150-120">Global admins and Microsoft Teams service admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="31150-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="31150-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /groups/{id}/team
```

## <a name="request-headers"></a><span data-ttu-id="31150-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="31150-122">Request headers</span></span>

| <span data-ttu-id="31150-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="31150-123">Header</span></span>       | <span data-ttu-id="31150-124">Valor</span><span class="sxs-lookup"><span data-stu-id="31150-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="31150-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="31150-125">Authorization</span></span>  | <span data-ttu-id="31150-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="31150-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="31150-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="31150-128">Content-Type</span></span>  | <span data-ttu-id="31150-129">application/json</span><span class="sxs-lookup"><span data-stu-id="31150-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="31150-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="31150-130">Request body</span></span>

<span data-ttu-id="31150-131">No corpo da solicitação, fornece uma representação JSON de um objeto de [equipe](../resources/team.md) .</span><span class="sxs-lookup"><span data-stu-id="31150-131">In the request body, supply a JSON representation of a [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="31150-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="31150-132">Response</span></span>

<span data-ttu-id="31150-133">Se tiver êxito, esse método deve retornar uma `201 Created` código de resposta e um objeto de [equipe](../resources/team.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="31150-133">If successful, this method should return a `201 Created` response code and a [team](../resources/team.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31150-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="31150-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="31150-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="31150-135">Request</span></span>

<span data-ttu-id="31150-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="31150-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "create_team"
}-->
```http
PUT https://graph.microsoft.com/v1.0/groups/{id}/team
Content-type: application/json

{  
  "memberSettings": {
    "allowCreateUpdateChannels": true
  },
  "messagingSettings": {
    "allowUserEditMessages": true,
    "allowUserDeleteMessages": true
  },
  "funSettings": {
    "allowGiphy": true,
    "giphyContentRating": "strict"
  }
}
```

#### <a name="response"></a><span data-ttu-id="31150-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="31150-137">Response</span></span>

<span data-ttu-id="31150-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="31150-138">The following is an example of the response.</span></span> 

><span data-ttu-id="31150-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="31150-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 401

{
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
  "description": "Create Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

## <a name="see-also"></a><span data-ttu-id="31150-141">Confira também</span><span class="sxs-lookup"><span data-stu-id="31150-141">See also</span></span>

- [<span data-ttu-id="31150-142">Criando um grupo com uma equipe</span><span class="sxs-lookup"><span data-stu-id="31150-142">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
