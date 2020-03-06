---
title: Canal de patch
description: Atualiza as propriedades do canal especificado.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 68265b319fd567097b72c9eaad82275fd3faefab
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518599"
---
# <a name="patch-channel"></a><span data-ttu-id="9411e-103">Canal de patch</span><span class="sxs-lookup"><span data-stu-id="9411e-103">Patch channel</span></span>

<span data-ttu-id="9411e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9411e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9411e-105">Atualiza as propriedades do [canal](../resources/channel.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="9411e-105">Update the properties of the specified [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9411e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9411e-106">Permissions</span></span>

<span data-ttu-id="9411e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9411e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9411e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9411e-109">Permission type</span></span>      | <span data-ttu-id="9411e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9411e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9411e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9411e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9411e-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9411e-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9411e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9411e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9411e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9411e-114">Not supported.</span></span>    |
|<span data-ttu-id="9411e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9411e-115">Application</span></span> | <span data-ttu-id="9411e-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9411e-116">Group.ReadWrite.All</span></span> |

> <span data-ttu-id="9411e-117">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="9411e-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="9411e-118">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="9411e-118">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="9411e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9411e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}/channels/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9411e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9411e-120">Request headers</span></span>

| <span data-ttu-id="9411e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9411e-121">Header</span></span>       | <span data-ttu-id="9411e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9411e-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9411e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9411e-123">Authorization</span></span>  | <span data-ttu-id="9411e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9411e-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9411e-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9411e-126">Content-Type</span></span>  | <span data-ttu-id="9411e-127">application/json</span><span class="sxs-lookup"><span data-stu-id="9411e-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9411e-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9411e-128">Request body</span></span>

<span data-ttu-id="9411e-129">No corpo da solicitação, fornça uma representação JSON do objeto [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="9411e-129">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9411e-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="9411e-130">Response</span></span>

<span data-ttu-id="9411e-131">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9411e-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9411e-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9411e-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="9411e-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9411e-133">Request</span></span>

<span data-ttu-id="9411e-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9411e-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9411e-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="9411e-135">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "patch_channel"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}
```
# <a name="objective-c"></a>[<span data-ttu-id="9411e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9411e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="9411e-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="9411e-137">Response</span></span>

<span data-ttu-id="9411e-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9411e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
