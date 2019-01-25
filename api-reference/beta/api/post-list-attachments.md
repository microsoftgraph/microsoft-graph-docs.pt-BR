---
title: Listar anexos
description: Recupere uma lista de objetos attachment anexados a uma postagem.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 910e269fb860ff21ecb80b8bcd247f9f9d43c947
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527009"
---
# <a name="list-attachments"></a><span data-ttu-id="7fc19-103">Listar anexos</span><span class="sxs-lookup"><span data-stu-id="7fc19-103">List attachments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7fc19-104">Recupere uma lista de objetos [attachment](../resources/attachment.md) anexados a uma postagem.</span><span class="sxs-lookup"><span data-stu-id="7fc19-104">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a post.</span></span>
## <a name="permissions"></a><span data-ttu-id="7fc19-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="7fc19-105">Permissions</span></span>
<span data-ttu-id="7fc19-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7fc19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7fc19-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7fc19-108">Permission type</span></span>      | <span data-ttu-id="7fc19-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7fc19-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7fc19-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7fc19-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7fc19-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7fc19-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7fc19-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7fc19-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7fc19-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7fc19-113">Not supported.</span></span>    |
|<span data-ttu-id="7fc19-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7fc19-114">Application</span></span> | <span data-ttu-id="7fc19-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7fc19-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7fc19-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7fc19-116">HTTP request</span></span>
<span data-ttu-id="7fc19-117"><!-- { "blockType": "ignored" } -->Anexos de uma [postagem](../resources/post.md) em um [segmento](../resources/conversationthread.md) pertencente a uma [conversa](../resources/conversation.md) de um grupo.</span><span class="sxs-lookup"><span data-stu-id="7fc19-117"><!-- { "blockType": "ignored" } --> Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7fc19-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7fc19-118">Optional query parameters</span></span>
<span data-ttu-id="7fc19-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7fc19-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="7fc19-120">Em particular, você pode usar o $expandir o parâmetro de consulta para incluir todos os o embutido de anexos post com o restante das propriedades post.</span><span class="sxs-lookup"><span data-stu-id="7fc19-120">In particular, you can use the $expand query parameter to include all of the post attachments inline with the rest of the post properties.</span></span> <span data-ttu-id="7fc19-121">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="7fc19-121">For example:</span></span>

```
GET https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}?$expand=attachments
```
## <a name="request-headers"></a><span data-ttu-id="7fc19-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7fc19-122">Request headers</span></span>
| <span data-ttu-id="7fc19-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7fc19-123">Header</span></span>       | <span data-ttu-id="7fc19-124">Valor</span><span class="sxs-lookup"><span data-stu-id="7fc19-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7fc19-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="7fc19-125">Authorization</span></span>  | <span data-ttu-id="7fc19-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7fc19-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7fc19-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7fc19-128">Request body</span></span>
<span data-ttu-id="7fc19-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7fc19-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7fc19-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="7fc19-130">Response</span></span>

<span data-ttu-id="7fc19-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7fc19-131">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7fc19-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7fc19-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7fc19-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7fc19-133">Request</span></span>
<span data-ttu-id="7fc19-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7fc19-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="7fc19-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="7fc19-135">Response</span></span>
<span data-ttu-id="7fc19-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7fc19-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "value": [
    {
      "@odata.type": "#Microsoft.OutlookServices.FileAttachment",
      "id": "id-value",
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "2016-10-19T10:37:00Z",
      "isInline": false,
      "name": "name-value",
      "size": 99
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/post-list-attachments.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
