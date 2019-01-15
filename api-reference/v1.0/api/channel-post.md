---
title: Criar canal
description: Crie um novo canal em um Microsoft Team, conforme especificado no corpo da solicitação.
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 9021ed45cb187b8db64ec2a3270b6a7f840134ba
ms.sourcegitcommit: 2c60e38bb1b71ba958659f66ad4736495e520851
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28016685"
---
# <a name="create-channel"></a><span data-ttu-id="60696-103">Criar canal</span><span class="sxs-lookup"><span data-stu-id="60696-103">Create Channel</span></span>



<span data-ttu-id="60696-104">Crie um novo [canal](../resources/channel.md) em um Microsoft Team, conforme especificado no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="60696-104">Create a new [channel](../resources/channel.md) in a Microsoft Team, as specified in the request body.</span></span>

> <span data-ttu-id="60696-105">**Observação**: não há um problema conhecido com permissões de aplicativo e essa API.</span><span class="sxs-lookup"><span data-stu-id="60696-105">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="60696-106">Para obter detalhes, consulte a [lista de problemas conhecidos do](/graph/known-issues#application-permissions).</span><span class="sxs-lookup"><span data-stu-id="60696-106">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="60696-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="60696-107">Permissions</span></span>
<span data-ttu-id="60696-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60696-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="60696-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="60696-110">Permission type</span></span>      | <span data-ttu-id="60696-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="60696-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="60696-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="60696-112">Delegated (work or school account)</span></span> | <span data-ttu-id="60696-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60696-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="60696-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="60696-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60696-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="60696-115">Not supported.</span></span>    |
|<span data-ttu-id="60696-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="60696-116">Application</span></span> | <span data-ttu-id="60696-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60696-117">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="60696-118">**Observação**: Esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="60696-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="60696-119">Administradores globais e administradores de serviço de Teams da Microsoft podem acessar as equipes que eles não serão um membro do.</span><span class="sxs-lookup"><span data-stu-id="60696-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="60696-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="60696-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels
```
## <a name="request-headers"></a><span data-ttu-id="60696-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="60696-121">Request headers</span></span>
| <span data-ttu-id="60696-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="60696-122">Header</span></span>       | <span data-ttu-id="60696-123">Valor</span><span class="sxs-lookup"><span data-stu-id="60696-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="60696-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="60696-124">Authorization</span></span>  | <span data-ttu-id="60696-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="60696-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="60696-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="60696-127">Content-Type</span></span>  | <span data-ttu-id="60696-128">application/json</span><span class="sxs-lookup"><span data-stu-id="60696-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="60696-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="60696-129">Request body</span></span>
<span data-ttu-id="60696-130">No corpo da solicitação, fornece uma representação JSON do objeto de [canal](../resources/channel.md) .</span><span class="sxs-lookup"><span data-stu-id="60696-130">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="60696-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="60696-131">Response</span></span>

<span data-ttu-id="60696-132">Se tiver êxito, este método retornará `201 Created` objeto de código e o [canal](../resources/channel.md) de resposta no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="60696-132">If successful, this method returns `201 Created` response code and [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60696-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="60696-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="60696-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="60696-134">Request</span></span>
<span data-ttu-id="60696-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="60696-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_channel_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{id}/channels
Content-type: application/json

{
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans"
}
```
##### <a name="response"></a><span data-ttu-id="60696-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="60696-136">Response</span></span>
<span data-ttu-id="60696-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="60696-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "id": "id-value",
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
