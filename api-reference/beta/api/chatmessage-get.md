---
title: Obter chat
description: Recupere as propriedades e os relacionamentos de um objeto chat.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6ef40a53be083744f99cac01cf2e72466e616b20
ms.sourcegitcommit: 624ac42e74533a9bf0d0d22b3b15adbb258fd594
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/05/2019
ms.locfileid: "34720861"
---
# <a name="get-chatmessage"></a><span data-ttu-id="19a78-103">Obter chat</span><span class="sxs-lookup"><span data-stu-id="19a78-103">Get chatMessage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19a78-104">Recupere as propriedades e os relacionamentos de um objeto [chat](../resources/chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="19a78-104">Retrieve the properties and relationships of a [chatMessage](../resources/chatmessage.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="19a78-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="19a78-105">Permissions</span></span>

<span data-ttu-id="19a78-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19a78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="19a78-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="19a78-108">Permission type</span></span>                        | <span data-ttu-id="19a78-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="19a78-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="19a78-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="19a78-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="19a78-111">Chat. Read, chat. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19a78-111">Chat.Read, Chat.ReadWrite</span></span> |
| <span data-ttu-id="19a78-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="19a78-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19a78-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="19a78-113">Not supported.</span></span> |
| <span data-ttu-id="19a78-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="19a78-114">Application</span></span>                            | <span data-ttu-id="19a78-115">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="19a78-115">Chat.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="19a78-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="19a78-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}
GET /users/{id}/chats/{id}/messages/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="19a78-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="19a78-117">Optional query parameters</span></span>

<span data-ttu-id="19a78-118">Esta operação não oferece suporte aos [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="19a78-118">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="19a78-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="19a78-119">Request headers</span></span>

| <span data-ttu-id="19a78-120">Nome</span><span class="sxs-lookup"><span data-stu-id="19a78-120">Name</span></span>      |<span data-ttu-id="19a78-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="19a78-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="19a78-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="19a78-122">Authorization</span></span> | <span data-ttu-id="19a78-123">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="19a78-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="19a78-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="19a78-124">Request body</span></span>

<span data-ttu-id="19a78-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="19a78-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="19a78-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="19a78-126">Response</span></span>

<span data-ttu-id="19a78-127">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [chat](../resources/chatmessage.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="19a78-127">If successful, this method returns a `200 OK` response code and the requested [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="19a78-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="19a78-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="19a78-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="19a78-129">Request</span></span>

<span data-ttu-id="19a78-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="19a78-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_chatmessage"
}-->

```http
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}
```

### <a name="response"></a><span data-ttu-id="19a78-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="19a78-131">Response</span></span>

<span data-ttu-id="19a78-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="19a78-132">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="19a78-133">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="19a78-133">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="19a78-134">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="19a78-134">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "replyToId": "replyToId-value",
  "from": {
    "application": {
      "id": "id-value",
      "displayName": "displayName-value"
    },
    "device": {
      "id": "id-value",
      "displayName": "displayName-value"
    },
    "user": {
      "id": "id-value",
      "displayName": "displayName-value"
    }
  },
  "etag": "etag-value",
  "messageType": "messageType-value",
  "createdDateTime": "datetime-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get chatMessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->