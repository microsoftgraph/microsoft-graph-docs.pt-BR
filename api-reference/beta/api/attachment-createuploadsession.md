---
title: 'Anexo: createUploadSession'
description: Crie uma sessão de upload para carregar de forma iterativa os intervalos de um arquivo para anexar o arquivo à mensagem especificada.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 116efc7583b0344cc1845f698210f760e3843d9b
ms.sourcegitcommit: b1e1f614299f668453916bd85761ef7b6c8d6eff
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37968913"
---
# <a name="attachment-createuploadsession"></a><span data-ttu-id="8e72c-103">Anexo: createUploadSession</span><span class="sxs-lookup"><span data-stu-id="8e72c-103">attachment: createUploadSession</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e72c-104">Criar uma sessão de carregamento que permite que um aplicativo carregue intervalos de um arquivo de forma iterativa, para anexar o arquivo à [mensagem](../resources/message.md)especificada.</span><span class="sxs-lookup"><span data-stu-id="8e72c-104">Create an upload session that allows an app to iteratively upload ranges of a file, so as to attach the file to the specified [message](../resources/message.md).</span></span>

<span data-ttu-id="8e72c-105">Use essa abordagem para anexar arquivos de tamanhos entre 3 MB e 150 MB a uma **mensagem**.</span><span class="sxs-lookup"><span data-stu-id="8e72c-105">Use this approach to attach files of sizes between 3 MB and 150 MB to a **message**.</span></span> <span data-ttu-id="8e72c-106">Para anexar arquivos de tamanhos abaixo de 4 MB, basta [postar na propriedade de navegação Attachments](message-post-attachments.md).</span><span class="sxs-lookup"><span data-stu-id="8e72c-106">To attach files of sizes under 4 MB, simply [POST on the attachments navigation property](message-post-attachments.md).</span></span> 

<span data-ttu-id="8e72c-107">Como parte da resposta, esta ação retorna uma URL de upload que você pode usar em consultas sequenciais `PUT` subsequentes.</span><span class="sxs-lookup"><span data-stu-id="8e72c-107">As part of the response, this action returns an upload URL that you can use in subsequent sequential `PUT` queries.</span></span> <span data-ttu-id="8e72c-108">Os cabeçalhos de solicitação `PUT` para cada operação permitem que você especifique o intervalo exato de bytes a serem carregados.</span><span class="sxs-lookup"><span data-stu-id="8e72c-108">Request headers for each `PUT` operation let you specify the exact range of bytes to be uploaded.</span></span> <span data-ttu-id="8e72c-109">Isso permite que a transferência seja retomada, caso a conexão de rede seja interrompida durante o carregamento.</span><span class="sxs-lookup"><span data-stu-id="8e72c-109">This allows transfer to be resumed, in case the network connection is dropped during upload.</span></span> 

<span data-ttu-id="8e72c-110">A seguir estão as etapas para anexar um arquivo usando uma sessão de carregamento:</span><span class="sxs-lookup"><span data-stu-id="8e72c-110">The following are the steps to attach a file using an upload session:</span></span>

1. <span data-ttu-id="8e72c-111">Criar uma sessão de upload</span><span class="sxs-lookup"><span data-stu-id="8e72c-111">Create an upload session</span></span>
2. <span data-ttu-id="8e72c-112">Dentro dessa sessão de upload, carregue de forma iterativa os intervalos de bytes (até 4 MB cada vez) até que todos os bytes do arquivo tenham sido carregados e o arquivo seja anexado à mensagem especificada</span><span class="sxs-lookup"><span data-stu-id="8e72c-112">Within that upload session, iteratively upload ranges of bytes (up to 4 MB each time) until all the bytes of the file have been uploaded, and the file is attached to the specified message</span></span>
3. <span data-ttu-id="8e72c-113">Salvar a ID do anexo para acesso futuro</span><span class="sxs-lookup"><span data-stu-id="8e72c-113">Save the ID for the attachment for future access</span></span>
4. <span data-ttu-id="8e72c-114">Opcional: excluir a sessão de upload</span><span class="sxs-lookup"><span data-stu-id="8e72c-114">Optional: Delete the upload session</span></span> 

