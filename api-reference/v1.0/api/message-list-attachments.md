---
title: Listar anexos
description: Recupere uma lista de objetos anexados a uma mensagem.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 6da58306f855caea958e07efa6f8000ff1f07b5a
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35275030"
---
# <a name="list-attachments"></a><span data-ttu-id="d014b-103">Listar anexos</span><span class="sxs-lookup"><span data-stu-id="d014b-103">List attachments</span></span>

<span data-ttu-id="d014b-104">Recupere uma lista de objetos [attachment](../resources/attachment.md) anexados a uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="d014b-104">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a message.</span></span>
## <a name="permissions"></a><span data-ttu-id="d014b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d014b-105">Permissions</span></span>
<span data-ttu-id="d014b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d014b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d014b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d014b-108">Permission type</span></span>      | <span data-ttu-id="d014b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d014b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d014b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d014b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d014b-111">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="d014b-111">Mail.Read</span></span>    |
|<span data-ttu-id="d014b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d014b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d014b-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="d014b-113">Mail.Read</span></span>    |
|<span data-ttu-id="d014b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d014b-114">Application</span></span> | <span data-ttu-id="d014b-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="d014b-115">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="d014b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d014b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="d014b-117">Anexos de uma [message](../resources/message.md) em uma caixa de correio de usuário.</span><span class="sxs-lookup"><span data-stu-id="d014b-117">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
GET /me/messages/{id}/attachments
GET /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="d014b-118">Anexos de uma [message](../resources/message.md) contidos em uma [mailFolder](../resources/mailfolder.md) de nível superior na caixa de correio de um usuário.</span><span class="sxs-lookup"><span data-stu-id="d014b-118">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
GET /me/mailFolders/{id}/messages/{id}/attachments
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="d014b-p102">Anexos de uma [message](../resources/message.md) contidos em uma pasta filha de uma [mailFolder](../resources/mailfolder.md) na caixa de correio de um usuário.  O exemplo a seguir mostra um nível de aninhamento, mas uma mensagem pode estar localizada em um filho de um filho, e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="d014b-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d014b-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d014b-121">Optional query parameters</span></span>
<span data-ttu-id="d014b-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d014b-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d014b-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d014b-123">Request headers</span></span>
| <span data-ttu-id="d014b-124">Nome</span><span class="sxs-lookup"><span data-stu-id="d014b-124">Name</span></span>       | <span data-ttu-id="d014b-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="d014b-125">Type</span></span> | <span data-ttu-id="d014b-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="d014b-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d014b-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="d014b-127">Authorization</span></span>  | <span data-ttu-id="d014b-128">string</span><span class="sxs-lookup"><span data-stu-id="d014b-128">string</span></span>  | <span data-ttu-id="d014b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d014b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d014b-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d014b-131">Request body</span></span>
<span data-ttu-id="d014b-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d014b-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d014b-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="d014b-133">Response</span></span>

<span data-ttu-id="d014b-134">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d014b-134">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d014b-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d014b-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d014b-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d014b-136">Request</span></span>
<span data-ttu-id="d014b-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d014b-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="d014b-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="d014b-138">Response</span></span>
<span data-ttu-id="d014b-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d014b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "base64-contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "datetime-value",
      "id": "id-value",
      "isInline": false,
      "name": "name-value",
      "size": 99
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d014b-142">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="d014b-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d014b-143">C#</span><span class="sxs-lookup"><span data-stu-id="d014b-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_attachments-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d014b-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="d014b-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_attachments-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d014b-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d014b-145">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_attachments-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/message-list-attachments.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/message-list-attachments.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/message-list-attachments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
