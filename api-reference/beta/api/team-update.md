---
title: Equipe de atualização
description: Atualize as propriedades da equipe especificado.
ms.openlocfilehash: 9d07fd687facc96c1bc4a93c37cb492b321518e6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034408"
---
# <a name="update-team"></a><span data-ttu-id="791ce-103">Equipe de atualização</span><span class="sxs-lookup"><span data-stu-id="791ce-103">Update team</span></span>

> <span data-ttu-id="791ce-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="791ce-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="791ce-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="791ce-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="791ce-106">Atualize as propriedades da [equipe](../resources/team.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="791ce-106">Update the properties of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="791ce-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="791ce-107">Permissions</span></span>
<span data-ttu-id="791ce-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="791ce-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="791ce-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="791ce-110">Permission type</span></span>      | <span data-ttu-id="791ce-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="791ce-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="791ce-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="791ce-112">Delegated (work or school account)</span></span> | <span data-ttu-id="791ce-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="791ce-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="791ce-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="791ce-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="791ce-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="791ce-115">Not supported.</span></span>    |
|<span data-ttu-id="791ce-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="791ce-116">Application</span></span> | <span data-ttu-id="791ce-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="791ce-117">Group.Read.All, Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="791ce-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="791ce-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}
```
## <a name="request-headers"></a><span data-ttu-id="791ce-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="791ce-119">Request headers</span></span>
| <span data-ttu-id="791ce-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="791ce-120">Header</span></span>       | <span data-ttu-id="791ce-121">Valor</span><span class="sxs-lookup"><span data-stu-id="791ce-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="791ce-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="791ce-122">Authorization</span></span>  | <span data-ttu-id="791ce-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="791ce-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="791ce-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="791ce-125">Content-Type</span></span>  | <span data-ttu-id="791ce-126">application/json</span><span class="sxs-lookup"><span data-stu-id="791ce-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="791ce-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="791ce-127">Request body</span></span>
<span data-ttu-id="791ce-128">No corpo da solicitação, fornece uma representação JSON do objeto de [equipe](../resources/team.md) .</span><span class="sxs-lookup"><span data-stu-id="791ce-128">In the request body, supply a JSON representation of [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="791ce-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="791ce-129">Response</span></span>

<span data-ttu-id="791ce-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="791ce-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="791ce-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="791ce-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="791ce-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="791ce-132">Request</span></span>
<span data-ttu-id="791ce-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="791ce-133">The following is an example of the request.</span></span>
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
#### <a name="response"></a><span data-ttu-id="791ce-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="791ce-134">Response</span></span>
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
