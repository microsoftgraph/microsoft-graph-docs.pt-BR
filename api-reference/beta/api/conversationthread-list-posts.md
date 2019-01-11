---
title: Listar postagens
description: 'Obtenha as postagens do thread especificado. Você pode especificar tanto a conversa pai e o thread, ou, '
localization_priority: Normal
ms.openlocfilehash: da2fb8dadd18445cab051421d2c614bbbe9ec384
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27808754"
---
# <a name="list-posts"></a><span data-ttu-id="1f183-104">Listar postagens</span><span class="sxs-lookup"><span data-stu-id="1f183-104">List posts</span></span>

> <span data-ttu-id="1f183-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1f183-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1f183-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1f183-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1f183-p103">Obtenha as postagens do thread especificado. Você pode especificar a conversa pai e o thread ou apenas o thread, sem fazer referência à conversa pai.</span><span class="sxs-lookup"><span data-stu-id="1f183-p103">Get the posts of the specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="1f183-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="1f183-109">Permissions</span></span>
<span data-ttu-id="1f183-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f183-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f183-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1f183-112">Permission type</span></span>      | <span data-ttu-id="1f183-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1f183-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1f183-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1f183-114">Delegated (work or school account)</span></span> | <span data-ttu-id="1f183-115">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="1f183-115">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="1f183-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1f183-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f183-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1f183-117">Not supported.</span></span>    |
|<span data-ttu-id="1f183-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1f183-118">Application</span></span> | <span data-ttu-id="1f183-119">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="1f183-119">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1f183-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1f183-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts
GET /groups/{id}/conversations/{id}/threads/{id}/posts

```
## <a name="optional-query-parameters"></a><span data-ttu-id="1f183-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1f183-121">Optional query parameters</span></span>
<span data-ttu-id="1f183-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1f183-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1f183-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1f183-123">Request headers</span></span>
| <span data-ttu-id="1f183-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1f183-124">Header</span></span>       | <span data-ttu-id="1f183-125">Valor</span><span class="sxs-lookup"><span data-stu-id="1f183-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1f183-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="1f183-126">Authorization</span></span>  | <span data-ttu-id="1f183-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1f183-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1f183-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1f183-129">Request body</span></span>
<span data-ttu-id="1f183-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1f183-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f183-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f183-131">Response</span></span>

<span data-ttu-id="1f183-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Post](../resources/post.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1f183-132">If successful, this method returns a `200 OK` response code and collection of [Post](../resources/post.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1f183-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1f183-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1f183-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1f183-134">Request</span></span>
<span data-ttu-id="1f183-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1f183-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_posts"
}-->
```http
GET https://graph.microsoft.com/beta/groups/0d75b8dc-c42d-44dd-890a-751a99c0589f/threads/AAQkAD8EJUmcWwTJi06Cew==/posts
```
##### <a name="response"></a><span data-ttu-id="1f183-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f183-136">Response</span></span>
<span data-ttu-id="1f183-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1f183-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.post",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups('0d75b8dc-c42d-44dd-890a-751a99c0589f')/threads('AAQkAD8EJUmcWwTJi06Cew%3D%3D')/posts",
    "value":[
        {
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
