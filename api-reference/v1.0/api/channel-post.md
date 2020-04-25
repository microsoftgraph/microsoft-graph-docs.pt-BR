---
title: Criar canal
description: Crie um novo canal no Microsoft Team, como especificado no corpo da solicitação.
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c83511faf6034caab1c55ec394c3e53394011097
ms.sourcegitcommit: 195fa0d441a49662e144323d37518dbba0c76fc7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2020
ms.locfileid: "43806121"
---
# <a name="create-channel"></a><span data-ttu-id="cf45f-103">Criar canal</span><span class="sxs-lookup"><span data-stu-id="cf45f-103">Create Channel</span></span>

<span data-ttu-id="cf45f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf45f-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="cf45f-105">Criar um novo [canal](../resources/channel.md) no Microsoft Team, como especificado no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cf45f-105">Create a new [channel](../resources/channel.md) in a Microsoft Team, as specified in the request body.</span></span>

> <span data-ttu-id="cf45f-106">**Observação**: Há um problema conhecido com as permissões do aplicativo e este API.</span><span class="sxs-lookup"><span data-stu-id="cf45f-106">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="cf45f-107">Para saber mais, confira a [lista de problemas conhecidos](/graph/known-issues#application-permissions).</span><span class="sxs-lookup"><span data-stu-id="cf45f-107">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="cf45f-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="cf45f-108">Permissions</span></span>
<span data-ttu-id="cf45f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf45f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="cf45f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cf45f-111">Permission type</span></span>      | <span data-ttu-id="cf45f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cf45f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cf45f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cf45f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="cf45f-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf45f-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="cf45f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cf45f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf45f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf45f-116">Not supported.</span></span>    |
|<span data-ttu-id="cf45f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cf45f-117">Application</span></span> | <span data-ttu-id="cf45f-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf45f-118">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="cf45f-119">**Observação**: esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="cf45f-119">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="cf45f-120">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="cf45f-120">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="cf45f-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cf45f-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels
```
## <a name="request-headers"></a><span data-ttu-id="cf45f-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cf45f-122">Request headers</span></span>
| <span data-ttu-id="cf45f-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cf45f-123">Header</span></span>       | <span data-ttu-id="cf45f-124">Valor</span><span class="sxs-lookup"><span data-stu-id="cf45f-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cf45f-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="cf45f-125">Authorization</span></span>  | <span data-ttu-id="cf45f-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cf45f-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cf45f-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cf45f-128">Content-Type</span></span>  | <span data-ttu-id="cf45f-129">application/json</span><span class="sxs-lookup"><span data-stu-id="cf45f-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cf45f-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cf45f-130">Request body</span></span>
<span data-ttu-id="cf45f-131">No corpo da solicitação, fornça uma representação JSON do objeto [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="cf45f-131">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="cf45f-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf45f-132">Response</span></span>

<span data-ttu-id="cf45f-133">Se bem-sucedido, esse método retornará `201 Created` código de resposta e um objeto [canal](../resources/channel.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cf45f-133">If successful, this method returns `201 Created` response code and [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf45f-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cf45f-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cf45f-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cf45f-135">Request</span></span>
<span data-ttu-id="cf45f-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cf45f-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cf45f-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="cf45f-137">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="cf45f-138">C#</span><span class="sxs-lookup"><span data-stu-id="cf45f-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-channel-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cf45f-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cf45f-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-channel-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cf45f-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cf45f-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-channel-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cf45f-141">Java</span><span class="sxs-lookup"><span data-stu-id="cf45f-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-channel-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="cf45f-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf45f-142">Response</span></span>
<span data-ttu-id="cf45f-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cf45f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->
```http
HTTP/1.1 201 Created
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
