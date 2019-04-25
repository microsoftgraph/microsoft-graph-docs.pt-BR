---
title: Listar anexos
description: Recupere uma lista de objetos attachment anexados a uma postagem.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 5000ed8f65c0dd982a341ceff5c125dada073290
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32574282"
---
# <a name="list-attachments"></a><span data-ttu-id="04c46-103">Listar anexos</span><span class="sxs-lookup"><span data-stu-id="04c46-103">List attachments</span></span>

<span data-ttu-id="04c46-104">Recupere uma lista de objetos [attachment](../resources/attachment.md) anexados a uma postagem.</span><span class="sxs-lookup"><span data-stu-id="04c46-104">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a post.</span></span>
## <a name="permissions"></a><span data-ttu-id="04c46-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="04c46-105">Permissions</span></span>
<span data-ttu-id="04c46-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04c46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04c46-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="04c46-108">Permission type</span></span>      | <span data-ttu-id="04c46-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="04c46-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="04c46-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="04c46-110">Delegated (work or school account)</span></span> | <span data-ttu-id="04c46-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04c46-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="04c46-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="04c46-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04c46-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="04c46-113">Not supported.</span></span>    |
|<span data-ttu-id="04c46-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="04c46-114">Application</span></span> | <span data-ttu-id="04c46-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04c46-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="04c46-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="04c46-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="04c46-117">Anexos de uma [post](../resources/post.md) em um [thread](../resources/conversationthread.md) que pertence a uma [conversation](../resources/conversation.md) de um grupo.</span><span class="sxs-lookup"><span data-stu-id="04c46-117">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="04c46-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="04c46-118">Optional query parameters</span></span>
<span data-ttu-id="04c46-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="04c46-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="04c46-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="04c46-120">Request headers</span></span>
| <span data-ttu-id="04c46-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="04c46-121">Header</span></span>       | <span data-ttu-id="04c46-122">Valor</span><span class="sxs-lookup"><span data-stu-id="04c46-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="04c46-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="04c46-123">Authorization</span></span>  | <span data-ttu-id="04c46-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="04c46-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="04c46-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="04c46-126">Request body</span></span>
<span data-ttu-id="04c46-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="04c46-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="04c46-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="04c46-128">Response</span></span>

<span data-ttu-id="04c46-129">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="04c46-129">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="04c46-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="04c46-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="04c46-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="04c46-131">Request</span></span>
<span data-ttu-id="04c46-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="04c46-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="04c46-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="04c46-133">Response</span></span>
<span data-ttu-id="04c46-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="04c46-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
