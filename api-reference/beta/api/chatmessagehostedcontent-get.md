---
title: Obter chatMessageHostedContent
description: Recupere as propriedades e os relacionamentos do objeto chatMessageHostedContent.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6ff4776b35544b62c7388bc760a54893c35dba36
ms.sourcegitcommit: 624ac42e74533a9bf0d0d22b3b15adbb258fd594
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/05/2019
ms.locfileid: "34720853"
---
# <a name="get-chatmessagehostedcontent"></a><span data-ttu-id="1783a-103">Obter chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="1783a-103">Get chatMessageHostedContent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1783a-104">Recupere as propriedades e os relacionamentos do objeto [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) .</span><span class="sxs-lookup"><span data-stu-id="1783a-104">Retrieve the properties and relationships of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1783a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="1783a-105">Permissions</span></span>

<span data-ttu-id="1783a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1783a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1783a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1783a-108">Permission type</span></span>                        | <span data-ttu-id="1783a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1783a-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1783a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1783a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="1783a-111">Chat. Read, chat. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1783a-111">Chat.Read, Chat.ReadWrite</span></span> |
| <span data-ttu-id="1783a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1783a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1783a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1783a-113">Not supported.</span></span> |
| <span data-ttu-id="1783a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1783a-114">Application</span></span>                            | <span data-ttu-id="1783a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1783a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1783a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1783a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}/hostedContents/{id}
GET /users/{id}/chats/{id}/messages/{id}/hostedContents/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1783a-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1783a-117">Optional query parameters</span></span>

<span data-ttu-id="1783a-118">Esta operação não oferece suporte aos [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1783a-118">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1783a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1783a-119">Request headers</span></span>

| <span data-ttu-id="1783a-120">Nome</span><span class="sxs-lookup"><span data-stu-id="1783a-120">Name</span></span>      |<span data-ttu-id="1783a-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="1783a-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1783a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1783a-122">Authorization</span></span> | <span data-ttu-id="1783a-123">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="1783a-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="1783a-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1783a-124">Request body</span></span>

<span data-ttu-id="1783a-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1783a-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1783a-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="1783a-126">Response</span></span>

<span data-ttu-id="1783a-127">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1783a-127">If successful, this method returns a `200 OK` response code and the requested [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1783a-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1783a-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1783a-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1783a-129">Request</span></span>

<span data-ttu-id="1783a-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1783a-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_chatmessagehostedcontent"
}-->

```http
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents/{id}
```

### <a name="response"></a><span data-ttu-id="1783a-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="1783a-131">Response</span></span>

<span data-ttu-id="1783a-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1783a-132">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="1783a-133">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1783a-133">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1783a-134">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1783a-134">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessageHostedContent"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get chatMessageHostedContent",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->