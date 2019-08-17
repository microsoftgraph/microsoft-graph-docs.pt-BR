---
title: Listar anexos
description: Recupere uma lista de objetos anexados a uma mensagem.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 01024da4bc2c33c763ad759cb043da2069fd3a9e
ms.sourcegitcommit: 36066afdced00f32838a03747d3e7760fc43683a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/17/2019
ms.locfileid: "36453162"
---
# <a name="list-attachments"></a><span data-ttu-id="f23b1-103">Listar anexos</span><span class="sxs-lookup"><span data-stu-id="f23b1-103">List attachments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f23b1-104">Recupere uma lista de objetos [attachment](../resources/attachment.md) anexados a uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="f23b1-104">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a message.</span></span>
## <a name="permissions"></a><span data-ttu-id="f23b1-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f23b1-105">Permissions</span></span>
<span data-ttu-id="f23b1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f23b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f23b1-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f23b1-108">Permission type</span></span>      | <span data-ttu-id="f23b1-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f23b1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f23b1-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f23b1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f23b1-111">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="f23b1-111">Mail.Read</span></span>    |
|<span data-ttu-id="f23b1-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f23b1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f23b1-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="f23b1-113">Mail.Read</span></span>    |
|<span data-ttu-id="f23b1-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f23b1-114">Application</span></span> | <span data-ttu-id="f23b1-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="f23b1-115">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="f23b1-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f23b1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="f23b1-117">Anexos de uma [message](../resources/message.md) em uma caixa de correio de usuário.</span><span class="sxs-lookup"><span data-stu-id="f23b1-117">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
GET /me/messages/{id}/attachments
GET /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="f23b1-118">Anexos de uma [message](../resources/message.md) contidos em uma [mailFolder](../resources/mailfolder.md) de nível superior na caixa de correio de um usuário.</span><span class="sxs-lookup"><span data-stu-id="f23b1-118">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
GET /me/mailFolders/{id}/messages/{id}/attachments
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="f23b1-p102">Anexos de uma [message](../resources/message.md) contidos em uma pasta filha de uma [mailFolder](../resources/mailfolder.md) na caixa de correio de um usuário.  O exemplo a seguir mostra um nível de aninhamento, mas uma mensagem pode estar localizada em um filho de um filho, e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="f23b1-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f23b1-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f23b1-121">Optional query parameters</span></span>
<span data-ttu-id="f23b1-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f23b1-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="f23b1-123">Em particular, você pode usar o $expand parâmetro de consulta para incluir todos os anexos de mensagem embutidos com o restante das propriedades de mensagem.</span><span class="sxs-lookup"><span data-stu-id="f23b1-123">In particular, you can use the $expand query parameter to include all of the message attachments inline with the rest of the message properties.</span></span> <span data-ttu-id="f23b1-124">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="f23b1-124">For example:</span></span>

```
GET https://graph.microsoft.com/beta/me/messages/{id}?$expand=attachments
```
## <a name="request-headers"></a><span data-ttu-id="f23b1-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f23b1-125">Request headers</span></span>
| <span data-ttu-id="f23b1-126">Nome</span><span class="sxs-lookup"><span data-stu-id="f23b1-126">Name</span></span>       | <span data-ttu-id="f23b1-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="f23b1-127">Type</span></span> | <span data-ttu-id="f23b1-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="f23b1-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f23b1-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="f23b1-129">Authorization</span></span>  | <span data-ttu-id="f23b1-130">string</span><span class="sxs-lookup"><span data-stu-id="f23b1-130">string</span></span>  | <span data-ttu-id="f23b1-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f23b1-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f23b1-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f23b1-133">Request body</span></span>
<span data-ttu-id="f23b1-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f23b1-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f23b1-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f23b1-135">Response</span></span>

<span data-ttu-id="f23b1-136">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f23b1-136">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f23b1-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f23b1-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f23b1-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f23b1-138">Request</span></span>
<span data-ttu-id="f23b1-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f23b1-139">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f23b1-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="f23b1-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_get_attachments_beta"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages/{id}/attachments
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f23b1-141">C#</span><span class="sxs-lookup"><span data-stu-id="f23b1-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-get-attachments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f23b1-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f23b1-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-get-attachments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f23b1-143">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="f23b1-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-get-attachments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f23b1-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="f23b1-144">Response</span></span>
<span data-ttu-id="f23b1-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f23b1-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "message_get_attachments_beta",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAttachment",
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
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "2016-10-19T10:37:00Z",
      "id": "id-value",
      "isInline": false,
      "isContactPhoto": false,
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
  ]
}
-->
