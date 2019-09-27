---
title: Canal de patch
description: Atualiza as propriedades do canal especificado.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b9b8abd495a9ce66458973360a93e47f0bddfdf9
ms.sourcegitcommit: d9e94c109c0934cc93f340aafa1dccaa1a5da9c7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37275672"
---
# <a name="patch-channel"></a><span data-ttu-id="a703c-103">Canal de patch</span><span class="sxs-lookup"><span data-stu-id="a703c-103">Patch channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a703c-104">Atualiza as propriedades do [canal](../resources/channel.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="a703c-104">Update the properties of the specified [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a703c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a703c-105">Permissions</span></span>

<span data-ttu-id="a703c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a703c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a703c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a703c-108">Permission type</span></span>      | <span data-ttu-id="a703c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a703c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a703c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a703c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a703c-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a703c-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a703c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a703c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a703c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a703c-113">Not supported.</span></span>    |
|<span data-ttu-id="a703c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a703c-114">Application</span></span> | <span data-ttu-id="a703c-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a703c-115">Group.ReadWrite.All</span></span> |

> <span data-ttu-id="a703c-116">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="a703c-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="a703c-117">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="a703c-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="a703c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a703c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="a703c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a703c-119">Request headers</span></span>
| <span data-ttu-id="a703c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a703c-120">Header</span></span>       | <span data-ttu-id="a703c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a703c-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a703c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a703c-122">Authorization</span></span>  | <span data-ttu-id="a703c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a703c-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a703c-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a703c-125">Content-Type</span></span>  | <span data-ttu-id="a703c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a703c-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a703c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a703c-127">Request body</span></span>

<span data-ttu-id="a703c-128">No corpo da solicitação, fornça uma representação JSON do objeto [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="a703c-128">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

> <span data-ttu-id="a703c-129">Observação: não é possível atualizar `membershipType` o valor de um canal existente.</span><span class="sxs-lookup"><span data-stu-id="a703c-129">Note: You cannot update the `membershipType` value for an existing channel.</span></span>

## <a name="response"></a><span data-ttu-id="a703c-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="a703c-130">Response</span></span>

<span data-ttu-id="a703c-131">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a703c-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a703c-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a703c-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="a703c-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a703c-133">Request</span></span>

<span data-ttu-id="a703c-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a703c-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a703c-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="a703c-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "patch_channel"
}-->
```http
PATCH https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a703c-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a703c-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="a703c-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="a703c-137">Response</span></span>

<span data-ttu-id="a703c-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a703c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
    "description": "description-value",
    "displayName": "display-name-value",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Patch channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
