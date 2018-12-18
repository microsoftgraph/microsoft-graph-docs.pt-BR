---
title: Equipe de atualização
description: Atualize as propriedades da equipe especificado.
author: nkramer
ms.openlocfilehash: ff2d4f9c32ff68f865c446fc5f86781f4527f075
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314263"
---
# <a name="update-team"></a><span data-ttu-id="d4969-103">Equipe de atualização</span><span class="sxs-lookup"><span data-stu-id="d4969-103">Update team</span></span>



<span data-ttu-id="d4969-104">Atualize as propriedades da [equipe](../resources/team.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="d4969-104">Update the properties of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d4969-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d4969-105">Permissions</span></span>
<span data-ttu-id="d4969-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4969-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d4969-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d4969-108">Permission type</span></span>      | <span data-ttu-id="d4969-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d4969-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d4969-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d4969-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d4969-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4969-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d4969-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d4969-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4969-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d4969-113">Not supported.</span></span>    |
|<span data-ttu-id="d4969-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d4969-114">Application</span></span> | <span data-ttu-id="d4969-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4969-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="d4969-116">**Observação**: Esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="d4969-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="d4969-117">Administradores globais e administradores de serviço de Teams da Microsoft podem acessar as equipes que eles não serão um membro do.</span><span class="sxs-lookup"><span data-stu-id="d4969-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="d4969-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d4969-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d4969-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d4969-119">Request headers</span></span>
| <span data-ttu-id="d4969-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d4969-120">Header</span></span>       | <span data-ttu-id="d4969-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d4969-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d4969-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d4969-122">Authorization</span></span>  | <span data-ttu-id="d4969-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d4969-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d4969-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d4969-125">Content-Type</span></span>  | <span data-ttu-id="d4969-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d4969-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d4969-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d4969-127">Request body</span></span>
<span data-ttu-id="d4969-128">No corpo da solicitação, fornece uma representação JSON do objeto de [equipe](../resources/team.md) .</span><span class="sxs-lookup"><span data-stu-id="d4969-128">In the request body, supply a JSON representation of [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d4969-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4969-129">Response</span></span>

<span data-ttu-id="d4969-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d4969-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d4969-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d4969-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="d4969-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d4969-132">Request</span></span>
<span data-ttu-id="d4969-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d4969-133">The following is an example of the request.</span></span>
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
#### <a name="response"></a><span data-ttu-id="d4969-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4969-134">Response</span></span>
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
