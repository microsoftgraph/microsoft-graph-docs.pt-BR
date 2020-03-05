---
title: Criar anexo
description: Use esta API para adicionar um anexo a um outlookTask.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 9d81c0c9b3c59e41c1df42f2af446a61d7bb1a34
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456177"
---
# <a name="create-attachment"></a><span data-ttu-id="663a7-103">Criar anexo</span><span class="sxs-lookup"><span data-stu-id="663a7-103">Create attachment</span></span>

<span data-ttu-id="663a7-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="663a7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="663a7-105">Use esta API para adicionar um [anexo](../resources/attachment.md) a um [outlookTask](../resources/outlooktask.md).</span><span class="sxs-lookup"><span data-stu-id="663a7-105">Use this API to add an [attachment](../resources/attachment.md) to an [outlookTask](../resources/outlooktask.md).</span></span> <span data-ttu-id="663a7-106">O anexo pode ser um arquivo (de tipo [Fileattachment](../resources/fileattachment.md) ) ou um item do Outlook (tipo de[anexo](../resources/itemattachment.md) ).</span><span class="sxs-lookup"><span data-stu-id="663a7-106">The attachment can be a file (of [fileAttachment](../resources/fileattachment.md) type) or Outlook item ([itemAttachment](../resources/itemattachment.md) type).</span></span>

## <a name="permissions"></a><span data-ttu-id="663a7-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="663a7-107">Permissions</span></span>

<span data-ttu-id="663a7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="663a7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="663a7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="663a7-110">Permission type</span></span>      | <span data-ttu-id="663a7-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="663a7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="663a7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="663a7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="663a7-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="663a7-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="663a7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="663a7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="663a7-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="663a7-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="663a7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="663a7-116">Application</span></span> | <span data-ttu-id="663a7-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="663a7-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="663a7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="663a7-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/outlook/tasks/{id}/attachments
POST /users/{id|userPrincipalName}/outlook/tasks/{id}/attachments
```

## <a name="request-headers"></a><span data-ttu-id="663a7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="663a7-119">Request headers</span></span>

| <span data-ttu-id="663a7-120">Nome</span><span class="sxs-lookup"><span data-stu-id="663a7-120">Name</span></span>       | <span data-ttu-id="663a7-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="663a7-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="663a7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="663a7-122">Authorization</span></span>  | <span data-ttu-id="663a7-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="663a7-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="663a7-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="663a7-125">Content-Type</span></span> | <span data-ttu-id="663a7-126">Uma cadeia de caracteres que representa o tipo de dados no corpo de uma entidade.</span><span class="sxs-lookup"><span data-stu-id="663a7-126">A string that represents the type of data in the body of an entity.</span></span> <span data-ttu-id="663a7-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="663a7-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="663a7-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="663a7-128">Request body</span></span>

<span data-ttu-id="663a7-129">No corpo da solicitação, forneça uma representação JSON do objeto [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="663a7-129">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="663a7-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="663a7-130">Response</span></span>

<span data-ttu-id="663a7-131">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="663a7-131">If successful, this method returns `201 Created` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="663a7-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="663a7-132">Examples</span></span>

### <a name="example-1-add-file-attachment"></a><span data-ttu-id="663a7-133">Exemplo 1: Adicionar anexo de arquivo</span><span class="sxs-lookup"><span data-stu-id="663a7-133">Example 1: Add file attachment</span></span> 

#### <a name="request"></a><span data-ttu-id="663a7-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="663a7-134">Request</span></span>

<span data-ttu-id="663a7-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="663a7-135">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="663a7-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="663a7-136">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="663a7-137">C#</span><span class="sxs-lookup"><span data-stu-id="663a7-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-file-attachment-to-task-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="663a7-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="663a7-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-file-attachment-to-task-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="663a7-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="663a7-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-file-attachment-to-task-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="663a7-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="663a7-140">Response</span></span>

<span data-ttu-id="663a7-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="663a7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

### <a name="example-2-add-item-attachment"></a><span data-ttu-id="663a7-144">Exemplo 2: Adicionar anexo de item</span><span class="sxs-lookup"><span data-stu-id="663a7-144">Example 2: Add item attachment</span></span>

#### <a name="request"></a><span data-ttu-id="663a7-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="663a7-145">Request</span></span>

<span data-ttu-id="663a7-146">Eis um exemplo que anexa um evento com outro evento como um anexo de item.</span><span class="sxs-lookup"><span data-stu-id="663a7-146">Here is an example which attaches an event with another event as an item attachment.</span></span>

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


#### <a name="response"></a><span data-ttu-id="663a7-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="663a7-147">Response</span></span>

<span data-ttu-id="663a7-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="663a7-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
