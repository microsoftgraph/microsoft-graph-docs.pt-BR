---
title: Criar anexo
description: Use essa API para adicionar um anexo a um outlookTask.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 70e14b9e13656e61a17bb0d3dc7b393dcf36f9b4
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50474742"
---
# <a name="create-attachment-deprecated"></a><span data-ttu-id="b708b-103">Criar anexo (preterido)</span><span class="sxs-lookup"><span data-stu-id="b708b-103">Create attachment (deprecated)</span></span>

<span data-ttu-id="b708b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b708b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="b708b-105">Use essa API para adicionar um [anexo](../resources/attachment.md) a um [outlookTask](../resources/outlooktask.md).</span><span class="sxs-lookup"><span data-stu-id="b708b-105">Use this API to add an [attachment](../resources/attachment.md) to an [outlookTask](../resources/outlooktask.md).</span></span> <span data-ttu-id="b708b-106">O anexo pode ser um arquivo (do [tipo fileAttachment)](../resources/fileattachment.md) ou um item do Outlook ([tipo itemAttachment).](../resources/itemattachment.md)</span><span class="sxs-lookup"><span data-stu-id="b708b-106">The attachment can be a file (of [fileAttachment](../resources/fileattachment.md) type) or Outlook item ([itemAttachment](../resources/itemattachment.md) type).</span></span>

## <a name="permissions"></a><span data-ttu-id="b708b-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="b708b-107">Permissions</span></span>

<span data-ttu-id="b708b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b708b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b708b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b708b-110">Permission type</span></span>      | <span data-ttu-id="b708b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b708b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b708b-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b708b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b708b-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b708b-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="b708b-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b708b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b708b-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b708b-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="b708b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b708b-116">Application</span></span> | <span data-ttu-id="b708b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b708b-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b708b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b708b-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/outlook/tasks/{id}/attachments
POST /users/{id|userPrincipalName}/outlook/tasks/{id}/attachments
```

## <a name="request-headers"></a><span data-ttu-id="b708b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b708b-119">Request headers</span></span>

| <span data-ttu-id="b708b-120">Nome</span><span class="sxs-lookup"><span data-stu-id="b708b-120">Name</span></span>       | <span data-ttu-id="b708b-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="b708b-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b708b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b708b-122">Authorization</span></span>  | <span data-ttu-id="b708b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b708b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b708b-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b708b-125">Content-Type</span></span> | <span data-ttu-id="b708b-126">Uma cadeia de caracteres que representa o tipo de dados no corpo de uma entidade.</span><span class="sxs-lookup"><span data-stu-id="b708b-126">A string that represents the type of data in the body of an entity.</span></span> <span data-ttu-id="b708b-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b708b-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b708b-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b708b-128">Request body</span></span>

<span data-ttu-id="b708b-129">No corpo da solicitação, forneça uma representação JSON do objeto [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="b708b-129">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b708b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="b708b-130">Response</span></span>

<span data-ttu-id="b708b-131">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b708b-131">If successful, this method returns `201 Created` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b708b-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b708b-132">Examples</span></span>

### <a name="example-1-add-file-attachment"></a><span data-ttu-id="b708b-133">Exemplo 1: Adicionar anexo de arquivo</span><span class="sxs-lookup"><span data-stu-id="b708b-133">Example 1: Add file attachment</span></span> 

#### <a name="request"></a><span data-ttu-id="b708b-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b708b-134">Request</span></span>

<span data-ttu-id="b708b-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b708b-135">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b708b-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="b708b-136">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b708b-137">C#</span><span class="sxs-lookup"><span data-stu-id="b708b-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-file-attachment-to-task-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b708b-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b708b-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-file-attachment-to-task-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b708b-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b708b-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-file-attachment-to-task-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b708b-140">Java</span><span class="sxs-lookup"><span data-stu-id="b708b-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-file-attachment-to-task-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b708b-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="b708b-141">Response</span></span>

<span data-ttu-id="b708b-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b708b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

### <a name="example-2-add-item-attachment"></a><span data-ttu-id="b708b-145">Exemplo 2: Adicionar anexo de item</span><span class="sxs-lookup"><span data-stu-id="b708b-145">Example 2: Add item attachment</span></span>

#### <a name="request"></a><span data-ttu-id="b708b-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b708b-146">Request</span></span>

<span data-ttu-id="b708b-147">Eis um exemplo que anexa um evento com outro evento como um anexo de item.</span><span class="sxs-lookup"><span data-stu-id="b708b-147">Here is an example which attaches an event with another event as an item attachment.</span></span>


# <a name="http"></a>[<span data-ttu-id="b708b-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="b708b-148">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b708b-149">C#</span><span class="sxs-lookup"><span data-stu-id="b708b-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-item-attachment-to-task-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b708b-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b708b-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-item-attachment-to-task-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b708b-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b708b-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-item-attachment-to-task-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b708b-152">Java</span><span class="sxs-lookup"><span data-stu-id="b708b-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-item-attachment-to-task-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="b708b-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="b708b-153">Response</span></span>

<span data-ttu-id="b708b-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b708b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


