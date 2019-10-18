---
title: Criar canal
description: Crie um novo canal no Microsoft Team, como especificado no corpo da solicitação.
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 08fca46352bf7cbb96f6567a0c0812bf41dfec8b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369007"
---
# <a name="create-channel"></a><span data-ttu-id="2d42e-103">Criar canal</span><span class="sxs-lookup"><span data-stu-id="2d42e-103">Create Channel</span></span>



<span data-ttu-id="2d42e-104">Criar um novo [canal](../resources/channel.md) no Microsoft Team, como especificado no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2d42e-104">Create a new [channel](../resources/channel.md) in a Microsoft Team, as specified in the request body.</span></span>

> <span data-ttu-id="2d42e-105">**Observação**: Há um problema conhecido com as permissões do aplicativo e este API.</span><span class="sxs-lookup"><span data-stu-id="2d42e-105">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="2d42e-106">Para saber mais, confira a [lista de problemas conhecidos](/graph/known-issues#application-permissions).</span><span class="sxs-lookup"><span data-stu-id="2d42e-106">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="2d42e-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="2d42e-107">Permissions</span></span>
<span data-ttu-id="2d42e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d42e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2d42e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2d42e-110">Permission type</span></span>      | <span data-ttu-id="2d42e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2d42e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2d42e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2d42e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2d42e-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d42e-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2d42e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2d42e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d42e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2d42e-115">Not supported.</span></span>    |
|<span data-ttu-id="2d42e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2d42e-116">Application</span></span> | <span data-ttu-id="2d42e-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d42e-117">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="2d42e-118">**Observação**: esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="2d42e-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="2d42e-119">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="2d42e-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="2d42e-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2d42e-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels
```
## <a name="request-headers"></a><span data-ttu-id="2d42e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2d42e-121">Request headers</span></span>
| <span data-ttu-id="2d42e-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2d42e-122">Header</span></span>       | <span data-ttu-id="2d42e-123">Valor</span><span class="sxs-lookup"><span data-stu-id="2d42e-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2d42e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="2d42e-124">Authorization</span></span>  | <span data-ttu-id="2d42e-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2d42e-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2d42e-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2d42e-127">Content-Type</span></span>  | <span data-ttu-id="2d42e-128">application/json</span><span class="sxs-lookup"><span data-stu-id="2d42e-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2d42e-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2d42e-129">Request body</span></span>
<span data-ttu-id="2d42e-130">No corpo da solicitação, fornça uma representação JSON do objeto [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="2d42e-130">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2d42e-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d42e-131">Response</span></span>

<span data-ttu-id="2d42e-132">Se bem-sucedido, esse método retornará `201 Created` código de resposta e um objeto [canal](../resources/channel.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2d42e-132">If successful, this method returns `201 Created` response code and [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d42e-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2d42e-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2d42e-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2d42e-134">Request</span></span>
<span data-ttu-id="2d42e-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2d42e-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2d42e-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="2d42e-136">--Http</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="2d42e-137">C#</span><span class="sxs-lookup"><span data-stu-id="2d42e-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-channel-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2d42e-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2d42e-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-channel-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2d42e-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2d42e-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-channel-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="2d42e-140">Java</span><span class="sxs-lookup"><span data-stu-id="2d42e-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-channel-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2d42e-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d42e-141">Response</span></span>
<span data-ttu-id="2d42e-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2d42e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
