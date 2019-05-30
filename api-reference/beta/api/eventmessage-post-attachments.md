---
title: Adicionar anexo
description: Use esta API para criar um novo Anexo.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 0540769e0cda600eecdf14016adc4de3a27f7400
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536270"
---
# <a name="add-attachment"></a><span data-ttu-id="3bc50-103">Adicionar anexo</span><span class="sxs-lookup"><span data-stu-id="3bc50-103">Add attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3bc50-104">Use esta API para criar um novo Anexo.</span><span class="sxs-lookup"><span data-stu-id="3bc50-104">Use this API to create a new Attachment.</span></span>

<span data-ttu-id="3bc50-105">Um anexo pode ser de um dos seguintes tipos:</span><span class="sxs-lookup"><span data-stu-id="3bc50-105">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="3bc50-106">Um arquivo (recurso [fileAttachment](../resources/fileattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="3bc50-106">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="3bc50-107">Um item (contato, evento ou mensagem, representado por um recurso [itemAttachment](../resources/itemattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="3bc50-107">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="3bc50-108">Um link para um arquivo (recurso [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="3bc50-108">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="3bc50-109">Todos esses tipos de recursos de anexo são derivados do recurso [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="3bc50-109">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="3bc50-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="3bc50-110">Permissions</span></span>
<span data-ttu-id="3bc50-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3bc50-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3bc50-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3bc50-113">Permission type</span></span>      | <span data-ttu-id="3bc50-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3bc50-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3bc50-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3bc50-115">Delegated (work or school account)</span></span> | <span data-ttu-id="3bc50-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3bc50-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="3bc50-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3bc50-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3bc50-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3bc50-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="3bc50-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3bc50-119">Application</span></span> | <span data-ttu-id="3bc50-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3bc50-120">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3bc50-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3bc50-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/attachments
POST /users/{id|userPrincipalName}/messages/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="3bc50-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3bc50-122">Request headers</span></span>
| <span data-ttu-id="3bc50-123">Nome</span><span class="sxs-lookup"><span data-stu-id="3bc50-123">Name</span></span>       | <span data-ttu-id="3bc50-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="3bc50-124">Type</span></span> | <span data-ttu-id="3bc50-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="3bc50-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3bc50-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="3bc50-126">Authorization</span></span>  | <span data-ttu-id="3bc50-127">string</span><span class="sxs-lookup"><span data-stu-id="3bc50-127">string</span></span>  | <span data-ttu-id="3bc50-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3bc50-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3bc50-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3bc50-130">Content-Type</span></span> | <span data-ttu-id="3bc50-131">string</span><span class="sxs-lookup"><span data-stu-id="3bc50-131">string</span></span>  | <span data-ttu-id="3bc50-p103">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3bc50-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3bc50-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3bc50-134">Request body</span></span>
<span data-ttu-id="3bc50-135">No corpo da solicitação, forneça uma representação JSON do objeto [Attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="3bc50-135">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3bc50-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="3bc50-136">Response</span></span>

<span data-ttu-id="3bc50-137">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3bc50-137">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="3bc50-138">Exemplo (anexo de arquivo)</span><span class="sxs-lookup"><span data-stu-id="3bc50-138">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="3bc50-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3bc50-139">Request</span></span>
<span data-ttu-id="3bc50-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3bc50-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_eventmessage"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/{id}/attachments
Content-type: application/json

{
  "@odata.type": "#Microsoft.OutlookServices.FileAttachment",
  "name": "name-value",
  "contentType": "contentType-value",
  "isInline": false,
  "contentLocation": "contentLocation-value",
  "contentBytes": "contentBytes-value"
}
```

##### <a name="response"></a><span data-ttu-id="3bc50-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="3bc50-141">Response</span></span>
<span data-ttu-id="3bc50-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3bc50-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP 201 Created
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="3bc50-145">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="3bc50-145">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3bc50-146">C#</span><span class="sxs-lookup"><span data-stu-id="3bc50-146">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_file_attachment_from_eventmessage-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3bc50-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="3bc50-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_file_attachment_from_eventmessage-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


## <a name="example-item-attachment"></a><span data-ttu-id="3bc50-148">Exemplo (anexo de item)</span><span class="sxs-lookup"><span data-stu-id="3bc50-148">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="3bc50-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3bc50-149">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_eventmessage"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/attachments
Content-type: application/json

{
  "@odata.type": "#Microsoft.OutlookServices.ItemAttachment",
  "name": "name-value",
  "item": "message or event entity"
}
```

##### <a name="response"></a><span data-ttu-id="3bc50-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="3bc50-150">Response</span></span>
<span data-ttu-id="3bc50-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3bc50-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP 201 Created
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="3bc50-154">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="3bc50-154">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3bc50-155">C#</span><span class="sxs-lookup"><span data-stu-id="3bc50-155">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_item_attachment_from_eventmessage-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3bc50-156">Javascript</span><span class="sxs-lookup"><span data-stu-id="3bc50-156">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_item_attachment_from_eventmessage-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/eventmessage-post-attachments.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/eventmessage-post-attachments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
