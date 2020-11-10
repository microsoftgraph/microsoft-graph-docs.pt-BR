---
title: Listar anexos
description: Recupere uma lista de objetos anexados a uma mensagem.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 73b6bb66c96d67093f398525ab26b4c0262a8251
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979814"
---
# <a name="list-attachments"></a><span data-ttu-id="b152e-103">Listar anexos</span><span class="sxs-lookup"><span data-stu-id="b152e-103">List attachments</span></span>

<span data-ttu-id="b152e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b152e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b152e-105">Recupere uma lista de objetos [attachment](../resources/attachment.md) anexados a uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="b152e-105">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a message.</span></span>
## <a name="permissions"></a><span data-ttu-id="b152e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b152e-106">Permissions</span></span>
<span data-ttu-id="b152e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b152e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b152e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b152e-109">Permission type</span></span>      | <span data-ttu-id="b152e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b152e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b152e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b152e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b152e-112">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="b152e-112">Mail.Read</span></span>    |
|<span data-ttu-id="b152e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b152e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b152e-114">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="b152e-114">Mail.Read</span></span>    |
|<span data-ttu-id="b152e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b152e-115">Application</span></span> | <span data-ttu-id="b152e-116">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="b152e-116">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="b152e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b152e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="b152e-118">Anexos de uma [message](../resources/message.md) em uma caixa de correio de usuário.</span><span class="sxs-lookup"><span data-stu-id="b152e-118">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
GET /me/messages/{id}/attachments
GET /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="b152e-119">Anexos de uma [message](../resources/message.md) contidos em uma [mailFolder](../resources/mailfolder.md) de nível superior na caixa de correio de um usuário.</span><span class="sxs-lookup"><span data-stu-id="b152e-119">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
GET /me/mailFolders/{id}/messages/{id}/attachments
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="b152e-p102">Anexos de uma [message](../resources/message.md) contidos em uma pasta filha de uma [mailFolder](../resources/mailfolder.md) na caixa de correio de um usuário.  O exemplo a seguir mostra um nível de aninhamento, mas uma mensagem pode estar localizada em um filho de um filho, e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="b152e-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b152e-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b152e-122">Optional query parameters</span></span>
<span data-ttu-id="b152e-123">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b152e-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="b152e-124">Em particular, você pode usar o $expand parâmetro de consulta para incluir todos os anexos de mensagem embutidos com o restante das propriedades de mensagem.</span><span class="sxs-lookup"><span data-stu-id="b152e-124">In particular, you can use the $expand query parameter to include all of the message attachments inline with the rest of the message properties.</span></span> <span data-ttu-id="b152e-125">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="b152e-125">For example:</span></span>

```
GET https://graph.microsoft.com/beta/me/messages/{id}?$expand=attachments
```
## <a name="request-headers"></a><span data-ttu-id="b152e-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b152e-126">Request headers</span></span>
| <span data-ttu-id="b152e-127">Nome</span><span class="sxs-lookup"><span data-stu-id="b152e-127">Name</span></span>       | <span data-ttu-id="b152e-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="b152e-128">Type</span></span> | <span data-ttu-id="b152e-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="b152e-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b152e-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="b152e-130">Authorization</span></span>  | <span data-ttu-id="b152e-131">string</span><span class="sxs-lookup"><span data-stu-id="b152e-131">string</span></span>  | <span data-ttu-id="b152e-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b152e-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b152e-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b152e-134">Request body</span></span>
<span data-ttu-id="b152e-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b152e-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b152e-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="b152e-136">Response</span></span>

<span data-ttu-id="b152e-137">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b152e-137">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b152e-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b152e-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b152e-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b152e-139">Request</span></span>
<span data-ttu-id="b152e-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b152e-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b152e-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="b152e-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_get_attachments_beta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages/{id}/attachments
```
# <a name="c"></a>[<span data-ttu-id="b152e-142">C#</span><span class="sxs-lookup"><span data-stu-id="b152e-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-get-attachments-beta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b152e-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b152e-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-get-attachments-beta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b152e-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b152e-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-get-attachments-beta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b152e-145">Java</span><span class="sxs-lookup"><span data-stu-id="b152e-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-get-attachments-beta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b152e-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="b152e-146">Response</span></span>
<span data-ttu-id="b152e-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b152e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
