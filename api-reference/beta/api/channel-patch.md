---
title: Canal do patch
description: Atualize as propriedades do canal especificado.
author: nkramer
ms.openlocfilehash: 267cc6bc148259bc573625fdb2775ac8b581a988
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328347"
---
# <a name="patch-channel"></a><span data-ttu-id="473f9-103">Canal do patch</span><span class="sxs-lookup"><span data-stu-id="473f9-103">Patch channel</span></span>

> <span data-ttu-id="473f9-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="473f9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="473f9-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="473f9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="473f9-106">Atualize as propriedades do [canal](../resources/channel.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="473f9-106">Update the properties of the specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="473f9-107">**Observação**: não há um problema conhecido com permissões de aplicativo e essa API.</span><span class="sxs-lookup"><span data-stu-id="473f9-107">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="473f9-108">Para obter detalhes, consulte a [lista de problemas conhecidos do](/graph/known-issues#application-permissions).</span><span class="sxs-lookup"><span data-stu-id="473f9-108">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="473f9-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="473f9-109">Permissions</span></span>
<span data-ttu-id="473f9-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="473f9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="473f9-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="473f9-112">Permission type</span></span>      | <span data-ttu-id="473f9-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="473f9-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="473f9-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="473f9-114">Delegated (work or school account)</span></span> | <span data-ttu-id="473f9-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="473f9-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="473f9-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="473f9-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="473f9-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="473f9-117">Not supported.</span></span>    |
|<span data-ttu-id="473f9-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="473f9-118">Application</span></span> | <span data-ttu-id="473f9-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="473f9-119">Group.ReadWrite.All</span></span> |

> <span data-ttu-id="473f9-120">**Observação**: Esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="473f9-120">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="473f9-121">Administradores globais e administradores de serviço de Teams da Microsoft podem acessar as equipes que eles não serão um membro do.</span><span class="sxs-lookup"><span data-stu-id="473f9-121">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="473f9-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="473f9-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="473f9-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="473f9-123">Request headers</span></span>
| <span data-ttu-id="473f9-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="473f9-124">Header</span></span>       | <span data-ttu-id="473f9-125">Valor</span><span class="sxs-lookup"><span data-stu-id="473f9-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="473f9-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="473f9-126">Authorization</span></span>  | <span data-ttu-id="473f9-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="473f9-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="473f9-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="473f9-129">Content-Type</span></span>  | <span data-ttu-id="473f9-130">application/json</span><span class="sxs-lookup"><span data-stu-id="473f9-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="473f9-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="473f9-131">Request body</span></span>
<span data-ttu-id="473f9-132">No corpo da solicitação, fornece uma representação JSON do objeto de [canal](../resources/channel.md) .</span><span class="sxs-lookup"><span data-stu-id="473f9-132">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="473f9-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="473f9-133">Response</span></span>

<span data-ttu-id="473f9-134">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="473f9-134">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="473f9-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="473f9-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="473f9-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="473f9-136">Request</span></span>
<span data-ttu-id="473f9-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="473f9-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "patch_channel"
}-->
```http
PATCH https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
##### <a name="response"></a><span data-ttu-id="473f9-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="473f9-138">Response</span></span>
<span data-ttu-id="473f9-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="473f9-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
