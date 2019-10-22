---
title: 'Anexo: createUploadSession'
description: Crie uma sessão de upload para carregar de forma iterativa os intervalos de um arquivo para anexar o arquivo à mensagem especificada.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 116b73b53689c01e346568b6b5d67e56fb31b283
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2019
ms.locfileid: "37621599"
---
# <a name="attachment-createuploadsession"></a><span data-ttu-id="7aba7-103">Anexo: createUploadSession</span><span class="sxs-lookup"><span data-stu-id="7aba7-103">attachment: createUploadSession</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7aba7-104">Criar uma sessão de carregamento que permite que um aplicativo carregue intervalos de um arquivo de forma iterativa, para anexar o arquivo à [mensagem](../resources/message.md)especificada.</span><span class="sxs-lookup"><span data-stu-id="7aba7-104">Create an upload session that allows an app to iteratively upload ranges of a file, so as to attach the file to the specified [message](../resources/message.md).</span></span>

<span data-ttu-id="7aba7-105">Use essa abordagem para anexar arquivos de tamanhos entre 3 MB e 150MB a uma **mensagem**.</span><span class="sxs-lookup"><span data-stu-id="7aba7-105">Use this approach to attach files of sizes between 3MB and 150MB to a **message**.</span></span> <span data-ttu-id="7aba7-106">Para anexar arquivos de tamanhos em 4 MB, basta [postar na propriedade de navegação Attachments](message-post-attachments.md).</span><span class="sxs-lookup"><span data-stu-id="7aba7-106">To attach files of sizes under 4MB, simply [POST on the attachments navigation property](message-post-attachments.md).</span></span> 

<span data-ttu-id="7aba7-107">Como parte da resposta, esta ação retorna uma URL de upload que você pode usar em consultas sequenciais `PUT` subsequentes.</span><span class="sxs-lookup"><span data-stu-id="7aba7-107">As part of the response, this action returns an upload URL that you can use in subsequent sequential `PUT` queries.</span></span> <span data-ttu-id="7aba7-108">Os cabeçalhos de solicitação `PUT` para cada operação permitem que você especifique o intervalo exato de bytes a serem carregados.</span><span class="sxs-lookup"><span data-stu-id="7aba7-108">Request headers for each `PUT` operation let you specify the exact range of bytes to be uploaded.</span></span> <span data-ttu-id="7aba7-109">Isso permite que a transferência seja retomada, caso a conexão de rede seja interrompida durante o carregamento.</span><span class="sxs-lookup"><span data-stu-id="7aba7-109">This allows transfer to be resumed, in case the network connection is dropped during upload.</span></span> 

<span data-ttu-id="7aba7-110">A seguir estão as etapas para anexar um arquivo usando uma sessão de carregamento:</span><span class="sxs-lookup"><span data-stu-id="7aba7-110">The following are the steps to attach a file using an upload session:</span></span>

1. <span data-ttu-id="7aba7-111">Criar uma sessão de upload</span><span class="sxs-lookup"><span data-stu-id="7aba7-111">Create an upload session</span></span>
2. <span data-ttu-id="7aba7-112">Dentro dessa sessão de upload, carregue de forma iterativa os intervalos de bytes (até 4 MB cada vez) até que todos os bytes do arquivo tenham sido carregados e o arquivo seja anexado à mensagem especificada</span><span class="sxs-lookup"><span data-stu-id="7aba7-112">Within that upload session, iteratively upload ranges of bytes (up to 4 MB each time) until all the bytes of the file have been uploaded, and the file is attached to the specified message</span></span>
3. <span data-ttu-id="7aba7-113">Salvar a ID do anexo para acesso futuro</span><span class="sxs-lookup"><span data-stu-id="7aba7-113">Save the ID for the attachment for future access</span></span>
4. <span data-ttu-id="7aba7-114">Opcional: excluir a sessão de upload</span><span class="sxs-lookup"><span data-stu-id="7aba7-114">Optional: Delete the upload session</span></span> 

<span data-ttu-id="7aba7-115">Consulte [anexar arquivos grandes às mensagens do Outlook](/graph/outlook-large-attachments) para obter um exemplo.</span><span class="sxs-lookup"><span data-stu-id="7aba7-115">See [attach large files to Outlook messages](/graph/outlook-large-attachments) for an example.</span></span>


## <a name="permissions"></a><span data-ttu-id="7aba7-116">Permissões</span><span class="sxs-lookup"><span data-stu-id="7aba7-116">Permissions</span></span>

