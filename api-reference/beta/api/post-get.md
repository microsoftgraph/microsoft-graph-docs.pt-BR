---
title: Obter postagem
description: 'Obtenha as propriedades e os relacionamentos de uma postagem em um thread especificado. Você pode especificar ambas pai '
ms.openlocfilehash: e0aadef98da7056779993d0a7e11ec596cd97870
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040822"
---
# <a name="get-post"></a><span data-ttu-id="e88e4-104">Obter postagem</span><span class="sxs-lookup"><span data-stu-id="e88e4-104">Get post</span></span>

> <span data-ttu-id="e88e4-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e88e4-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e88e4-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e88e4-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e88e4-p103">Obtenha as propriedades e os relacionamentos de uma postagem em um thread especificado. Você pode especificar a conversa pai e o thread ou apenas o thread, sem fazer referência à conversa pai.</span><span class="sxs-lookup"><span data-stu-id="e88e4-p103">Get the properties and relationships of a post in a specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

<span data-ttu-id="e88e4-109">Como o recurso **post** dá suporte a [extensions](/graph/extensibility-overview), você também pode usar a operação `GET` para obter propriedades personalizadas e dados de extensão em uma instância de **post**.</span><span class="sxs-lookup"><span data-stu-id="e88e4-109">Since the **post** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **post** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="e88e4-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="e88e4-110">Permissions</span></span>
<span data-ttu-id="e88e4-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e88e4-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e88e4-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e88e4-113">Permission type</span></span>      | <span data-ttu-id="e88e4-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e88e4-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e88e4-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e88e4-115">Delegated (work or school account)</span></span> | <span data-ttu-id="e88e4-116">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e88e4-116">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e88e4-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e88e4-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e88e4-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e88e4-118">Not supported.</span></span>    |
|<span data-ttu-id="e88e4-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e88e4-119">Application</span></span> | <span data-ttu-id="e88e4-120">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e88e4-120">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e88e4-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e88e4-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e88e4-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e88e4-122">Optional query parameters</span></span>
<span data-ttu-id="e88e4-123">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e88e4-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e88e4-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e88e4-124">Request headers</span></span>
| <span data-ttu-id="e88e4-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e88e4-125">Header</span></span>       | <span data-ttu-id="e88e4-126">Valor</span><span class="sxs-lookup"><span data-stu-id="e88e4-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e88e4-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="e88e4-127">Authorization</span></span>  | <span data-ttu-id="e88e4-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e88e4-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e88e4-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e88e4-130">Request body</span></span>
<span data-ttu-id="e88e4-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e88e4-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e88e4-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="e88e4-132">Response</span></span>

<span data-ttu-id="e88e4-133">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [post](../resources/post.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e88e4-133">If successful, this method returns a `200 OK` response code and [post](../resources/post.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e88e4-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e88e4-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e88e4-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e88e4-135">Request</span></span>
<span data-ttu-id="e88e4-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e88e4-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_post"
}-->
```http
GET https://graph.microsoft.com/beta/groups/0d75b8dc-c42d-44dd-890a-751a99c0589f/threads/AAQkAD8EJUmcWwTJi06Cew==/posts/AQMkADgAAAIJbQAAAA==
```
##### <a name="response"></a><span data-ttu-id="e88e4-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="e88e4-137">Response</span></span>
<span data-ttu-id="e88e4-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e88e4-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.post"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups('0d75b8dc-c42d-44dd-890a-751a99c0589f')/threads('AAQkAD8EJUmcWwTJi06Cew%3D%3D')/posts/$entity",
    "@odata.etag":"W/\"CQAAABYAAAC/3QURwysWS6IJYYw5exv4AAAAAAlK\"",
    "id":"AQMkADgAAAIJbQAAAA==",
    "createdDateTime":"2018-01-11T17:36:17Z",
    "lastModifiedDateTime":"2018-01-11T17:36:17Z",
    "importance": "normal",
    "changeKey":"CQAAABYAAAC/3QURwysWS6IJYYw5exv4AAAAAAlK",
    "categories":[

    ],
    "receivedDateTime":"2018-01-11T17:36:17Z",
    "hasAttachments":false,
    "body":{
        "contentType":"html",
        "content":"<html><body></body></html>"
    },
    "from":{
        "emailAddress":{
            "name":"Marketing",
            "address":"Marketing@M365B489948.onmicrosoft.com"
        }
    },
    "sender":{
        "emailAddress":{
            "name":"Marketing",
            "address":"Marketing@M365B489948.onmicrosoft.com"
        }
    }
}
```

## <a name="see-also"></a><span data-ttu-id="e88e4-141">Confira também</span><span class="sxs-lookup"><span data-stu-id="e88e4-141">See also</span></span>

- [<span data-ttu-id="e88e4-142">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="e88e4-142">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="e88e4-143">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="e88e4-143">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="e88e4-144">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="e88e4-144">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get post",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
