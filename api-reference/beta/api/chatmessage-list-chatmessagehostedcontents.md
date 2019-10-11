---
title: Listar chatMessageHostedContents
description: Recupere a lista de objetos chatMessageHostedContent de uma mensagem.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: cc43513ea215f9e4a0d037c39fb9e9fe560e0bb3
ms.sourcegitcommit: e4b0211db9b20dfea8be964003661cd99fe064d1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/10/2019
ms.locfileid: "37439867"
---
# <a name="list-hostedcontents"></a><span data-ttu-id="73d21-103">Listar hostedContents</span><span class="sxs-lookup"><span data-stu-id="73d21-103">List hostedContents</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73d21-104">Recupere a lista de objetos [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="73d21-104">Retrieve the list of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) objects from a message.</span></span>

## <a name="permissions"></a><span data-ttu-id="73d21-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="73d21-105">Permissions</span></span>

<span data-ttu-id="73d21-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73d21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="73d21-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="73d21-108">Permission type</span></span>                        | <span data-ttu-id="73d21-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="73d21-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="73d21-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="73d21-110">Delegated (work or school account)</span></span>|<span data-ttu-id="73d21-111">Para o **usuário** ou recurso de **chat** :</span><span class="sxs-lookup"><span data-stu-id="73d21-111">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="73d21-112">Chat. Read, chat. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73d21-112">Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="73d21-113">Para o recurso de **canal** :</span><span class="sxs-lookup"><span data-stu-id="73d21-113">For **channel** resource:</span></span><br/><span data-ttu-id="73d21-114">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73d21-114">Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="73d21-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="73d21-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73d21-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="73d21-116">Not supported</span></span>|
|<span data-ttu-id="73d21-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="73d21-117">Application</span></span>| <span data-ttu-id="73d21-118">Para o **usuário** ou recurso de **chat** :</span><span class="sxs-lookup"><span data-stu-id="73d21-118">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="73d21-119">Chat. Read. All, chat. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="73d21-119">Chat.Read.All, Chat.ReadWrite.All</span></span><br/><br/><span data-ttu-id="73d21-120">Para o recurso de **canal** :</span><span class="sxs-lookup"><span data-stu-id="73d21-120">For **channel** resource:</span></span><br/><span data-ttu-id="73d21-121">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73d21-121">Group.Read.All, Group.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="73d21-122">Antes de chamar esta API com permissões de aplicativo, você deve solicitar acesso.</span><span class="sxs-lookup"><span data-stu-id="73d21-122">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="73d21-123">Para obter detalhes, consulte [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="73d21-123">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="73d21-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="73d21-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{id}/messages/{id}/hostedContents
GET /users/{id}/chats/{id}/messages/{id}/hostedContents
GET /teams/{id}/channels/{id}/messages/{id}/hostedContents
```

## <a name="optional-query-parameters"></a><span data-ttu-id="73d21-125">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="73d21-125">Optional query parameters</span></span>

<span data-ttu-id="73d21-126">Esta operação não oferece suporte aos [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="73d21-126">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="73d21-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="73d21-127">Request headers</span></span>

| <span data-ttu-id="73d21-128">Nome</span><span class="sxs-lookup"><span data-stu-id="73d21-128">Name</span></span>      |<span data-ttu-id="73d21-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="73d21-129">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="73d21-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="73d21-130">Authorization</span></span> | <span data-ttu-id="73d21-131">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="73d21-131">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="73d21-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="73d21-132">Request body</span></span>

<span data-ttu-id="73d21-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="73d21-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73d21-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="73d21-134">Response</span></span>

<span data-ttu-id="73d21-135">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="73d21-135">If successful, this method returns a `200 OK` response code and a collection of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="73d21-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="73d21-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="73d21-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="73d21-137">Request</span></span>

<span data-ttu-id="73d21-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="73d21-138">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="73d21-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="73d21-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_hostedcontents"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/{id}/messages/{id}/hostedContents
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="73d21-140">C#</span><span class="sxs-lookup"><span data-stu-id="73d21-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-hostedcontents-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="73d21-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="73d21-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-hostedcontents-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="73d21-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="73d21-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-hostedcontents-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="73d21-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="73d21-143">Response</span></span>

<span data-ttu-id="73d21-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="73d21-144">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="73d21-145">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="73d21-145">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="73d21-146">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="73d21-146">All the properties will be returned from an actual call.</span></span>

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
  "tocPath": "",
  "suppressions": [
  ]
}-->
