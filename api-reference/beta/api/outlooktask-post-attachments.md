---
title: Criar anexo
description: Use esta API para adicionar um anexo a um outlookTask.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: c4f9386e680bb344055c62063232d5a8603fe42f
ms.sourcegitcommit: 66c8fcafee151278f8089cd26d0c5766d33d04a8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/09/2020
ms.locfileid: "40994705"
---
# <a name="create-attachment"></a><span data-ttu-id="c9765-103">Criar anexo</span><span class="sxs-lookup"><span data-stu-id="c9765-103">Create attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9765-104">Use esta API para adicionar um [anexo](../resources/attachment.md) a um [outlookTask](../resources/outlooktask.md).</span><span class="sxs-lookup"><span data-stu-id="c9765-104">Use this API to add an [attachment](../resources/attachment.md) to an [outlookTask](../resources/outlooktask.md).</span></span> <span data-ttu-id="c9765-105">O anexo pode ser um arquivo (de tipo [Fileattachment](../resources/fileattachment.md) ) ou um item do Outlook (tipo de[anexo](../resources/itemattachment.md) ).</span><span class="sxs-lookup"><span data-stu-id="c9765-105">The attachment can be a file (of [fileAttachment](../resources/fileattachment.md) type) or Outlook item ([itemAttachment](../resources/itemattachment.md) type).</span></span>

## <a name="permissions"></a><span data-ttu-id="c9765-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c9765-106">Permissions</span></span>

<span data-ttu-id="c9765-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9765-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9765-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c9765-109">Permission type</span></span>      | <span data-ttu-id="c9765-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c9765-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c9765-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c9765-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c9765-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c9765-112">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="c9765-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c9765-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9765-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c9765-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="c9765-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c9765-115">Application</span></span> | <span data-ttu-id="c9765-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c9765-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c9765-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c9765-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/outlook/tasks/{id}/attachments
POST /users/{id|userPrincipalName}/outlook/tasks/{id}/attachments
```

## <a name="request-headers"></a><span data-ttu-id="c9765-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c9765-118">Request headers</span></span>

| <span data-ttu-id="c9765-119">Nome</span><span class="sxs-lookup"><span data-stu-id="c9765-119">Name</span></span>       | <span data-ttu-id="c9765-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9765-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c9765-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c9765-121">Authorization</span></span>  | <span data-ttu-id="c9765-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c9765-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c9765-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c9765-124">Content-Type</span></span> | <span data-ttu-id="c9765-125">Uma cadeia de caracteres que representa o tipo de dados no corpo de uma entidade.</span><span class="sxs-lookup"><span data-stu-id="c9765-125">A string that represents the type of data in the body of an entity.</span></span> <span data-ttu-id="c9765-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c9765-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c9765-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c9765-127">Request body</span></span>

<span data-ttu-id="c9765-128">No corpo da solicitação, forneça uma representação JSON do objeto [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="c9765-128">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c9765-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9765-129">Response</span></span>

<span data-ttu-id="c9765-130">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c9765-130">If successful, this method returns `201 Created` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c9765-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c9765-131">Examples</span></span>

### <a name="example-1-add-file-attachment"></a><span data-ttu-id="c9765-132">Exemplo 1: Adicionar anexo de arquivo</span><span class="sxs-lookup"><span data-stu-id="c9765-132">Example 1: Add file attachment</span></span> 

#### <a name="request"></a><span data-ttu-id="c9765-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c9765-133">Request</span></span>

<span data-ttu-id="c9765-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c9765-134">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "add_file_attachment_to_task"
}-->

```http
POST https://graph.microsoft.com/beta/me/outlook/tasks/AAMkADAAAANXbdnAAA=/attachments
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.fileAttachment",
    "name": "menu.txt",
    "contentBytes": "bWFjIGFuZCBjaGVlc2UgdG9kYXk="
}
```

#### <a name="response"></a><span data-ttu-id="c9765-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9765-135">Response</span></span>

<span data-ttu-id="c9765-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c9765-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "add_file_attachment_to_task",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAttachment"
} -->

```http
HTTP 201 Created

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/outlook/tasks('AAMkADAAAANXbdnAAA%3D')/attachments/$entity",
    "@odata.type": "#microsoft.graph.fileAttachment",
    "@odata.mediaContentType": "text/plain",
    "id": "AAMkADAAAANXbdnAAABEgAQAKQF4_X0QwVHpmAmxUgHN_Q=",
    "lastModifiedDateTime": "2020-01-07T22:13:30Z",
    "name": "menu.txt",
    "contentType": "text/plain",
    "size": 178,
    "isInline": false,
    "contentId": null,
    "contentLocation": null,
    "contentBytes": "bWFjIGFuZCBjaGVlc2UgdG9kYXk="
}
```

### <a name="example-2-add-item-attachment"></a><span data-ttu-id="c9765-139">Exemplo 2: Adicionar anexo de item</span><span class="sxs-lookup"><span data-stu-id="c9765-139">Example 2: Add item attachment</span></span>

#### <a name="request"></a><span data-ttu-id="c9765-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c9765-140">Request</span></span>

<span data-ttu-id="c9765-141">Eis um exemplo que anexa um evento com outro evento como um anexo de item.</span><span class="sxs-lookup"><span data-stu-id="c9765-141">Here is an example which attaches an event with another event as an item attachment.</span></span>

<!-- {
  "blockType": "request",
  "name": "add_item_attachment_to_task"
}-->

```http
POST https://graph.microsoft.com/beta/me/outlook/tasks/AAMkADAAAANXbdnAAA=/attachments
Content-type: application/json

{
  "@odata.type": "#microsoft.graph.itemAttachment",
  "name": "Holiday event",
  "item": {
        "@odata.type": "microsoft.graph.event",
        "subject": "Discuss gifts for children",
        "body": {
            "contentType": "HTML",
            "content": "Let's look for funding!"
         },
         "start": {
             "dateTime": "2020-01-12T18:00:00",
             "timeZone": "Pacific Standard Time"
          },
          "end": {
             "dateTime": "2020-01-12T19:00:00",
             "timeZone": "Pacific Standard Time"
          }
    }
}
```


#### <a name="response"></a><span data-ttu-id="c9765-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9765-142">Response</span></span>

<span data-ttu-id="c9765-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c9765-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "add_item_attachment_to_task",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemAttachment"
} -->

```http
HTTP 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/outlook/tasks('AAMkADAAAANXbdnAAA%3D')/attachments/$entity",
    "@odata.type": "#microsoft.graph.itemAttachment",
    "id": "AAMkADAAAANXbdnAAABEgAQANgBvaZHiKVMskpdj1k9KEQ=",
    "lastModifiedDateTime": "2020-01-07T22:18:11Z",
    "name": "Holiday event",
    "contentType": null,
    "size": 2067,
    "isInline": false
}
```



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
