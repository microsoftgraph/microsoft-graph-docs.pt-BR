---
title: Equipe de atualização
description: Atualize as propriedades da equipe especificado.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 1185ad9d835f660c98d12fac8472bd6325463858
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991871"
---
# <a name="update-team"></a><span data-ttu-id="2a9b6-103">Equipe de atualização</span><span class="sxs-lookup"><span data-stu-id="2a9b6-103">Update team</span></span>



<span data-ttu-id="2a9b6-104">Atualize as propriedades da [equipe](../resources/team.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="2a9b6-104">Update the properties of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2a9b6-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="2a9b6-105">Permissions</span></span>
<span data-ttu-id="2a9b6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a9b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2a9b6-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2a9b6-108">Permission type</span></span>      | <span data-ttu-id="2a9b6-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2a9b6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2a9b6-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2a9b6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2a9b6-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a9b6-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2a9b6-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2a9b6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a9b6-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2a9b6-113">Not supported.</span></span>    |
|<span data-ttu-id="2a9b6-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2a9b6-114">Application</span></span> | <span data-ttu-id="2a9b6-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a9b6-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="2a9b6-116">**Observação**: Esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="2a9b6-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="2a9b6-117">Administradores globais e administradores de serviço de Teams da Microsoft podem acessar as equipes que eles não serão um membro do.</span><span class="sxs-lookup"><span data-stu-id="2a9b6-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="2a9b6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2a9b6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2a9b6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2a9b6-119">Request headers</span></span>
| <span data-ttu-id="2a9b6-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2a9b6-120">Header</span></span>       | <span data-ttu-id="2a9b6-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2a9b6-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2a9b6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2a9b6-122">Authorization</span></span>  | <span data-ttu-id="2a9b6-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2a9b6-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2a9b6-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2a9b6-125">Content-Type</span></span>  | <span data-ttu-id="2a9b6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2a9b6-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2a9b6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2a9b6-127">Request body</span></span>
<span data-ttu-id="2a9b6-128">No corpo da solicitação, fornece uma representação JSON do objeto de [equipe](../resources/team.md) .</span><span class="sxs-lookup"><span data-stu-id="2a9b6-128">In the request body, supply a JSON representation of [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2a9b6-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a9b6-129">Response</span></span>

<span data-ttu-id="2a9b6-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2a9b6-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2a9b6-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2a9b6-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="2a9b6-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2a9b6-132">Request</span></span>
<span data-ttu-id="2a9b6-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2a9b6-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_team"
}-->
```http
PATCH https://graph.microsoft.com/beta/teams/{id}
Content-type: application/json
Content-length: 211

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
#### <a name="response"></a><span data-ttu-id="2a9b6-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a9b6-134">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