<span data-ttu-id="7aba7-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7aba7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7aba7-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7aba7-119">Permission type</span></span>                        | <span data-ttu-id="7aba7-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7aba7-120">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7aba7-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7aba7-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="7aba7-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7aba7-122">Mail.ReadWrite</span></span> |
| <span data-ttu-id="7aba7-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7aba7-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7aba7-124">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7aba7-124">Mail.ReadWrite</span></span> |
| <span data-ttu-id="7aba7-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7aba7-125">Application</span></span>                            | <span data-ttu-id="7aba7-126">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7aba7-126">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="7aba7-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7aba7-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/attachments/createUploadSession
```

## <a name="request-headers"></a><span data-ttu-id="7aba7-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7aba7-128">Request headers</span></span>

| <span data-ttu-id="7aba7-129">Nome</span><span class="sxs-lookup"><span data-stu-id="7aba7-129">Name</span></span>          | <span data-ttu-id="7aba7-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="7aba7-130">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="7aba7-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="7aba7-131">Authorization</span></span> | <span data-ttu-id="7aba7-132">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="7aba7-132">Bearer {token}</span></span> |


## <a name="request-body"></a><span data-ttu-id="7aba7-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7aba7-133">Request body</span></span>

<span data-ttu-id="7aba7-134">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7aba7-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7aba7-135">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="7aba7-135">Parameter</span></span>    | <span data-ttu-id="7aba7-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="7aba7-136">Type</span></span>        | <span data-ttu-id="7aba7-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="7aba7-137">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7aba7-138">AttachmentItem</span><span class="sxs-lookup"><span data-stu-id="7aba7-138">AttachmentItem</span></span>|[<span data-ttu-id="7aba7-139">attachmentItem</span><span class="sxs-lookup"><span data-stu-id="7aba7-139">attachmentItem</span></span>](../resources/attachmentitem.md)|<span data-ttu-id="7aba7-140">Representa os atributos do item a ser carregado e anexado.</span><span class="sxs-lookup"><span data-stu-id="7aba7-140">Represents attributes of the item to be uploaded and attached.</span></span> <span data-ttu-id="7aba7-141">Especifique, no mínimo, o tipo de`file`anexo (), um nome e o tamanho do arquivo.</span><span class="sxs-lookup"><span data-stu-id="7aba7-141">At minimum, specify the attachment type (`file`), a name, and the size of the file.</span></span>|

## <a name="response"></a><span data-ttu-id="7aba7-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="7aba7-142">Response</span></span>

<span data-ttu-id="7aba7-143">Se bem-sucedido, este método retorna `201, Created` um código de resposta e um novo objeto [uploadSession](../resources/uploadsession.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7aba7-143">If successful, this method returns `201, Created` response code and a new [uploadSession](../resources/uploadsession.md) object in the response body.</span></span>

><span data-ttu-id="7aba7-144">**Observação**:</span><span class="sxs-lookup"><span data-stu-id="7aba7-144">**Note**:</span></span> 
>
><span data-ttu-id="7aba7-145">A propriedade **uploadUrl** retornada como parte do objeto de resposta **UPLOADSESSION** é uma URL opaca para consultas `PUT` subsequentes para carregar intervalos de bytes do arquivo.</span><span class="sxs-lookup"><span data-stu-id="7aba7-145">The **uploadUrl** property returned as part of the **uploadSession** response object is an opaque URL for subsequent `PUT` queries to upload byte ranges of the file.</span></span> <span data-ttu-id="7aba7-146">Ele contém o token de autenticação apropriado para `PUT` consultas subsequentes que expiram pelo **expirationDateTime**.</span><span class="sxs-lookup"><span data-stu-id="7aba7-146">It contains the appropriate auth token for subsequent `PUT` queries that expire by **expirationDateTime**.</span></span> <span data-ttu-id="7aba7-147">Não Personalize esta URL.</span><span class="sxs-lookup"><span data-stu-id="7aba7-147">Do not customize this URL.</span></span>
>
><span data-ttu-id="7aba7-148">A propriedade **nextExpectedRanges** especifica o próximo local de byte de arquivo para carregar, por exemplo `"NextExpectedRanges":["2097152"]`,.</span><span class="sxs-lookup"><span data-stu-id="7aba7-148">The **nextExpectedRanges** property specifies the next file byte location to upload from, for example, `"NextExpectedRanges":["2097152"]`.</span></span> <span data-ttu-id="7aba7-149">Você deve carregar bytes em um arquivo na ordem.</span><span class="sxs-lookup"><span data-stu-id="7aba7-149">You must upload bytes in a file in order.</span></span>

<!-- The **nextExpectedRanges** property specifies one or more ranges of bytes that the server is still missing for the file. These ranges are zero-indexed and of the format `{start}-{end}`, unless if the server misses the remainder of the bytes from the start of that range, in which case the format is simply `{start}`.  -->


## <a name="examples"></a><span data-ttu-id="7aba7-150">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7aba7-150">Examples</span></span>

<span data-ttu-id="7aba7-151">Veja a seguir um exemplo de como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="7aba7-151">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="7aba7-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7aba7-152">Request</span></span>

<span data-ttu-id="7aba7-153">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7aba7-153">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7aba7-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="7aba7-154">Response</span></span>

<span data-ttu-id="7aba7-155">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7aba7-155">The following is an example of the response.</span></span>

> <span data-ttu-id="7aba7-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7aba7-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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