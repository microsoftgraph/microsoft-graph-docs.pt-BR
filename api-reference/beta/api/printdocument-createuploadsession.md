---
title: 'Documento de documentos: createUploadSession'
description: Criar uma sessão de carregamento para carregar com interseção intervalos de arquivos binários do arquivo de documentos.
localization_priority: Normal
author: nilakhan
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 47043b64806cfa9ef3a66026a60b84ae11112168
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48704875"
---
# <a name="printdocument-createuploadsession"></a><span data-ttu-id="0a8a1-103">Documento de documentos: createUploadSession</span><span class="sxs-lookup"><span data-stu-id="0a8a1-103">printDocument: createUploadSession</span></span>

<span data-ttu-id="0a8a1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a8a1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a8a1-105">Criar uma sessão de carregamento que permite que um aplicativo carregue intervalos de forma iterativa de um arquivo binário vinculado ao documento de impressão.</span><span class="sxs-lookup"><span data-stu-id="0a8a1-105">Create an upload session that allows an app to iteratively upload ranges of a binary file linked to the print document.</span></span>

<span data-ttu-id="0a8a1-106">Como parte da resposta, esta ação retorna uma URL de upload que pode ser usada em consultas sequenciais subsequentes `PUT` .</span><span class="sxs-lookup"><span data-stu-id="0a8a1-106">As part of the response, this action returns an upload URL that can be used in subsequent sequential `PUT` queries.</span></span> <span data-ttu-id="0a8a1-107">Os cabeçalhos de solicitação de cada `PUT` operação podem ser usados para especificar o intervalo exato de bytes a serem carregados.</span><span class="sxs-lookup"><span data-stu-id="0a8a1-107">Request headers for each `PUT` operation can be used to specify the exact range of bytes to be uploaded.</span></span> <span data-ttu-id="0a8a1-108">Isso permite que a transferência seja retomada, caso a conexão de rede seja interrompida durante o carregamento.</span><span class="sxs-lookup"><span data-stu-id="0a8a1-108">This allows transfer to be resumed, in case the network connection is dropped during upload.</span></span> 

## <a name="permissions"></a><span data-ttu-id="0a8a1-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="0a8a1-109">Permissions</span></span>

<span data-ttu-id="0a8a1-110">Uma das seguintes permissões é necessária para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="0a8a1-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="0a8a1-111">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a8a1-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
<span data-ttu-id="0a8a1-112">Além das permissões a seguir, o locatário do usuário ou do aplicativo deve ter uma assinatura de impressão universal ativa e ter uma permissão que conceda [obter impressora](printer-get.md) ou obter o acesso do [printerShare](printershare-get.md) , dependendo se a impressora ou o printerShare está sendo usado.</span><span class="sxs-lookup"><span data-stu-id="0a8a1-112">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) or [Get printerShare](printershare-get.md) access depending upon whether printer or printerShare is being used.</span></span>

| <span data-ttu-id="0a8a1-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0a8a1-113">Permission type</span></span>                        | <span data-ttu-id="0a8a1-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0a8a1-114">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0a8a1-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0a8a1-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="0a8a1-116">PrintJob. ReadWrite, PrintJob. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="0a8a1-116">PrintJob.ReadWrite, PrintJob.ReadWrite.All</span></span> |
| <span data-ttu-id="0a8a1-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0a8a1-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a8a1-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0a8a1-118">Not Supported.</span></span> |
| <span data-ttu-id="0a8a1-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0a8a1-119">Application</span></span>                            | <span data-ttu-id="0a8a1-120">PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a8a1-120">PrintJob.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0a8a1-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0a8a1-121">HTTP request</span></span>

<span data-ttu-id="0a8a1-122">Para criar uma sessão de carregamento usando **impressora**:</span><span class="sxs-lookup"><span data-stu-id="0a8a1-122">To create an upload session using **printer**:</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/documents/{id}/createUploadSession
```

<span data-ttu-id="0a8a1-123">Para criar uma sessão de carregamento usando o **printerShare**:</span><span class="sxs-lookup"><span data-stu-id="0a8a1-123">To create an upload session using **printerShare**:</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST /print/shares/{id}/jobs/{id}/documents/{id}/createUploadSession
```

## <a name="request-headers"></a><span data-ttu-id="0a8a1-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0a8a1-124">Request headers</span></span>

