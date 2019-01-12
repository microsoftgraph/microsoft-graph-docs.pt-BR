---
title: Adicionar anexo
description: Use esta API para criar um novo Anexo.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: d2e2de9e8e7e328f2e0cabc1df8fdf7dcd7b4856
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27965912"
---
# <a name="add-attachment"></a><span data-ttu-id="ae8f1-103">Adicionar anexo</span><span class="sxs-lookup"><span data-stu-id="ae8f1-103">Add attachment</span></span>

> <span data-ttu-id="ae8f1-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ae8f1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ae8f1-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ae8f1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ae8f1-106">Use esta API para criar um novo Anexo.</span><span class="sxs-lookup"><span data-stu-id="ae8f1-106">Use this API to create a new Attachment.</span></span>

<span data-ttu-id="ae8f1-107">Um anexo pode ser de um dos seguintes tipos:</span><span class="sxs-lookup"><span data-stu-id="ae8f1-107">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="ae8f1-108">Um arquivo (recurso [fileAttachment](../resources/fileattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="ae8f1-108">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="ae8f1-109">Um item (contato, evento ou mensagem, representado por um recurso [itemAttachment](../resources/itemattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="ae8f1-109">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="ae8f1-110">Um link para um arquivo (recurso [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="ae8f1-110">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="ae8f1-111">Todos esses tipos de recursos de anexo são derivados do recurso [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="ae8f1-111">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="ae8f1-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="ae8f1-112">Permissions</span></span>
<span data-ttu-id="ae8f1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae8f1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae8f1-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ae8f1-115">Permission type</span></span>      | <span data-ttu-id="ae8f1-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ae8f1-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae8f1-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ae8f1-117">Delegated (work or school account)</span></span> | <span data-ttu-id="ae8f1-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ae8f1-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ae8f1-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ae8f1-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae8f1-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ae8f1-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ae8f1-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ae8f1-121">Application</span></span> | <span data-ttu-id="ae8f1-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ae8f1-122">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae8f1-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ae8f1-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/attachments
POST /users/{id|userPrincipalName}/messages/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="ae8f1-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ae8f1-124">Request headers</span></span>
| <span data-ttu-id="ae8f1-125">Nome</span><span class="sxs-lookup"><span data-stu-id="ae8f1-125">Name</span></span>       | <span data-ttu-id="ae8f1-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="ae8f1-126">Type</span></span> | <span data-ttu-id="ae8f1-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae8f1-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ae8f1-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="ae8f1-128">Authorization</span></span>  | <span data-ttu-id="ae8f1-129">string</span><span class="sxs-lookup"><span data-stu-id="ae8f1-129">string</span></span>  | <span data-ttu-id="ae8f1-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ae8f1-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ae8f1-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ae8f1-132">Content-Type</span></span> | <span data-ttu-id="ae8f1-133">string</span><span class="sxs-lookup"><span data-stu-id="ae8f1-133">string</span></span>  | <span data-ttu-id="ae8f1-p104">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ae8f1-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ae8f1-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ae8f1-136">Request body</span></span>
<span data-ttu-id="ae8f1-137">No corpo da solicitação, forneça uma representação JSON do objeto [Attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="ae8f1-137">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ae8f1-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae8f1-138">Response</span></span>

<span data-ttu-id="ae8f1-139">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ae8f1-139">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="ae8f1-140">Exemplo (anexo de arquivo)</span><span class="sxs-lookup"><span data-stu-id="ae8f1-140">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="ae8f1-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ae8f1-141">Request</span></span>
<span data-ttu-id="ae8f1-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ae8f1-142">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="ae8f1-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae8f1-143">Response</span></span>
<span data-ttu-id="ae8f1-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ae8f1-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP 201 Created
```


## <a name="example-item-attachment"></a><span data-ttu-id="ae8f1-147">Exemplo (anexo de item)</span><span class="sxs-lookup"><span data-stu-id="ae8f1-147">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="ae8f1-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ae8f1-148">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="ae8f1-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae8f1-149">Response</span></span>
<span data-ttu-id="ae8f1-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ae8f1-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP 201 Created
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
