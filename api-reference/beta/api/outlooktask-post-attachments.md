---
title: Criar anexo
description: Use esta API para adicionar um anexo a um outlookTask.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: ce0be79110f1718e320ddbfb237f2a8a58b40cb7
ms.sourcegitcommit: 5f643d3b3f71a9711963c8953da2188539fc9b0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/14/2020
ms.locfileid: "41119700"
---
# <a name="create-attachment"></a><span data-ttu-id="f784c-103">Criar anexo</span><span class="sxs-lookup"><span data-stu-id="f784c-103">Create attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f784c-104">Use esta API para adicionar um [anexo](../resources/attachment.md) a um [outlookTask](../resources/outlooktask.md).</span><span class="sxs-lookup"><span data-stu-id="f784c-104">Use this API to add an [attachment](../resources/attachment.md) to an [outlookTask](../resources/outlooktask.md).</span></span> <span data-ttu-id="f784c-105">O anexo pode ser um arquivo (de tipo [Fileattachment](../resources/fileattachment.md) ) ou um item do Outlook (tipo de[anexo](../resources/itemattachment.md) ).</span><span class="sxs-lookup"><span data-stu-id="f784c-105">The attachment can be a file (of [fileAttachment](../resources/fileattachment.md) type) or Outlook item ([itemAttachment](../resources/itemattachment.md) type).</span></span>

## <a name="permissions"></a><span data-ttu-id="f784c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f784c-106">Permissions</span></span>

<span data-ttu-id="f784c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f784c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f784c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f784c-109">Permission type</span></span>      | <span data-ttu-id="f784c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f784c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f784c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f784c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f784c-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f784c-112">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="f784c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f784c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f784c-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f784c-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="f784c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f784c-115">Application</span></span> | <span data-ttu-id="f784c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f784c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f784c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f784c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/outlook/tasks/{id}/attachments
POST /users/{id|userPrincipalName}/outlook/tasks/{id}/attachments
```

## <a name="request-headers"></a><span data-ttu-id="f784c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f784c-118">Request headers</span></span>

| <span data-ttu-id="f784c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="f784c-119">Name</span></span>       | <span data-ttu-id="f784c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f784c-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f784c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f784c-121">Authorization</span></span>  | <span data-ttu-id="f784c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f784c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f784c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f784c-124">Content-Type</span></span> | <span data-ttu-id="f784c-125">Uma cadeia de caracteres que representa o tipo de dados no corpo de uma entidade.</span><span class="sxs-lookup"><span data-stu-id="f784c-125">A string that represents the type of data in the body of an entity.</span></span> <span data-ttu-id="f784c-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f784c-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f784c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f784c-127">Request body</span></span>

<span data-ttu-id="f784c-128">No corpo da solicitação, forneça uma representação JSON do objeto [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="f784c-128">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f784c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f784c-129">Response</span></span>

<span data-ttu-id="f784c-130">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f784c-130">If successful, this method returns `201 Created` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f784c-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f784c-131">Examples</span></span>

### <a name="example-1-add-file-attachment"></a><span data-ttu-id="f784c-132">Exemplo 1: Adicionar anexo de arquivo</span><span class="sxs-lookup"><span data-stu-id="f784c-132">Example 1: Add file attachment</span></span> 

#### <a name="request"></a><span data-ttu-id="f784c-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f784c-133">Request</span></span>

<span data-ttu-id="f784c-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f784c-134">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f784c-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="f784c-135">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="f784c-136">C#</span><span class="sxs-lookup"><span data-stu-id="f784c-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-file-attachment-to-task-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f784c-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f784c-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-file-attachment-to-task-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f784c-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f784c-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-file-attachment-to-task-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f784c-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="f784c-139">Response</span></span>

<span data-ttu-id="f784c-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f784c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

### <a name="example-2-add-item-attachment"></a><span data-ttu-id="f784c-143">Exemplo 2: Adicionar anexo de item</span><span class="sxs-lookup"><span data-stu-id="f784c-143">Example 2: Add item attachment</span></span>

#### <a name="request"></a><span data-ttu-id="f784c-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f784c-144">Request</span></span>

<span data-ttu-id="f784c-145">Eis um exemplo que anexa um evento com outro evento como um anexo de item.</span><span class="sxs-lookup"><span data-stu-id="f784c-145">Here is an example which attaches an event with another event as an item attachment.</span></span>

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


#### <a name="response"></a><span data-ttu-id="f784c-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="f784c-146">Response</span></span>

<span data-ttu-id="f784c-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f784c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