| <span data-ttu-id="0a8a1-125">Nome</span><span class="sxs-lookup"><span data-stu-id="0a8a1-125">Name</span></span>          | <span data-ttu-id="0a8a1-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a8a1-126">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="0a8a1-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="0a8a1-127">Authorization</span></span> | <span data-ttu-id="0a8a1-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0a8a1-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0a8a1-130">Content-type</span><span class="sxs-lookup"><span data-stu-id="0a8a1-130">Content-type</span></span> | <span data-ttu-id="0a8a1-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0a8a1-p104">application/json. Required.</span></span>|


## <a name="request-body"></a><span data-ttu-id="0a8a1-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0a8a1-133">Request body</span></span>

<span data-ttu-id="0a8a1-134">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0a8a1-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0a8a1-135">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="0a8a1-135">Parameter</span></span>    | <span data-ttu-id="0a8a1-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="0a8a1-136">Type</span></span>        | <span data-ttu-id="0a8a1-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a8a1-137">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0a8a1-138">propriedades</span><span class="sxs-lookup"><span data-stu-id="0a8a1-138">properties</span></span>|[<span data-ttu-id="0a8a1-139">printDocumentUploadProperties</span><span class="sxs-lookup"><span data-stu-id="0a8a1-139">printDocumentUploadProperties</span></span>](../resources/printDocumentUploadProperties.md)|<span data-ttu-id="0a8a1-140">Representa as propriedades do arquivo binário a ser carregado.</span><span class="sxs-lookup"><span data-stu-id="0a8a1-140">Represents properties of the binary file to be uploaded.</span></span>|

## <a name="response"></a><span data-ttu-id="0a8a1-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a8a1-141">Response</span></span>

<span data-ttu-id="0a8a1-142">Se tiver êxito, este método retornará um `200 OK` código de resposta e um novo objeto [uploadSession](../resources/uploadsession.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0a8a1-142">If successful, this method returns a `200 OK` response code and a new [uploadSession](../resources/uploadsession.md) object in the response body.</span></span>

><span data-ttu-id="0a8a1-143">**Observação**: a propriedade **uploadUrl** retornada como parte do objeto de resposta **uploadSession** é uma URL opaca para consultas subsequentes `PUT` para carregar intervalos de bytes do arquivo.</span><span class="sxs-lookup"><span data-stu-id="0a8a1-143">**Note**: The **uploadUrl** property returned as part of the **uploadSession** response object is an opaque URL for subsequent `PUT` queries to upload byte ranges of the file.</span></span> <span data-ttu-id="0a8a1-144">Ele contém o token de autenticação apropriado para `PUT` consultas subsequentes que expiram pelo **expirationDateTime**.</span><span class="sxs-lookup"><span data-stu-id="0a8a1-144">It contains the appropriate auth token for subsequent `PUT` queries that expire by **expirationDateTime**.</span></span> <span data-ttu-id="0a8a1-145">Não altere essa URL.</span><span class="sxs-lookup"><span data-stu-id="0a8a1-145">Do not change this URL.</span></span>

## <a name="examples"></a><span data-ttu-id="0a8a1-146">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0a8a1-146">Examples</span></span>

<span data-ttu-id="0a8a1-147">O exemplo a seguir mostra como criar uma sessão de carregamento que você pode usar em operações de upload de arquivo subsequentes para o documento de documentos.</span><span class="sxs-lookup"><span data-stu-id="0a8a1-147">The following example shows how to create an upload session that you can use in subsequent file upload operations to the specified printDocument.</span></span>

### <a name="request"></a><span data-ttu-id="0a8a1-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0a8a1-148">Request</span></span>

<!-- {
  "blockType": "request",
}-->
```http
POST https://graph.microsoft.com/beta/print/shares/1c879027-5120-4aaf-954a-ebfd509a3bcc/jobs/46207/documents/9001bcd9-e36a-4f51-bfc6-140c3ad7f9f7/createUploadSession
Content-type: application/json

{
  "properties": {
    "documentName": "TestFile.pdf",
    "contentType": "application/pdf", 
    "size": 4533322
  }
}
```

### <a name="response"></a><span data-ttu-id="0a8a1-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a8a1-149">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.uploadSession"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.uploadSession",
    "uploadUrl": "https://print.print.microsoft.com/uploadSessions/5400be13-5a4e-4c20-be70-90c85bfe5d6e?tempauthtoken={token}",
    "expirationDateTime": "2020-10-25T02:19:38.1694207Z",
    "nextExpectedRanges": [
        "0-4533321"
    ]
}
```
