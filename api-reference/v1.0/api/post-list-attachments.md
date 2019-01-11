---
title: Listar anexos
description: Recupere uma lista de objetos attachment anexados a uma postagem.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 408d54049e74b017e1b57e2c810f2d32aadfff98
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859931"
---
# <a name="list-attachments"></a><span data-ttu-id="40f2c-103">Listar anexos</span><span class="sxs-lookup"><span data-stu-id="40f2c-103">List attachments</span></span>

<span data-ttu-id="40f2c-104">Recupere uma lista de objetos [attachment](../resources/attachment.md) anexados a uma postagem.</span><span class="sxs-lookup"><span data-stu-id="40f2c-104">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a post.</span></span>
## <a name="permissions"></a><span data-ttu-id="40f2c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="40f2c-105">Permissions</span></span>
<span data-ttu-id="40f2c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40f2c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40f2c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="40f2c-108">Permission type</span></span>      | <span data-ttu-id="40f2c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="40f2c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="40f2c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="40f2c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="40f2c-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40f2c-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="40f2c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="40f2c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40f2c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="40f2c-113">Not supported.</span></span>    |
|<span data-ttu-id="40f2c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="40f2c-114">Application</span></span> | <span data-ttu-id="40f2c-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40f2c-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="40f2c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="40f2c-116">HTTP request</span></span>
<span data-ttu-id="40f2c-117"><!-- { "blockType": "ignored" } -->Anexos de uma [postagem](../resources/post.md) em um [segmento](../resources/conversationthread.md) pertencente a uma [conversa](../resources/conversation.md) de um grupo.</span><span class="sxs-lookup"><span data-stu-id="40f2c-117"><!-- { "blockType": "ignored" } --> Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="40f2c-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="40f2c-118">Optional query parameters</span></span>
<span data-ttu-id="40f2c-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="40f2c-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="40f2c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="40f2c-120">Request headers</span></span>
| <span data-ttu-id="40f2c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="40f2c-121">Header</span></span>       | <span data-ttu-id="40f2c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="40f2c-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="40f2c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="40f2c-123">Authorization</span></span>  | <span data-ttu-id="40f2c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="40f2c-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="40f2c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="40f2c-126">Request body</span></span>
<span data-ttu-id="40f2c-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="40f2c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40f2c-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="40f2c-128">Response</span></span>

<span data-ttu-id="40f2c-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="40f2c-129">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="40f2c-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="40f2c-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="40f2c-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="40f2c-131">Request</span></span>
<span data-ttu-id="40f2c-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="40f2c-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="40f2c-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="40f2c-133">Response</span></span>
<span data-ttu-id="40f2c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="40f2c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.attachment)",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "value": [
    {
      "@odata.type": "microsoft.graph.fileAttachment",
      "id": "id-value",
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "base64-contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "datetime-value",
      "isInline": false,
      "name": "name-value",
      "size": 99
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
