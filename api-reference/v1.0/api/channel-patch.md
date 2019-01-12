---
title: Canal do patch
description: Atualize as propriedades do canal especificado.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4c3a03aaab52da62f56ca376035e56a9b8584832
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984336"
---
# <a name="patch-channel"></a><span data-ttu-id="1f871-103">Canal do patch</span><span class="sxs-lookup"><span data-stu-id="1f871-103">Patch channel</span></span>



<span data-ttu-id="1f871-104">Atualize as propriedades do [canal](../resources/channel.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="1f871-104">Update the properties of the specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="1f871-105">**Observação**: não há um problema conhecido com permissões de aplicativo e essa API.</span><span class="sxs-lookup"><span data-stu-id="1f871-105">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="1f871-106">Para obter detalhes, consulte a [lista de problemas conhecidos do](/graph/known-issues#application-permissions).</span><span class="sxs-lookup"><span data-stu-id="1f871-106">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="1f871-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="1f871-107">Permissions</span></span>
<span data-ttu-id="1f871-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f871-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f871-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1f871-110">Permission type</span></span>      | <span data-ttu-id="1f871-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1f871-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1f871-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1f871-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1f871-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f871-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1f871-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1f871-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f871-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1f871-115">Not supported.</span></span>    |
|<span data-ttu-id="1f871-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1f871-116">Application</span></span> | <span data-ttu-id="1f871-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f871-117">Group.ReadWrite.All</span></span> |

> <span data-ttu-id="1f871-118">**Observação**: Esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="1f871-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="1f871-119">Administradores globais e administradores de serviço de Teams da Microsoft podem acessar as equipes que eles não serão um membro do.</span><span class="sxs-lookup"><span data-stu-id="1f871-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="1f871-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1f871-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="1f871-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1f871-121">Request headers</span></span>
| <span data-ttu-id="1f871-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1f871-122">Header</span></span>       | <span data-ttu-id="1f871-123">Valor</span><span class="sxs-lookup"><span data-stu-id="1f871-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1f871-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="1f871-124">Authorization</span></span>  | <span data-ttu-id="1f871-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1f871-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1f871-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1f871-127">Content-Type</span></span>  | <span data-ttu-id="1f871-128">application/json</span><span class="sxs-lookup"><span data-stu-id="1f871-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1f871-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1f871-129">Request body</span></span>
<span data-ttu-id="1f871-130">No corpo da solicitação, fornece uma representação JSON do objeto de [canal](../resources/channel.md) .</span><span class="sxs-lookup"><span data-stu-id="1f871-130">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="1f871-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f871-131">Response</span></span>

<span data-ttu-id="1f871-132">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1f871-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1f871-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1f871-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1f871-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1f871-134">Request</span></span>
<span data-ttu-id="1f871-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1f871-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "patch_channel"
}-->
```http
PATCH https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
##### <a name="response"></a><span data-ttu-id="1f871-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f871-136">Response</span></span>
<span data-ttu-id="1f871-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1f871-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Patch channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
