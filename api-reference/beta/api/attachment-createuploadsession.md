---
title: 'Anexo: createUploadSession'
description: Crie uma sessão de upload para carregar de forma iterativa os intervalos de um arquivo para anexar o arquivo à mensagem especificada.
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: c06699c99a381e46195f9e9bcb4eb772655df349
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895696"
---
# <a name="attachment-createuploadsession"></a><span data-ttu-id="8c0fa-103">Anexo: createUploadSession</span><span class="sxs-lookup"><span data-stu-id="8c0fa-103">attachment: createUploadSession</span></span>

<span data-ttu-id="8c0fa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c0fa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c0fa-105">Criar uma sessão de carregamento que permite que um aplicativo carregue intervalos de um arquivo de forma iterativa, para anexar o arquivo a um item do Outlook.</span><span class="sxs-lookup"><span data-stu-id="8c0fa-105">Create an upload session that allows an app to iteratively upload ranges of a file, so as to attach the file to an Outlook item.</span></span> <span data-ttu-id="8c0fa-106">O item pode ser uma [mensagem](../resources/message.md) ou um [evento](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="8c0fa-106">The item can be a [message](../resources/message.md) or [event](../resources/event.md).</span></span>

<span data-ttu-id="8c0fa-107">Use essa abordagem para anexar um arquivo se o tamanho do arquivo estiver entre 3 MB e 150 MB.</span><span class="sxs-lookup"><span data-stu-id="8c0fa-107">Use this approach to attach a file if the file size is between 3 MB and 150 MB.</span></span> <span data-ttu-id="8c0fa-108">Para anexar um arquivo menor que 3 MB, execute uma `POST` operação na propriedade de navegação **Attachments** do item do Outlook; Veja como fazer isso [para uma mensagem](message-post-attachments.md) ou [para um evento](event-post-attachments.md).</span><span class="sxs-lookup"><span data-stu-id="8c0fa-108">To attach a file that's smaller than 3 MB, do a `POST` operation on the **attachments** navigation property of the Outlook item; see how to do this [for a message](message-post-attachments.md) or [for an event](event-post-attachments.md).</span></span> 

<span data-ttu-id="8c0fa-109">Como parte da resposta, esta ação retorna uma URL de upload que você pode usar em consultas sequenciais subsequentes `PUT` .</span><span class="sxs-lookup"><span data-stu-id="8c0fa-109">As part of the response, this action returns an upload URL that you can use in subsequent sequential `PUT` queries.</span></span> <span data-ttu-id="8c0fa-110">Os cabeçalhos de solicitação para cada `PUT` operação permitem que você especifique o intervalo exato de bytes a serem carregados.</span><span class="sxs-lookup"><span data-stu-id="8c0fa-110">Request headers for each `PUT` operation let you specify the exact range of bytes to be uploaded.</span></span> <span data-ttu-id="8c0fa-111">Isso permite que a transferência seja retomada, caso a conexão de rede seja interrompida durante o carregamento.</span><span class="sxs-lookup"><span data-stu-id="8c0fa-111">This allows transfer to be resumed, in case the network connection is dropped during upload.</span></span> 

<span data-ttu-id="8c0fa-112">A seguir estão as etapas para anexar um arquivo a um item do Outlook usando uma sessão de carregamento:</span><span class="sxs-lookup"><span data-stu-id="8c0fa-112">The following are the steps to attach a file to an Outlook item using an upload session:</span></span>

1. <span data-ttu-id="8c0fa-113">Criar uma sessão de carregamento.</span><span class="sxs-lookup"><span data-stu-id="8c0fa-113">Create an upload session.</span></span>
2. <span data-ttu-id="8c0fa-114">Dentro dessa sessão de upload, carregue de forma iterativa os intervalos de bytes (até 4 MB cada vez) até que todos os bytes do arquivo tenham sido carregados e o arquivo esteja anexado ao item especificado.</span><span class="sxs-lookup"><span data-stu-id="8c0fa-114">Within that upload session, iteratively upload ranges of bytes (up to 4 MB each time) until all the bytes of the file have been uploaded, and the file is attached to the specified item.</span></span>
3. <span data-ttu-id="8c0fa-115">Salve a ID do anexo para acesso futuro.</span><span class="sxs-lookup"><span data-stu-id="8c0fa-115">Save the ID for the attachment for future access.</span></span>
4. <span data-ttu-id="8c0fa-116">Opcional: exclua a sessão de upload.</span><span class="sxs-lookup"><span data-stu-id="8c0fa-116">Optional: Delete the upload session.</span></span>

<span data-ttu-id="8c0fa-117">Consulte [anexar arquivos grandes a mensagens ou eventos do Outlook](/graph/outlook-large-attachments) para obter um exemplo.</span><span class="sxs-lookup"><span data-stu-id="8c0fa-117">See [attach large files to Outlook messages or events](/graph/outlook-large-attachments) for an example.</span></span>

> [!TIP]
> <span data-ttu-id="8c0fa-118">O Exchange Online permite que os administradores personalizem o limite de tamanho de mensagens de caixas de correio do Microsoft 365, incluindo qualquer anexo de mensagem.</span><span class="sxs-lookup"><span data-stu-id="8c0fa-118">Exchange Online lets administrators customize the message size limit for Microsoft 365 mailboxes,  including any message attachments.</span></span> <span data-ttu-id="8c0fa-119">Por padrão, esse limite de tamanho de mensagem é de 35 MB.</span><span class="sxs-lookup"><span data-stu-id="8c0fa-119">By default, this message size limit is 35 MB.</span></span> <span data-ttu-id="8c0fa-120">Descubra como [Personalizar o tamanho máximo da mensagem](https://www.microsoft.com/microsoft-365/blog/2015/04/15/office-365-now-supports-larger-email-messages-up-to-150-mb) para dar suporte a anexos maiores que o limite padrão para o seu locatário.</span><span class="sxs-lookup"><span data-stu-id="8c0fa-120">Find out how to [customize the maximum message size](https://www.microsoft.com/microsoft-365/blog/2015/04/15/office-365-now-supports-larger-email-messages-up-to-150-mb) to support attachments larger than the default limit for your tenant.</span></span> 

> [!IMPORTANT] 
> <span data-ttu-id="8c0fa-121">Esteja ciente de um [problema conhecido](/graph/known-issues#attaching-large-files-to-messages) se estiver anexando um arquivo grande a uma mensagem ou evento em uma caixa de correio compartilhada ou delegada.</span><span class="sxs-lookup"><span data-stu-id="8c0fa-121">Be aware of a [known issue](/graph/known-issues#attaching-large-files-to-messages) if you're attaching a large file to a message or event in a shared or delegated mailbox.</span></span>


## <a name="permissions"></a><span data-ttu-id="8c0fa-122">Permissões</span><span class="sxs-lookup"><span data-stu-id="8c0fa-122">Permissions</span></span>

<span data-ttu-id="8c0fa-123">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="8c0fa-123">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="8c0fa-124">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c0fa-124">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8c0fa-125">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8c0fa-125">Permission type</span></span>                        | <span data-ttu-id="8c0fa-126">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8c0fa-126">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8c0fa-127">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8c0fa-127">Delegated (work or school account)</span></span>     | <span data-ttu-id="8c0fa-128">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c0fa-128">Mail.ReadWrite</span></span> |
| <span data-ttu-id="8c0fa-129">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8c0fa-129">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c0fa-130">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c0fa-130">Mail.ReadWrite</span></span> |
| <span data-ttu-id="8c0fa-131">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8c0fa-131">Application</span></span>                            | <span data-ttu-id="8c0fa-132">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c0fa-132">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c0fa-133">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8c0fa-133">HTTP request</span></span>

<span data-ttu-id="8c0fa-134">Para criar uma sessão de carregamento para anexar um arquivo a um **evento**:</span><span class="sxs-lookup"><span data-stu-id="8c0fa-134">To create an upload session for attaching a file to an **event**:</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/attachments/createUploadSession
```

<span data-ttu-id="8c0fa-135">Para criar uma sessão de carregamento para anexar um arquivo a uma **mensagem**:</span><span class="sxs-lookup"><span data-stu-id="8c0fa-135">To create an upload session for attaching a file to a **message**:</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/attachments/createUploadSession
```

## <a name="request-headers"></a><span data-ttu-id="8c0fa-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8c0fa-136">Request headers</span></span>

| <span data-ttu-id="8c0fa-137">Nome</span><span class="sxs-lookup"><span data-stu-id="8c0fa-137">Name</span></span>          | <span data-ttu-id="8c0fa-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c0fa-138">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8c0fa-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="8c0fa-139">Authorization</span></span> | <span data-ttu-id="8c0fa-140">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="8c0fa-140">Bearer {token}</span></span> |


## <a name="request-body"></a><span data-ttu-id="8c0fa-141">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8c0fa-141">Request body</span></span>

<span data-ttu-id="8c0fa-142">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8c0fa-142">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8c0fa-143">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8c0fa-143">Parameter</span></span>    | <span data-ttu-id="8c0fa-144">Tipo</span><span class="sxs-lookup"><span data-stu-id="8c0fa-144">Type</span></span>        | <span data-ttu-id="8c0fa-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c0fa-145">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8c0fa-146">AttachmentItem</span><span class="sxs-lookup"><span data-stu-id="8c0fa-146">AttachmentItem</span></span>|[<span data-ttu-id="8c0fa-147">attachmentItem</span><span class="sxs-lookup"><span data-stu-id="8c0fa-147">attachmentItem</span></span>](../resources/attachmentitem.md)|<span data-ttu-id="8c0fa-148">Representa os atributos do item a ser carregado e anexado.</span><span class="sxs-lookup"><span data-stu-id="8c0fa-148">Represents attributes of the item to be uploaded and attached.</span></span> <span data-ttu-id="8c0fa-149">Especifique, no mínimo, o tipo de anexo ( `file` ), um nome e o tamanho do arquivo.</span><span class="sxs-lookup"><span data-stu-id="8c0fa-149">At minimum, specify the attachment type (`file`), a name, and the size of the file.</span></span>|

## <a name="response"></a><span data-ttu-id="8c0fa-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c0fa-150">Response</span></span>

<span data-ttu-id="8c0fa-151">Se tiver êxito, este método retornará um `201 Created` código de resposta e um novo objeto [uploadSession](../resources/uploadsession.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8c0fa-151">If successful, this method returns a `201 Created` response code and a new [uploadSession](../resources/uploadsession.md) object in the response body.</span></span>

><span data-ttu-id="8c0fa-152">**Observação**:</span><span class="sxs-lookup"><span data-stu-id="8c0fa-152">**Note**:</span></span> 
>
><span data-ttu-id="8c0fa-153">A propriedade **uploadUrl** retornada como parte do objeto de resposta **UPLOADSESSION** é uma URL opaca para consultas subsequentes `PUT` para carregar intervalos de bytes do arquivo.</span><span class="sxs-lookup"><span data-stu-id="8c0fa-153">The **uploadUrl** property returned as part of the **uploadSession** response object is an opaque URL for subsequent `PUT` queries to upload byte ranges of the file.</span></span> <span data-ttu-id="8c0fa-154">Ele contém o token de autenticação apropriado para `PUT` consultas subsequentes que expiram pelo **expirationDateTime**.</span><span class="sxs-lookup"><span data-stu-id="8c0fa-154">It contains the appropriate auth token for subsequent `PUT` queries that expire by **expirationDateTime**.</span></span> <span data-ttu-id="8c0fa-155">Não Personalize esta URL.</span><span class="sxs-lookup"><span data-stu-id="8c0fa-155">Do not customize this URL.</span></span>
>
><span data-ttu-id="8c0fa-156">A propriedade **nextExpectedRanges** especifica o próximo local de byte de arquivo para carregar, por exemplo, `"NextExpectedRanges":["2097152"]` .</span><span class="sxs-lookup"><span data-stu-id="8c0fa-156">The **nextExpectedRanges** property specifies the next file byte location to upload from, for example, `"NextExpectedRanges":["2097152"]`.</span></span> <span data-ttu-id="8c0fa-157">Você deve carregar os bytes em um arquivo na ordem.</span><span class="sxs-lookup"><span data-stu-id="8c0fa-157">You must upload bytes in a file in order.</span></span>

<!-- The **nextExpectedRanges** property specifies one or more ranges of bytes that the server is still missing for the file. These ranges are zero-indexed and of the format `{start}-{end}`, unless if the server misses the remainder of the bytes from the start of that range, in which case the format is simply `{start}`.  -->


## <a name="examples"></a><span data-ttu-id="8c0fa-158">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8c0fa-158">Examples</span></span>

<span data-ttu-id="8c0fa-159">O exemplo a seguir mostra como criar uma sessão de carregamento que você pode usar em operações de upload de arquivo subsequentes para a mensagem especificada.</span><span class="sxs-lookup"><span data-stu-id="8c0fa-159">The following example shows how to create an upload session that you can use in subsequent file upload operations to the specified message.</span></span>

### <a name="request"></a><span data-ttu-id="8c0fa-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8c0fa-160">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8c0fa-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="8c0fa-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "attachment_createuploadsession",
  "sampleKeys": ["AAMkADI5MAAIT3drCAAA="]
}-->

```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADI5MAAIT3drCAAA=/attachments/createUploadSession
Content-type: application/json

{
  "AttachmentItem": {
    "attachmentType": "file",
    "name": "flower", 
    "size": 3483322
  }
}
```
# <a name="c"></a>[<span data-ttu-id="8c0fa-162">C#</span><span class="sxs-lookup"><span data-stu-id="8c0fa-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/attachment-createuploadsession-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8c0fa-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8c0fa-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/attachment-createuploadsession-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8c0fa-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8c0fa-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/attachment-createuploadsession-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8c0fa-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c0fa-165">Response</span></span>

> <span data-ttu-id="8c0fa-166">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="8c0fa-166">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="8c0fa-167">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="8c0fa-167">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "attachment_createuploadsession",
  "truncated": true,
  "@odata.type": "microsoft.graph.uploadSession"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.uploadSession",
    "uploadUrl": "https://outlook.office.com/api/beta/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/AttachmentSessions('AAMkADI5MAAIT3k0uAAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIUlN6bllHMmNI",
    "expirationDateTime": "2019-09-25T01:09:30.7671707Z",
    "nextExpectedRanges": [
        "0-"
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attachment: createUploadSession",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
