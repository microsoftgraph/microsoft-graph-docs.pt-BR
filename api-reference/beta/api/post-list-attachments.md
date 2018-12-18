---
title: Listar anexos
description: Recupere uma lista de objetos attachment anexados a uma postagem.
author: dkershaw10
ms.openlocfilehash: f03cf2b9039c88690ddd4078ebe7c843b2e1766a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321606"
---
# <a name="list-attachments"></a><span data-ttu-id="e9d96-103">Listar anexos</span><span class="sxs-lookup"><span data-stu-id="e9d96-103">List attachments</span></span>

> <span data-ttu-id="e9d96-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e9d96-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e9d96-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e9d96-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e9d96-106">Recupere uma lista de objetos [attachment](../resources/attachment.md) anexados a uma postagem.</span><span class="sxs-lookup"><span data-stu-id="e9d96-106">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a post.</span></span>
## <a name="permissions"></a><span data-ttu-id="e9d96-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="e9d96-107">Permissions</span></span>
<span data-ttu-id="e9d96-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9d96-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9d96-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e9d96-110">Permission type</span></span>      | <span data-ttu-id="e9d96-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e9d96-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e9d96-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e9d96-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e9d96-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9d96-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e9d96-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e9d96-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9d96-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9d96-115">Not supported.</span></span>    |
|<span data-ttu-id="e9d96-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e9d96-116">Application</span></span> | <span data-ttu-id="e9d96-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9d96-117">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e9d96-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e9d96-118">HTTP request</span></span>
<span data-ttu-id="e9d96-119"><!-- { "blockType": "ignored" } -->Anexos de uma [postagem](../resources/post.md) em um [segmento](../resources/conversationthread.md) pertencente a uma [conversa](../resources/conversation.md) de um grupo.</span><span class="sxs-lookup"><span data-stu-id="e9d96-119"><!-- { "blockType": "ignored" } --> Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e9d96-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e9d96-120">Optional query parameters</span></span>
<span data-ttu-id="e9d96-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e9d96-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="e9d96-122">Em particular, você pode usar o $expandir o parâmetro de consulta para incluir todos os o embutido de anexos post com o restante das propriedades post.</span><span class="sxs-lookup"><span data-stu-id="e9d96-122">In particular, you can use the $expand query parameter to include all of the post attachments inline with the rest of the post properties.</span></span> <span data-ttu-id="e9d96-123">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="e9d96-123">For example:</span></span>

```
GET https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}?$expand=attachments
```
## <a name="request-headers"></a><span data-ttu-id="e9d96-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e9d96-124">Request headers</span></span>
| <span data-ttu-id="e9d96-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e9d96-125">Header</span></span>       | <span data-ttu-id="e9d96-126">Valor</span><span class="sxs-lookup"><span data-stu-id="e9d96-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e9d96-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="e9d96-127">Authorization</span></span>  | <span data-ttu-id="e9d96-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e9d96-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e9d96-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e9d96-130">Request body</span></span>
<span data-ttu-id="e9d96-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e9d96-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e9d96-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9d96-132">Response</span></span>

<span data-ttu-id="e9d96-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e9d96-133">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e9d96-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e9d96-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e9d96-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e9d96-135">Request</span></span>
<span data-ttu-id="e9d96-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e9d96-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="e9d96-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9d96-137">Response</span></span>
<span data-ttu-id="e9d96-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e9d96-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
