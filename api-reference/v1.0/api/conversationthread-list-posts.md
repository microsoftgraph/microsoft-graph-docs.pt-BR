---
title: Listar postagens
description: 'Obtenha as postagens do thread especificado. Você pode especificar tanto a conversa pai e o thread, ou, '
ms.openlocfilehash: 35c4c178b02cb700ab21a324c29a4522203fad19
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005002"
---
# <a name="list-posts"></a><span data-ttu-id="77b7d-104">Listar postagens</span><span class="sxs-lookup"><span data-stu-id="77b7d-104">List posts</span></span>

<span data-ttu-id="77b7d-p102">Obtenha as postagens do thread especificado. Você pode especificar a conversa pai e o thread ou apenas o thread, sem fazer referência à conversa pai.</span><span class="sxs-lookup"><span data-stu-id="77b7d-p102">Get the posts of the specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="77b7d-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="77b7d-107">Permissions</span></span>
<span data-ttu-id="77b7d-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77b7d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77b7d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="77b7d-110">Permission type</span></span>      | <span data-ttu-id="77b7d-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="77b7d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="77b7d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="77b7d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="77b7d-113">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="77b7d-113">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="77b7d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="77b7d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77b7d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="77b7d-115">Not supported.</span></span>    |
|<span data-ttu-id="77b7d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="77b7d-116">Application</span></span> | <span data-ttu-id="77b7d-117">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="77b7d-117">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="77b7d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="77b7d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts
GET /groups/{id}/conversations/{id}/threads/{id}/posts

```
## <a name="optional-query-parameters"></a><span data-ttu-id="77b7d-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="77b7d-119">Optional query parameters</span></span>
<span data-ttu-id="77b7d-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="77b7d-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="77b7d-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="77b7d-121">Request headers</span></span>
| <span data-ttu-id="77b7d-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="77b7d-122">Header</span></span>       | <span data-ttu-id="77b7d-123">Valor</span><span class="sxs-lookup"><span data-stu-id="77b7d-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="77b7d-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="77b7d-124">Authorization</span></span>  | <span data-ttu-id="77b7d-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="77b7d-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="77b7d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="77b7d-127">Request body</span></span>
<span data-ttu-id="77b7d-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="77b7d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77b7d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="77b7d-129">Response</span></span>

<span data-ttu-id="77b7d-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Post](../resources/post.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="77b7d-130">If successful, this method returns a `200 OK` response code and collection of [Post](../resources/post.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="77b7d-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="77b7d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="77b7d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="77b7d-132">Request</span></span>
<span data-ttu-id="77b7d-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="77b7d-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_posts"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts
```
##### <a name="response"></a><span data-ttu-id="77b7d-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="77b7d-134">Response</span></span>
<span data-ttu-id="77b7d-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="77b7d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.post",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 523

{
  "value": [
    {
      "body": {
        "contentType": "",
        "content": "content-value"
      },
      "receivedDateTime": "datetime-value",
      "hasAttachments": true,
      "from": {
        "emailAddress": {
          "name": "name-value",
          "address": "address-value"
        }
      },
      "sender": {
        "emailAddress": {
          "name": "name-value",
          "address": "address-value"
        }
      },
      "conversationThreadId": "conversationThreadId-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List posts",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