<span data-ttu-id="8e72c-115">Consulte [anexar arquivos grandes às mensagens do Outlook](/graph/outlook-large-attachments) para obter um exemplo.</span><span class="sxs-lookup"><span data-stu-id="8e72c-115">See [attach large files to Outlook messages](/graph/outlook-large-attachments) for an example.</span></span>

> [!TIP]
> <span data-ttu-id="8e72c-116">O Exchange Online permite que os administradores personalizem o limite de tamanho de mensagens de caixas de correio do Office 365, incluindo qualquer anexo de mensagem.</span><span class="sxs-lookup"><span data-stu-id="8e72c-116">Exchange Online lets administrators customize the message size limit for Office 365 mailboxes,  including any message attachments.</span></span> <span data-ttu-id="8e72c-117">Por padrão, esse limite de tamanho de mensagem é de 35 MB.</span><span class="sxs-lookup"><span data-stu-id="8e72c-117">By default, this message size limit is 35 MB.</span></span> <span data-ttu-id="8e72c-118">Descubra como [Personalizar o tamanho máximo da mensagem](https://www.microsoft.com/microsoft-365/blog/2015/04/15/office-365-now-supports-larger-email-messages-up-to-150-mb) para dar suporte a anexos maiores que o limite padrão para o seu locatário.</span><span class="sxs-lookup"><span data-stu-id="8e72c-118">Find out how to [customize the maximum message size](https://www.microsoft.com/microsoft-365/blog/2015/04/15/office-365-now-supports-larger-email-messages-up-to-150-mb) to support attachments larger than the default limit for your tenant.</span></span> 

## <a name="permissions"></a><span data-ttu-id="8e72c-119">Permissões</span><span class="sxs-lookup"><span data-stu-id="8e72c-119">Permissions</span></span>

<span data-ttu-id="8e72c-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e72c-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8e72c-122">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8e72c-122">Permission type</span></span>                        | <span data-ttu-id="8e72c-123">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8e72c-123">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8e72c-124">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8e72c-124">Delegated (work or school account)</span></span>     | <span data-ttu-id="8e72c-125">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8e72c-125">Mail.ReadWrite</span></span> |
| <span data-ttu-id="8e72c-126">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8e72c-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e72c-127">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8e72c-127">Mail.ReadWrite</span></span> |
| <span data-ttu-id="8e72c-128">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8e72c-128">Application</span></span>                            | <span data-ttu-id="8e72c-129">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8e72c-129">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8e72c-130">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8e72c-130">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/attachments/createUploadSession
```

## <a name="request-headers"></a><span data-ttu-id="8e72c-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8e72c-131">Request headers</span></span>

| <span data-ttu-id="8e72c-132">Nome</span><span class="sxs-lookup"><span data-stu-id="8e72c-132">Name</span></span>          | <span data-ttu-id="8e72c-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e72c-133">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8e72c-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="8e72c-134">Authorization</span></span> | <span data-ttu-id="8e72c-135">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="8e72c-135">Bearer {token}</span></span> |


## <a name="request-body"></a><span data-ttu-id="8e72c-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8e72c-136">Request body</span></span>

<span data-ttu-id="8e72c-137">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8e72c-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8e72c-138">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8e72c-138">Parameter</span></span>    | <span data-ttu-id="8e72c-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="8e72c-139">Type</span></span>        | <span data-ttu-id="8e72c-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e72c-140">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8e72c-141">AttachmentItem</span><span class="sxs-lookup"><span data-stu-id="8e72c-141">AttachmentItem</span></span>|[<span data-ttu-id="8e72c-142">attachmentItem</span><span class="sxs-lookup"><span data-stu-id="8e72c-142">attachmentItem</span></span>](../resources/attachmentitem.md)|<span data-ttu-id="8e72c-143">Representa os atributos do item a ser carregado e anexado.</span><span class="sxs-lookup"><span data-stu-id="8e72c-143">Represents attributes of the item to be uploaded and attached.</span></span> <span data-ttu-id="8e72c-144">Especifique, no mínimo, o tipo de`file`anexo (), um nome e o tamanho do arquivo.</span><span class="sxs-lookup"><span data-stu-id="8e72c-144">At minimum, specify the attachment type (`file`), a name, and the size of the file.</span></span>|

## <a name="response"></a><span data-ttu-id="8e72c-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e72c-145">Response</span></span>

<span data-ttu-id="8e72c-146">Se bem-sucedido, este método retorna `201, Created` um código de resposta e um novo objeto [uploadSession](../resources/uploadsession.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8e72c-146">If successful, this method returns `201, Created` response code and a new [uploadSession](../resources/uploadsession.md) object in the response body.</span></span>

><span data-ttu-id="8e72c-147">**Observação**:</span><span class="sxs-lookup"><span data-stu-id="8e72c-147">**Note**:</span></span> 
>
><span data-ttu-id="8e72c-148">A propriedade **uploadUrl** retornada como parte do objeto de resposta **UPLOADSESSION** é uma URL opaca para consultas `PUT` subsequentes para carregar intervalos de bytes do arquivo.</span><span class="sxs-lookup"><span data-stu-id="8e72c-148">The **uploadUrl** property returned as part of the **uploadSession** response object is an opaque URL for subsequent `PUT` queries to upload byte ranges of the file.</span></span> <span data-ttu-id="8e72c-149">Ele contém o token de autenticação apropriado para `PUT` consultas subsequentes que expiram pelo **expirationDateTime**.</span><span class="sxs-lookup"><span data-stu-id="8e72c-149">It contains the appropriate auth token for subsequent `PUT` queries that expire by **expirationDateTime**.</span></span> <span data-ttu-id="8e72c-150">Não Personalize esta URL.</span><span class="sxs-lookup"><span data-stu-id="8e72c-150">Do not customize this URL.</span></span>
>
><span data-ttu-id="8e72c-151">A propriedade **nextExpectedRanges** especifica o próximo local de byte de arquivo para carregar, por exemplo `"NextExpectedRanges":["2097152"]`,.</span><span class="sxs-lookup"><span data-stu-id="8e72c-151">The **nextExpectedRanges** property specifies the next file byte location to upload from, for example, `"NextExpectedRanges":["2097152"]`.</span></span> <span data-ttu-id="8e72c-152">Você deve carregar os bytes em um arquivo na ordem.</span><span class="sxs-lookup"><span data-stu-id="8e72c-152">You must upload bytes in a file in order.</span></span>

<!-- The **nextExpectedRanges** property specifies one or more ranges of bytes that the server is still missing for the file. These ranges are zero-indexed and of the format `{start}-{end}`, unless if the server misses the remainder of the bytes from the start of that range, in which case the format is simply `{start}`.  -->


## <a name="examples"></a><span data-ttu-id="8e72c-153">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8e72c-153">Examples</span></span>

<span data-ttu-id="8e72c-154">Veja a seguir um exemplo de como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="8e72c-154">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="8e72c-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8e72c-155">Request</span></span>

<span data-ttu-id="8e72c-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8e72c-156">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8e72c-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e72c-157">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="8e72c-158">C#</span><span class="sxs-lookup"><span data-stu-id="8e72c-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/attachment-createuploadsession-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8e72c-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e72c-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/attachment-createuploadsession-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8e72c-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8e72c-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/attachment-createuploadsession-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8e72c-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e72c-161">Response</span></span>

<span data-ttu-id="8e72c-162">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8e72c-162">The following is an example of the response.</span></span>

> <span data-ttu-id="8e72c-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8e72c-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
