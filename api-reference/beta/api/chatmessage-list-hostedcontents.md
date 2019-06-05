---
title: Listar hostedContents
description: Recupere uma lista de objetos chatMessageHostedContent.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 48a79739124f54267147599c69ec60f567d3ab85
ms.sourcegitcommit: 624ac42e74533a9bf0d0d22b3b15adbb258fd594
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/05/2019
ms.locfileid: "34720857"
---
# <a name="list-hostedcontents"></a><span data-ttu-id="bc14c-103">Listar hostedContents</span><span class="sxs-lookup"><span data-stu-id="bc14c-103">List hostedContents</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc14c-104">Recupere uma lista de objetos [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) .</span><span class="sxs-lookup"><span data-stu-id="bc14c-104">Retrieve a list of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="bc14c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="bc14c-105">Permissions</span></span>

<span data-ttu-id="bc14c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc14c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bc14c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bc14c-108">Permission type</span></span>                        | <span data-ttu-id="bc14c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bc14c-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bc14c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bc14c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="bc14c-111">Chat. Read, chat. ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="bc14c-111">Chat.Read, Chat.ReadWrite.</span></span> |
| <span data-ttu-id="bc14c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bc14c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc14c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc14c-113">Not supported.</span></span> |
| <span data-ttu-id="bc14c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bc14c-114">Application</span></span>                            | <span data-ttu-id="bc14c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc14c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc14c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bc14c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}/hostedContents
GET /users/{id}/chats/{id}/messages/{id}/hostedContents
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bc14c-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bc14c-117">Optional query parameters</span></span>

<span data-ttu-id="bc14c-118">Esta operação não oferece suporte aos [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="bc14c-118">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bc14c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bc14c-119">Request headers</span></span>

| <span data-ttu-id="bc14c-120">Nome</span><span class="sxs-lookup"><span data-stu-id="bc14c-120">Name</span></span>      |<span data-ttu-id="bc14c-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc14c-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bc14c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc14c-122">Authorization</span></span> | <span data-ttu-id="bc14c-123">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="bc14c-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="bc14c-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bc14c-124">Request body</span></span>

<span data-ttu-id="bc14c-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bc14c-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bc14c-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc14c-126">Response</span></span>

<span data-ttu-id="bc14c-127">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bc14c-127">If successful, this method returns a `200 OK` response code and a collection of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bc14c-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="bc14c-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bc14c-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bc14c-129">Request</span></span>

<span data-ttu-id="bc14c-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bc14c-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_hostedcontents"
}-->

```http
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents
```

### <a name="response"></a><span data-ttu-id="bc14c-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc14c-131">Response</span></span>

<span data-ttu-id="bc14c-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bc14c-132">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="bc14c-133">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="bc14c-133">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="bc14c-134">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bc14c-134">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessageHostedContent",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List hostedContents",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->