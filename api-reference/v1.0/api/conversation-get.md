---
title: Obter conversation
description: Recupera as propriedades e os relacionamentos do objeto conversation.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 174d5a5b5309348de5ebf01d38445d032d9e31ff
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566133"
---
# <a name="get-conversation"></a><span data-ttu-id="4f553-103">Obter conversa</span><span class="sxs-lookup"><span data-stu-id="4f553-103">Get conversation</span></span>

<span data-ttu-id="4f553-104">Recupera as propriedades e os relacionamentos do objeto conversation.</span><span class="sxs-lookup"><span data-stu-id="4f553-104">Retrieve the properties and relationships of conversation object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4f553-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4f553-105">Permissions</span></span>
<span data-ttu-id="4f553-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f553-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f553-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4f553-108">Permission type</span></span>      | <span data-ttu-id="4f553-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4f553-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4f553-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4f553-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4f553-111">Group. ReadWrite. All, Group. Read. All</span><span class="sxs-lookup"><span data-stu-id="4f553-111">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="4f553-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4f553-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f553-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f553-113">Not supported.</span></span>    |
|<span data-ttu-id="4f553-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4f553-114">Application</span></span> | <span data-ttu-id="4f553-115">Group. ReadWrite. All, Group. Read. All</span><span class="sxs-lookup"><span data-stu-id="4f553-115">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4f553-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4f553-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}

```
## <a name="optional-query-parameters"></a><span data-ttu-id="4f553-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4f553-117">Optional query parameters</span></span>
<span data-ttu-id="4f553-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4f553-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4f553-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4f553-119">Request headers</span></span>
| <span data-ttu-id="4f553-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4f553-120">Header</span></span>       | <span data-ttu-id="4f553-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4f553-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4f553-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4f553-122">Authorization</span></span>  | <span data-ttu-id="4f553-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4f553-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4f553-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4f553-125">Request body</span></span>
<span data-ttu-id="4f553-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4f553-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4f553-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f553-127">Response</span></span>

<span data-ttu-id="4f553-128">Se bem sucedido, este método retorna um código de resposta `200 OK` e um objeto [conversation](../resources/conversation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4f553-128">If successful, this method returns a `200 OK` response code and [conversation](../resources/conversation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4f553-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4f553-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4f553-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4f553-130">Request</span></span>
<span data-ttu-id="4f553-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4f553-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversation"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/conversations/{id}
```
##### <a name="response"></a><span data-ttu-id="4f553-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f553-132">Response</span></span>
<span data-ttu-id="4f553-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4f553-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
  "topic": "topic-value",
  "hasAttachments": true,
  "lastDeliveredDateTime": "datetime-value",
  "uniqueSenders": [
    "uniqueSenders-value"
  ],
  "preview": "preview-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
