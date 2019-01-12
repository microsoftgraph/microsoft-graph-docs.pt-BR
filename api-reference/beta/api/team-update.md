---
title: Equipe de atualização
description: Atualize as propriedades da equipe especificado.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: bb882a31916d31744d57cdc0ef3d2a161361b628
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925984"
---
# <a name="update-team"></a><span data-ttu-id="4edcf-103">Equipe de atualização</span><span class="sxs-lookup"><span data-stu-id="4edcf-103">Update team</span></span>

> <span data-ttu-id="4edcf-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4edcf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4edcf-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4edcf-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4edcf-106">Atualize as propriedades da [equipe](../resources/team.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="4edcf-106">Update the properties of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4edcf-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="4edcf-107">Permissions</span></span>
<span data-ttu-id="4edcf-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4edcf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4edcf-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4edcf-110">Permission type</span></span>      | <span data-ttu-id="4edcf-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4edcf-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4edcf-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4edcf-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4edcf-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4edcf-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4edcf-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4edcf-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4edcf-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4edcf-115">Not supported.</span></span>    |
|<span data-ttu-id="4edcf-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4edcf-116">Application</span></span> | <span data-ttu-id="4edcf-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4edcf-117">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="4edcf-118">**Observação**: Esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="4edcf-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="4edcf-119">Administradores globais e administradores de serviço de Teams da Microsoft podem acessar as equipes que eles não serão um membro do.</span><span class="sxs-lookup"><span data-stu-id="4edcf-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="4edcf-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4edcf-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}
```
## <a name="request-headers"></a><span data-ttu-id="4edcf-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4edcf-121">Request headers</span></span>
| <span data-ttu-id="4edcf-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4edcf-122">Header</span></span>       | <span data-ttu-id="4edcf-123">Valor</span><span class="sxs-lookup"><span data-stu-id="4edcf-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4edcf-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="4edcf-124">Authorization</span></span>  | <span data-ttu-id="4edcf-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4edcf-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4edcf-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4edcf-127">Content-Type</span></span>  | <span data-ttu-id="4edcf-128">application/json</span><span class="sxs-lookup"><span data-stu-id="4edcf-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4edcf-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4edcf-129">Request body</span></span>
<span data-ttu-id="4edcf-130">No corpo da solicitação, fornece uma representação JSON do objeto de [equipe](../resources/team.md) .</span><span class="sxs-lookup"><span data-stu-id="4edcf-130">In the request body, supply a JSON representation of [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="4edcf-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="4edcf-131">Response</span></span>

<span data-ttu-id="4edcf-132">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4edcf-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4edcf-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4edcf-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="4edcf-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4edcf-134">Request</span></span>
<span data-ttu-id="4edcf-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4edcf-135">The following is an example of the request.</span></span>
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
#### <a name="response"></a><span data-ttu-id="4edcf-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="4edcf-136">Response</span></span>
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
