---
title: Listar anexos
description: Recupere uma lista de objetos attachment anexados a uma mensagem.
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: b4f86871e31dcaaf9303d0cbd19e7d178137a9a9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867022"
---
# <a name="list-attachments"></a><span data-ttu-id="f0e79-103">Listar anexos</span><span class="sxs-lookup"><span data-stu-id="f0e79-103">List attachments</span></span>

<span data-ttu-id="f0e79-104">Recupere uma lista de objetos [attachment](../resources/attachment.md) anexados a uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="f0e79-104">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a message.</span></span>
## <a name="permissions"></a><span data-ttu-id="f0e79-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f0e79-105">Permissions</span></span>
<span data-ttu-id="f0e79-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0e79-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0e79-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f0e79-108">Permission type</span></span>      | <span data-ttu-id="f0e79-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f0e79-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f0e79-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f0e79-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f0e79-111">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="f0e79-111">Mail.Read</span></span>    |
|<span data-ttu-id="f0e79-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f0e79-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0e79-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="f0e79-113">Mail.Read</span></span>    |
|<span data-ttu-id="f0e79-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f0e79-114">Application</span></span> | <span data-ttu-id="f0e79-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="f0e79-115">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="f0e79-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f0e79-116">HTTP request</span></span>
<span data-ttu-id="f0e79-117"><!-- { "blockType": "ignored" } -->Anexos de uma [mensagem](../resources/message.md) na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="f0e79-117"><!-- { "blockType": "ignored" } --> Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
GET /me/messages/{id}/attachments
GET /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="f0e79-118">Anexos de uma [message](../resources/message.md) contidos em uma [mailFolder](../resources/mailfolder.md) de nível superior na caixa de correio de um usuário.</span><span class="sxs-lookup"><span data-stu-id="f0e79-118">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
GET /me/mailFolders/{id}/messages/{id}/attachments
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="f0e79-p102">Anexos de uma [message](../resources/message.md) contidos em uma pasta filha de uma [mailFolder](../resources/mailfolder.md) na caixa de correio de um usuário.  O exemplo a seguir mostra um nível de aninhamento, mas uma mensagem pode estar localizada em um filho de um filho, e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="f0e79-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f0e79-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f0e79-121">Optional query parameters</span></span>
<span data-ttu-id="f0e79-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f0e79-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f0e79-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f0e79-123">Request headers</span></span>
| <span data-ttu-id="f0e79-124">Nome</span><span class="sxs-lookup"><span data-stu-id="f0e79-124">Name</span></span>       | <span data-ttu-id="f0e79-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0e79-125">Type</span></span> | <span data-ttu-id="f0e79-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0e79-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f0e79-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="f0e79-127">Authorization</span></span>  | <span data-ttu-id="f0e79-128">string</span><span class="sxs-lookup"><span data-stu-id="f0e79-128">string</span></span>  | <span data-ttu-id="f0e79-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f0e79-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f0e79-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f0e79-131">Request body</span></span>
<span data-ttu-id="f0e79-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f0e79-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f0e79-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0e79-133">Response</span></span>

<span data-ttu-id="f0e79-134">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f0e79-134">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f0e79-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f0e79-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f0e79-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f0e79-136">Request</span></span>
<span data-ttu-id="f0e79-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f0e79-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="f0e79-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0e79-138">Response</span></span>
<span data-ttu-id="f0e79-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f0e79-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
