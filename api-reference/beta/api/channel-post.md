---
title: Criar canal
description: Criar um novo canal em uma equipe da Microsoft, conforme especificado no corpo da solicitação.
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: c1163b82bc5d2b6170079ab80ff77a1cc341c627
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32456560"
---
# <a name="create-channel"></a><span data-ttu-id="555b1-103">Criar canal</span><span class="sxs-lookup"><span data-stu-id="555b1-103">Create Channel</span></span>



<span data-ttu-id="555b1-104">Criar um novo [canal](../resources/channel.md) em uma equipe da Microsoft, conforme especificado no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="555b1-104">Create a new [channel](../resources/channel.md) in a Microsoft Team, as specified in the request body.</span></span>

> <span data-ttu-id="555b1-105">**Observação**: há um problema conhecido com permissões de aplicativo e essa API.</span><span class="sxs-lookup"><span data-stu-id="555b1-105">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="555b1-106">Para obter detalhes, consulte a [lista de problemas conhecidos](/graph/known-issues#application-permissions).</span><span class="sxs-lookup"><span data-stu-id="555b1-106">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="555b1-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="555b1-107">Permissions</span></span>
<span data-ttu-id="555b1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="555b1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="555b1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="555b1-110">Permission type</span></span>      | <span data-ttu-id="555b1-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="555b1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="555b1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="555b1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="555b1-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="555b1-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="555b1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="555b1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="555b1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="555b1-115">Not supported.</span></span>    |
|<span data-ttu-id="555b1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="555b1-116">Application</span></span> | <span data-ttu-id="555b1-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="555b1-117">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="555b1-118">**Observação**: esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="555b1-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="555b1-119">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="555b1-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="555b1-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="555b1-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels
```
## <a name="request-headers"></a><span data-ttu-id="555b1-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="555b1-121">Request headers</span></span>
| <span data-ttu-id="555b1-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="555b1-122">Header</span></span>       | <span data-ttu-id="555b1-123">Valor</span><span class="sxs-lookup"><span data-stu-id="555b1-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="555b1-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="555b1-124">Authorization</span></span>  | <span data-ttu-id="555b1-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="555b1-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="555b1-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="555b1-127">Content-Type</span></span>  | <span data-ttu-id="555b1-128">application/json</span><span class="sxs-lookup"><span data-stu-id="555b1-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="555b1-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="555b1-129">Request body</span></span>
<span data-ttu-id="555b1-130">No corpo da solicitação, forneça uma representação JSON do objeto [Channel](../resources/channel.md) .</span><span class="sxs-lookup"><span data-stu-id="555b1-130">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="555b1-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="555b1-131">Response</span></span>

<span data-ttu-id="555b1-132">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [Channel](../resources/channel.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="555b1-132">If successful, this method returns `201 Created` response code and [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="555b1-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="555b1-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="555b1-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="555b1-134">Request</span></span>
<span data-ttu-id="555b1-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="555b1-135">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="555b1-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="555b1-136">Response</span></span>
<span data-ttu-id="555b1-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="555b1-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
