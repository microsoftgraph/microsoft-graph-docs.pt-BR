---
title: Criar canal
description: Crie um novo canal no Microsoft Team, como especificado no corpo da solicitação.
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: bdf98d5bdfe49ca45e715d4eb6d63f0a514548b6
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35273665"
---
# <a name="create-channel"></a><span data-ttu-id="da935-103">Criar canal</span><span class="sxs-lookup"><span data-stu-id="da935-103">Create Channel</span></span>



<span data-ttu-id="da935-104">Criar um novo [canal](../resources/channel.md) no Microsoft Team, como especificado no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="da935-104">Create a new [channel](../resources/channel.md) in a Microsoft Team, as specified in the request body.</span></span>

> <span data-ttu-id="da935-105">**Observação**: Há um problema conhecido com as permissões do aplicativo e este API.</span><span class="sxs-lookup"><span data-stu-id="da935-105">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="da935-106">Para saber mais, confira a [lista de problemas conhecidos](/graph/known-issues#application-permissions).</span><span class="sxs-lookup"><span data-stu-id="da935-106">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="da935-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="da935-107">Permissions</span></span>
<span data-ttu-id="da935-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da935-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="da935-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="da935-110">Permission type</span></span>      | <span data-ttu-id="da935-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="da935-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da935-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="da935-112">Delegated (work or school account)</span></span> | <span data-ttu-id="da935-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da935-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="da935-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="da935-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da935-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da935-115">Not supported.</span></span>    |
|<span data-ttu-id="da935-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="da935-116">Application</span></span> | <span data-ttu-id="da935-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da935-117">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="da935-118">**Observação**: esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="da935-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="da935-119">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="da935-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="da935-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="da935-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels
```
## <a name="request-headers"></a><span data-ttu-id="da935-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="da935-121">Request headers</span></span>
| <span data-ttu-id="da935-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="da935-122">Header</span></span>       | <span data-ttu-id="da935-123">Valor</span><span class="sxs-lookup"><span data-stu-id="da935-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="da935-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="da935-124">Authorization</span></span>  | <span data-ttu-id="da935-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="da935-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="da935-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="da935-127">Content-Type</span></span>  | <span data-ttu-id="da935-128">application/json</span><span class="sxs-lookup"><span data-stu-id="da935-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="da935-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="da935-129">Request body</span></span>
<span data-ttu-id="da935-130">No corpo da solicitação, fornça uma representação JSON do objeto [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="da935-130">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="da935-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="da935-131">Response</span></span>

<span data-ttu-id="da935-132">Se bem-sucedido, esse método retornará `201 Created` código de resposta e um objeto [canal](../resources/channel.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="da935-132">If successful, this method returns `201 Created` response code and [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da935-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="da935-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="da935-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="da935-134">Request</span></span>
<span data-ttu-id="da935-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="da935-135">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="da935-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="da935-136">Response</span></span>
<span data-ttu-id="da935-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="da935-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="da935-140">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="da935-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="da935-141">C#</span><span class="sxs-lookup"><span data-stu-id="da935-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_channel_from_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="da935-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="da935-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_channel_from_group-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="da935-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="da935-143">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_channel_from_group-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/channel-post.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/channel-post.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/channel-post.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
