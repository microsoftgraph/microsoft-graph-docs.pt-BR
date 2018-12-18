---
title: Obter a mensagem de canal
description: Recupere uma única mensagem (sem respectivas respostas) em um canal de uma equipe.
author: nkramer
ms.openlocfilehash: 2da10f4151cc1ddaaa1bddfe376f4035a6baa180
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309223"
---
# <a name="get-channel-message"></a><span data-ttu-id="29faa-103">Obter a mensagem de canal</span><span class="sxs-lookup"><span data-stu-id="29faa-103">Get channel message</span></span>

> <span data-ttu-id="29faa-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="29faa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="29faa-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="29faa-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="29faa-106">Recupere uma única [mensagem](../resources/chatmessage.md) (sem respectivas respostas) em um [canal](../resources/channel.md) de uma equipe.</span><span class="sxs-lookup"><span data-stu-id="29faa-106">Retrieve a single [message](../resources/chatmessage.md) (without its replies) in a [channel](../resources/channel.md) of a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="29faa-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="29faa-107">Permissions</span></span>
<span data-ttu-id="29faa-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29faa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29faa-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="29faa-110">Permission Type</span></span>|<span data-ttu-id="29faa-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="29faa-111">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="29faa-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="29faa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="29faa-113">Group.Read.All,Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29faa-113">Group.Read.All,Group.ReadWrite.All</span></span>|
|<span data-ttu-id="29faa-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="29faa-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29faa-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="29faa-115">Not supported</span></span>|
|<span data-ttu-id="29faa-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="29faa-116">Application</span></span>| <span data-ttu-id="29faa-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="29faa-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="29faa-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="29faa-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="29faa-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="29faa-119">Optional query parameters</span></span>
<span data-ttu-id="29faa-120">Os [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) não são suportados no momento.</span><span class="sxs-lookup"><span data-stu-id="29faa-120">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="29faa-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="29faa-121">Request headers</span></span>
| <span data-ttu-id="29faa-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="29faa-122">Header</span></span>       | <span data-ttu-id="29faa-123">Valor</span><span class="sxs-lookup"><span data-stu-id="29faa-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="29faa-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="29faa-124">Authorization</span></span>  | <span data-ttu-id="29faa-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="29faa-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="29faa-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="29faa-127">Request body</span></span>
<span data-ttu-id="29faa-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="29faa-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="29faa-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="29faa-129">Response</span></span>

<span data-ttu-id="29faa-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [chatmessage](../resources/chatmessage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="29faa-130">If successful, this method returns a `200 OK` response code and a collection of [chatmessage](../resources/chatmessage.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29faa-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="29faa-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="29faa-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="29faa-132">Request</span></span>
<span data-ttu-id="29faa-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="29faa-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channel_message"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="29faa-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="29faa-134">Response</span></span>
<span data-ttu-id="29faa-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="29faa-135">Here is an example of the response.</span></span> 

><span data-ttu-id="29faa-136">**Observação:** No objeto response mostrado aqui são reduzidos para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="29faa-136">**Note:** The response object shown here are shortened for readability.</span></span> <span data-ttu-id="29faa-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="29faa-137">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
  "id": "id-value",
  "replyToId": "id-value",
  "from": {
      "user": { 
        "id": "id-value",
        "displayName": "John Doe"
      }  
  },
  "etag": "id-value",
  "messageType": "message",
  "createdDateTime": "2018-07-09T07:40:20.152Z",
  "lastModifiedDateTime": "2018-07-09T07:40:20.152Z",
  "body": {
      "content": "Hello World",
      "contentType": "text"
  },
  "attachments": [
        {
            "id": "5e32f195-168a-474f-a273-123123123",
            "contentType": "reference",
            "contentUrl": "https://test.sharepoint.com/sites/TestSite/Shared%20Documents/General/Test.txt",
            "content": null,
            "name": "Test.txt",
            "thumbnailUrl": null
        }
  ],
  "mentions": [
      {
          "type": "user",
          "id": "id-value ",
          "mentionText": "Test User"
      }
  ],
  "importance": "normal",
  "reactions": [
      {
        "reactionType": "like",
        "user": {
            "id": "id-value",
            "displayName": "John Doe"
        },
        "createdDateTime": "2018-07-09T07:40:20.152Z"
      }
  ],
  "locale": "en-us"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get channel message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
