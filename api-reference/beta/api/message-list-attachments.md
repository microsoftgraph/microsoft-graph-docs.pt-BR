---
title: Listar anexos
description: Recupere uma lista de objetos attachment anexados a uma mensagem.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 584b01114f22466673568d991c824a94c6d73dd2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983478"
---
# <a name="list-attachments"></a><span data-ttu-id="bd9df-103">Listar anexos</span><span class="sxs-lookup"><span data-stu-id="bd9df-103">List attachments</span></span>

> <span data-ttu-id="bd9df-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bd9df-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bd9df-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bd9df-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bd9df-106">Recupere uma lista de objetos [attachment](../resources/attachment.md) anexados a uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="bd9df-106">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a message.</span></span>
## <a name="permissions"></a><span data-ttu-id="bd9df-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="bd9df-107">Permissions</span></span>
<span data-ttu-id="bd9df-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd9df-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd9df-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bd9df-110">Permission type</span></span>      | <span data-ttu-id="bd9df-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bd9df-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bd9df-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bd9df-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bd9df-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="bd9df-113">Mail.Read</span></span>    |
|<span data-ttu-id="bd9df-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bd9df-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd9df-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="bd9df-115">Mail.Read</span></span>    |
|<span data-ttu-id="bd9df-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bd9df-116">Application</span></span> | <span data-ttu-id="bd9df-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="bd9df-117">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="bd9df-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bd9df-118">HTTP request</span></span>
<span data-ttu-id="bd9df-119"><!-- { "blockType": "ignored" } -->Anexos de uma [mensagem](../resources/message.md) na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="bd9df-119"><!-- { "blockType": "ignored" } --> Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
GET /me/messages/{id}/attachments
GET /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="bd9df-120">Anexos de uma [message](../resources/message.md) contidos em uma [mailFolder](../resources/mailfolder.md) de nível superior na caixa de correio de um usuário.</span><span class="sxs-lookup"><span data-stu-id="bd9df-120">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
GET /me/mailFolders/{id}/messages/{id}/attachments
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="bd9df-p103">Anexos de uma [message](../resources/message.md) contidos em uma pasta filha de uma [mailFolder](../resources/mailfolder.md) na caixa de correio de um usuário.  O exemplo a seguir mostra um nível de aninhamento, mas uma mensagem pode estar localizada em um filho de um filho, e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="bd9df-p103">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bd9df-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bd9df-123">Optional query parameters</span></span>
<span data-ttu-id="bd9df-124">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="bd9df-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="bd9df-125">Em particular, você pode usar o $expandir o parâmetro de consulta para incluir todos os anexos de mensagem em linha com o restante das propriedades de mensagem.</span><span class="sxs-lookup"><span data-stu-id="bd9df-125">In particular, you can use the $expand query parameter to include all of the message attachments inline with the rest of the message properties.</span></span> <span data-ttu-id="bd9df-126">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="bd9df-126">For example:</span></span>

```
GET https://graph.microsoft.com/beta/me/messages/{id}?$expand=attachments
```
## <a name="request-headers"></a><span data-ttu-id="bd9df-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bd9df-127">Request headers</span></span>
| <span data-ttu-id="bd9df-128">Nome</span><span class="sxs-lookup"><span data-stu-id="bd9df-128">Name</span></span>       | <span data-ttu-id="bd9df-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="bd9df-129">Type</span></span> | <span data-ttu-id="bd9df-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="bd9df-130">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="bd9df-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="bd9df-131">Authorization</span></span>  | <span data-ttu-id="bd9df-132">string</span><span class="sxs-lookup"><span data-stu-id="bd9df-132">string</span></span>  | <span data-ttu-id="bd9df-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bd9df-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bd9df-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bd9df-135">Request body</span></span>
<span data-ttu-id="bd9df-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bd9df-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd9df-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd9df-137">Response</span></span>

<span data-ttu-id="bd9df-138">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bd9df-138">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bd9df-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bd9df-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bd9df-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bd9df-140">Request</span></span>
<span data-ttu-id="bd9df-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bd9df-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="bd9df-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd9df-142">Response</span></span>
<span data-ttu-id="bd9df-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bd9df-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
