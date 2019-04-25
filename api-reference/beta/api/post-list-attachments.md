---
title: Listar anexos
description: Recupere uma lista de objetos attachment anexados a uma postagem.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 910e269fb860ff21ecb80b8bcd247f9f9d43c947
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32546787"
---
# <a name="list-attachments"></a><span data-ttu-id="4484b-103">Listar anexos</span><span class="sxs-lookup"><span data-stu-id="4484b-103">List attachments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4484b-104">Recupere uma lista de objetos [attachment](../resources/attachment.md) anexados a uma postagem.</span><span class="sxs-lookup"><span data-stu-id="4484b-104">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a post.</span></span>
## <a name="permissions"></a><span data-ttu-id="4484b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4484b-105">Permissions</span></span>
<span data-ttu-id="4484b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4484b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4484b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4484b-108">Permission type</span></span>      | <span data-ttu-id="4484b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4484b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4484b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4484b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4484b-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4484b-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4484b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4484b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4484b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4484b-113">Not supported.</span></span>    |
|<span data-ttu-id="4484b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4484b-114">Application</span></span> | <span data-ttu-id="4484b-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4484b-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4484b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4484b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="4484b-117">Anexos de uma [post](../resources/post.md) em um [thread](../resources/conversationthread.md) que pertence a uma [conversation](../resources/conversation.md) de um grupo.</span><span class="sxs-lookup"><span data-stu-id="4484b-117">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4484b-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4484b-118">Optional query parameters</span></span>
<span data-ttu-id="4484b-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4484b-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="4484b-120">Em particular, você pode usar o $expand parâmetro de consulta para incluir todos os anexos de postagem embutidos com o restante das propriedades post.</span><span class="sxs-lookup"><span data-stu-id="4484b-120">In particular, you can use the $expand query parameter to include all of the post attachments inline with the rest of the post properties.</span></span> <span data-ttu-id="4484b-121">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="4484b-121">For example:</span></span>

```
GET https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}?$expand=attachments
```
## <a name="request-headers"></a><span data-ttu-id="4484b-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4484b-122">Request headers</span></span>
| <span data-ttu-id="4484b-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4484b-123">Header</span></span>       | <span data-ttu-id="4484b-124">Valor</span><span class="sxs-lookup"><span data-stu-id="4484b-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4484b-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="4484b-125">Authorization</span></span>  | <span data-ttu-id="4484b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4484b-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4484b-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4484b-128">Request body</span></span>
<span data-ttu-id="4484b-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4484b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4484b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="4484b-130">Response</span></span>

<span data-ttu-id="4484b-131">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4484b-131">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4484b-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4484b-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4484b-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4484b-133">Request</span></span>
<span data-ttu-id="4484b-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4484b-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="4484b-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="4484b-135">Response</span></span>
<span data-ttu-id="4484b-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4484b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
