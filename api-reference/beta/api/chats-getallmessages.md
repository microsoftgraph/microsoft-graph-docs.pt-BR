---
title: 'chats: getAllMessages'
description: Obter mensagens de todos os chats nos quais um usuário é um participante.
author: RamjotSingh
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 18c6ec164d21c1efab249560f3c866fab5fabeb4
ms.sourcegitcommit: a9a035e7cf7b500aebe5477c05361552e7c3a7ab
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/28/2021
ms.locfileid: "52695928"
---
# <a name="chats-getallmessages"></a><span data-ttu-id="fb3f6-103">chats: getAllMessages</span><span class="sxs-lookup"><span data-stu-id="fb3f6-103">chats: getAllMessages</span></span>

<span data-ttu-id="fb3f6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb3f6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb3f6-105">Obtenha todas as mensagens de todos os [chats](../resources/chatmessage.md) de que um usuário é um participante, incluindo chats individuais, chats de grupo e chats de reunião.</span><span class="sxs-lookup"><span data-stu-id="fb3f6-105">Get all messages from all [chats](../resources/chatmessage.md) that a user is a participant in, including one-on-one chats, group chats, and meeting chats.</span></span>

## <a name="permissions"></a><span data-ttu-id="fb3f6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fb3f6-106">Permissions</span></span>

<span data-ttu-id="fb3f6-p101">As seguintes permissões são obrigatórias para chamar esta API. Para saber mais, incluindo como escolher as permissões, consulte [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb3f6-p101">The following permissions are required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb3f6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fb3f6-109">Permission type</span></span>      | <span data-ttu-id="fb3f6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fb3f6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fb3f6-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fb3f6-111">Delegated (work or school account)</span></span>| <span data-ttu-id="fb3f6-112">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="fb3f6-112">Not supported</span></span> |
|<span data-ttu-id="fb3f6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fb3f6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb3f6-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="fb3f6-114">Not supported</span></span> |
|<span data-ttu-id="fb3f6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fb3f6-115">Application</span></span> | <span data-ttu-id="fb3f6-116">Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb3f6-116">Chat.Read.All, Chat.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="fb3f6-117">É necessário solicitar acesso antes de chamar essa API com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fb3f6-117">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="fb3f6-118">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="fb3f6-118">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="fb3f6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fb3f6-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | user-principal-name}/chats/getAllMessages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fb3f6-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fb3f6-120">Optional query parameters</span></span>

<span data-ttu-id="fb3f6-121">Esta operação dá suporte aos [parâmetros de intervalo de datas](/graph/query-parameters) para personalizar a resposta, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="fb3f6-121">This operation supports [date range parameters](/graph/query-parameters) to customize the response, as shown in the following example.</span></span>

```http
GET /users/{id}/chats/getAllMessages?$top=50&$filter=lastModifiedDateTime gt 2020-06-04T18:03:11.591Z and lastModifiedDateTime lt 2020-06-05T21:00:09.413Z
```

## <a name="request-headers"></a><span data-ttu-id="fb3f6-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fb3f6-122">Request headers</span></span>
| <span data-ttu-id="fb3f6-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fb3f6-123">Header</span></span>       | <span data-ttu-id="fb3f6-124">Valor</span><span class="sxs-lookup"><span data-stu-id="fb3f6-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fb3f6-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="fb3f6-125">Authorization</span></span>  | <span data-ttu-id="fb3f6-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fb3f6-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="fb3f6-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb3f6-128">Response</span></span>

<span data-ttu-id="fb3f6-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [event](../resources/chatmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fb3f6-129">If successful, this method returns a `200 OK` response code and a list of [chatMessages](../resources/chatmessage.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb3f6-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fb3f6-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="fb3f6-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb3f6-131">Request</span></span>

```msgraph-interactive
GET https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5/chats/getAllMessages
```

### <a name="response"></a><span data-ttu-id="fb3f6-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb3f6-132">Response</span></span>

><span data-ttu-id="fb3f6-133">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="fb3f6-133">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK 
Content-type: application/json 
Content-length: 347 

{
   "@odata.context":"https://graph.microsoft.com/beta/$metadata#Collection(chatMessage)",
   "@odata.count":10,
   "@odata.nextLink":"https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5/chats/getAllMessages?$skip=10",
   "value":[
      {
         "@odata.type":"#microsoft.graph.chatMessage",
         "id":"1600457965467",
         "replyToId":null,
         "etag":"1600457965467",
         "messageType":"message",
         "createdDateTime":"2020-09-18T19:39:25.467Z",
         "lastModifiedDateTime":"2020-09-18T19:39:25.467Z",
         "lastEditedDateTime":null,
         "deletedDateTime":null,
         "subject":null,
         "summary":null,
         "chatId":"19:0de69e5e-2da8-4cf2-821f-5e6585b2c65b_5c64e248-3269-4268-a36e-0f80314e9c39@unq.gbl.spaces",
         "importance":"normal",
         "locale":"en-us",
         "webUrl":null,
         "channelIdentity":null,
         "policyViolation":null,
         "from":{
            "application":null,
            "device":null,
            "conversation":null,
            "user":{
               "id":"0de69e5e-2da8-4cf2-821f-5e6585b2c65b",
               "displayName":"Richard Wilson",
               "userIdentityType":"aadUser"
            }
         },
         "body":{
            "contentType":"html",
            "content":"<div>\n<blockquote itemscope=\"\" itemtype=\"http://schema.skype.com/Reply\" itemid=\"1600457867820\">\n<strong itemprop=\"mri\" itemid=\"8:orgid:0de69e5e-2da8-4cf2-821f-5e6585b2c65b\">Richard Wilson</strong><span itemprop=\"time\" itemid=\"1600457867820\"></span>\n<p itemprop=\"preview\">1237</p>\n</blockquote>\n<p>this is a reply</p>\n</div>"
         },
         "attachments":[
            
         ],
         "mentions":[
            
         ],
         "reactions":[
            
         ]
      }
   ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chats: getallmessages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
