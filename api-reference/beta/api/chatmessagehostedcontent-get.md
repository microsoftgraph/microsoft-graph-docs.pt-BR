---
title: Obter chatMessageHostedContent
description: Recupere as propriedades e os relacionamentos do objeto chatMessageHostedContent.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f3b20410ded987ba0c73de4767e36075d2593434
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37355852"
---
# <a name="get-chatmessagehostedcontent"></a><span data-ttu-id="5886e-103">Obter chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="5886e-103">Get chatMessageHostedContent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5886e-104">Recupere as propriedades e os relacionamentos do objeto [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) .</span><span class="sxs-lookup"><span data-stu-id="5886e-104">Retrieve the properties and relationships of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5886e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5886e-105">Permissions</span></span>

<span data-ttu-id="5886e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5886e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5886e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5886e-108">Permission type</span></span>                        | <span data-ttu-id="5886e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5886e-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="5886e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5886e-110">Delegated (work or school account)</span></span>|<span data-ttu-id="5886e-111">Para o **usuário** ou recurso de **chat** :</span><span class="sxs-lookup"><span data-stu-id="5886e-111">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="5886e-112">Chat. Read, chat. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5886e-112">Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="5886e-113">Para o recurso de **canal** :</span><span class="sxs-lookup"><span data-stu-id="5886e-113">For **channel** resource:</span></span><br/><span data-ttu-id="5886e-114">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5886e-114">Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="5886e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5886e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5886e-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5886e-116">Not supported</span></span>|
|<span data-ttu-id="5886e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5886e-117">Application</span></span>| <span data-ttu-id="5886e-118">Para o **usuário** ou recurso de **chat** :</span><span class="sxs-lookup"><span data-stu-id="5886e-118">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="5886e-119">Chat. Read. All, chat. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="5886e-119">Chat.Read.All, Chat.ReadWrite.All</span></span><br/><br/><span data-ttu-id="5886e-120">Para o recurso de **canal** :</span><span class="sxs-lookup"><span data-stu-id="5886e-120">For **channel** resource:</span></span><br/><span data-ttu-id="5886e-121">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5886e-121">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5886e-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5886e-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}/hostedContents/{id}
GET /users/{id}/chats/{id}/messages/{id}/hostedContents/{id}
GET /teams/{id}/channels/{id}/messages/{id}/hostedContents/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5886e-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5886e-123">Optional query parameters</span></span>

<span data-ttu-id="5886e-124">Esta operação não oferece suporte aos [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5886e-124">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5886e-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5886e-125">Request headers</span></span>

| <span data-ttu-id="5886e-126">Nome</span><span class="sxs-lookup"><span data-stu-id="5886e-126">Name</span></span>      |<span data-ttu-id="5886e-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="5886e-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5886e-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="5886e-128">Authorization</span></span> | <span data-ttu-id="5886e-129">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="5886e-129">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="5886e-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5886e-130">Request body</span></span>

<span data-ttu-id="5886e-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5886e-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5886e-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="5886e-132">Response</span></span>

<span data-ttu-id="5886e-133">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5886e-133">If successful, this method returns a `200 OK` response code and the requested [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5886e-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5886e-134">Examples</span></span>

### <a name="example-1-get-hosted-content"></a><span data-ttu-id="5886e-135">Exemplo 1: obter conteúdo hospedado</span><span class="sxs-lookup"><span data-stu-id="5886e-135">Example 1: Get hosted content</span></span>

#### <a name="request"></a><span data-ttu-id="5886e-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5886e-136">Request</span></span>

<span data-ttu-id="5886e-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5886e-137">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5886e-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="5886e-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chatmessagehostedcontent"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5886e-139">C#</span><span class="sxs-lookup"><span data-stu-id="5886e-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chatmessagehostedcontent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5886e-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5886e-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chatmessagehostedcontent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5886e-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5886e-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chatmessagehostedcontent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="5886e-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="5886e-142">Response</span></span>

<span data-ttu-id="5886e-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5886e-143">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="5886e-144">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5886e-144">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5886e-145">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5886e-145">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-hosted-content-bytes-for-an-image"></a><span data-ttu-id="5886e-146">Exemplo 2: obter bytes de conteúdo hospedados para uma imagem</span><span class="sxs-lookup"><span data-stu-id="5886e-146">Example 2: Get hosted content bytes for an image</span></span>

#### <a name="request"></a><span data-ttu-id="5886e-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5886e-147">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="5886e-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="5886e-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chatmessagehostedcontent"
}-->
```http
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents/{id}/$value
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5886e-149">C#</span><span class="sxs-lookup"><span data-stu-id="5886e-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chatmessagehostedcontent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5886e-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5886e-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chatmessagehostedcontent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5886e-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5886e-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chatmessagehostedcontent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5886e-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="5886e-152">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessageHostedContent"
} -->

```http
HTTP/1.1 200 OK
Content-type: image/jpeg
Content-length: 201
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get chatMessageHostedContent",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
