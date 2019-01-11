---
title: Criar canal
description: Crie um novo canal em um Microsoft Team, conforme especificado no corpo da solicitação.
localization_priority: Normal
ms.openlocfilehash: f7192c177d79e48a0a9e55c9edc5dbb394539928
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875044"
---
# <a name="create-channel"></a><span data-ttu-id="d52a3-103">Criar canal</span><span class="sxs-lookup"><span data-stu-id="d52a3-103">Create Channel</span></span>

> <span data-ttu-id="d52a3-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d52a3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d52a3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d52a3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d52a3-106">Crie um novo [canal](../resources/channel.md) em um Microsoft Team, conforme especificado no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d52a3-106">Create a new [channel](../resources/channel.md) in a Microsoft Team, as specified in the request body.</span></span>

> <span data-ttu-id="d52a3-107">**Observação**: não há um problema conhecido com permissões de aplicativo e essa API.</span><span class="sxs-lookup"><span data-stu-id="d52a3-107">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="d52a3-108">Para obter detalhes, consulte a [lista de problemas conhecidos do](/graph/known-issues#application-permissions).</span><span class="sxs-lookup"><span data-stu-id="d52a3-108">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="d52a3-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="d52a3-109">Permissions</span></span>
<span data-ttu-id="d52a3-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d52a3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d52a3-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d52a3-112">Permission type</span></span>      | <span data-ttu-id="d52a3-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d52a3-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d52a3-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d52a3-114">Delegated (work or school account)</span></span> | <span data-ttu-id="d52a3-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d52a3-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d52a3-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d52a3-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d52a3-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d52a3-117">Not supported.</span></span>    |
|<span data-ttu-id="d52a3-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d52a3-118">Application</span></span> | <span data-ttu-id="d52a3-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d52a3-119">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="d52a3-120">**Observação**: Esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="d52a3-120">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="d52a3-121">Administradores globais e administradores de serviço de Teams da Microsoft podem acessar as equipes que eles não serão um membro do.</span><span class="sxs-lookup"><span data-stu-id="d52a3-121">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="d52a3-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d52a3-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels
```
## <a name="request-headers"></a><span data-ttu-id="d52a3-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d52a3-123">Request headers</span></span>
| <span data-ttu-id="d52a3-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d52a3-124">Header</span></span>       | <span data-ttu-id="d52a3-125">Valor</span><span class="sxs-lookup"><span data-stu-id="d52a3-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d52a3-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="d52a3-126">Authorization</span></span>  | <span data-ttu-id="d52a3-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d52a3-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d52a3-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d52a3-129">Content-Type</span></span>  | <span data-ttu-id="d52a3-130">application/json</span><span class="sxs-lookup"><span data-stu-id="d52a3-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d52a3-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d52a3-131">Request body</span></span>
<span data-ttu-id="d52a3-132">No corpo da solicitação, fornece uma representação JSON do objeto de [canal](../resources/channel.md) .</span><span class="sxs-lookup"><span data-stu-id="d52a3-132">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d52a3-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="d52a3-133">Response</span></span>

<span data-ttu-id="d52a3-134">Se tiver êxito, este método retornará `201 Created` objeto de código e o [canal](../resources/channel.md) de resposta no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d52a3-134">If successful, this method returns `201 Created` response code and [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d52a3-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d52a3-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d52a3-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d52a3-136">Request</span></span>
<span data-ttu-id="d52a3-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d52a3-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_channel_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels
Content-type: application/json

{
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans"
}
```
##### <a name="response"></a><span data-ttu-id="d52a3-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="d52a3-138">Response</span></span>
<span data-ttu-id="d52a3-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d52a3-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
