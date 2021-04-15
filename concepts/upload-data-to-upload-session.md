---
title: Faça o upload de documentos utilizando a API de Impressão Universal do Microsoft Graph
description: A Impressão Universal é uma solução de impressão moderna que as organizações podem utilizar para gerenciar sua infraestrutura de impressão por meio de serviços em nuvem da Microsoft.
author: nilakhan
localization_priority: Priority
ms.prod: universal-print
ms.custom: scenarios:getting-started
ms.openlocfilehash: c51d027a0e76f24f6ec4788ae1429adcc29f2948
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766312"
---
# <a name="upload-documents-using-the-microsoft-graph-universal-print-api"></a><span data-ttu-id="10c1b-103">Faça o upload de documentos utilizando a API de Impressão Universal do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="10c1b-103">Upload documents using the Microsoft Graph Universal Print API</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../api-reference/includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="10c1b-104">Para imprimir um documento utilizando a API de Impressão Universal no Microsoft Graph, você [cria um trabalho de impressão](/graph/api/printershare-post-jobs), faz o upload do documento e, em seguida, [inicia o trabalho de impressão](/graph/api/printjob-start).</span><span class="sxs-lookup"><span data-stu-id="10c1b-104">To print a document using the Universal Print API in Microsoft Graph, you [create a print job](/graph/api/printershare-post-jobs), upload a document, and then [start the print job](/graph/api/printjob-start).</span></span> <span data-ttu-id="10c1b-105">Este artigo descreve como fazer o upload de um documento, que começa com [ a criação de uma sessão de upload ](/graph/api/printdocument-createuploadsession).</span><span class="sxs-lookup"><span data-stu-id="10c1b-105">This article describes how to upload a document, which starts with [creating an upload session](/graph/api/printdocument-createuploadsession).</span></span>

<span data-ttu-id="10c1b-106">Para fazer o upload de um arquivo, ou de parte de um arquivo, seu aplicativo faz uma solicitação PUT para o valor **uploadUrl** recebido na resposta **createUploadSession**.</span><span class="sxs-lookup"><span data-stu-id="10c1b-106">To upload a file, or a portion of a file, your app makes a PUT request to the **uploadUrl** value received in the **createUploadSession** response.</span></span>
<span data-ttu-id="10c1b-107">Você pode fazer o upload de todo o arquivo ou dividi-lo em vários intervalos de bytes, desde que o máximo de bytes em qualquer solicitação seja inferior a 10 MB.</span><span class="sxs-lookup"><span data-stu-id="10c1b-107">You can upload the entire file, or split the file into multiple byte ranges, as long as the maximum bytes in any given request is less than 10 MB.</span></span>

<span data-ttu-id="10c1b-108">É possível fazer o upload dos segmentos do arquivo em qualquer ordem e o upload pode ser feito em paralelo, com até quatro solicitações simultâneas.</span><span class="sxs-lookup"><span data-stu-id="10c1b-108">The segments of the file can be uploaded in any order and can be uploaded in parallel, with up to four concurrent requests.</span></span> <span data-ttu-id="10c1b-109">Quando todos os segmentos binários do documento são carregados, o arquivo binário é vinculado ao **printDocument**.</span><span class="sxs-lookup"><span data-stu-id="10c1b-109">When all the binary segments of document are uploaded, the binary file is linked to the **printDocument**.</span></span>

## <a name="http-request"></a><span data-ttu-id="10c1b-110">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="10c1b-110">HTTP request</span></span>

<span data-ttu-id="10c1b-111">Faça uma solicitação PUT para o valor **uploadUrl** recebido na resposta **createUploadSession**.</span><span class="sxs-lookup"><span data-stu-id="10c1b-111">Make a PUT request to the **uploadUrl** value received in the **createUploadSession** response.</span></span>

### <a name="request-headers"></a><span data-ttu-id="10c1b-112">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="10c1b-112">Request headers</span></span>
| <span data-ttu-id="10c1b-113">Nome</span><span class="sxs-lookup"><span data-stu-id="10c1b-113">Name</span></span>          | <span data-ttu-id="10c1b-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="10c1b-114">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="10c1b-115">Intervalo do conteúdo</span><span class="sxs-lookup"><span data-stu-id="10c1b-115">Content-Range</span></span> | <span data-ttu-id="10c1b-116">bytes {startByteIndex}-{endByteIndex}/{documentSizeInBytes}.</span><span class="sxs-lookup"><span data-stu-id="10c1b-116">bytes {startByteIndex}-{endByteIndex}‬/{documentSizeInBytes}.</span></span> <span data-ttu-id="10c1b-117">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="10c1b-117">Required.</span></span>|
| <span data-ttu-id="10c1b-118">Comprimento do Conteúdo</span><span class="sxs-lookup"><span data-stu-id="10c1b-118">Content-Length</span></span> | <span data-ttu-id="10c1b-119">{contentLength} Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="10c1b-119">{contentLength}‬ Required.</span></span>|

### <a name="request-body"></a><span data-ttu-id="10c1b-120">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="10c1b-120">Request body</span></span>
<span data-ttu-id="10c1b-121">O corpo da solicitação é um blob binário que contém os bytes do documento que são especificados como um intervalo de bytes **inclusivo** no cabeçalho `Content-Range`.</span><span class="sxs-lookup"><span data-stu-id="10c1b-121">The request body is a binary blob containing the bytes of the document that are specified as an **inclusive** byte range in the `Content-Range` header.</span></span> 

### <a name="example"></a><span data-ttu-id="10c1b-122">Exemplo</span><span class="sxs-lookup"><span data-stu-id="10c1b-122">Example</span></span>

```http
PUT https://print.print.microsoft.com/uploadSessions/5400be13-5a4e-4c20-be70-90c85bfe5d6e?tempauthtoken={token}
Content-Range: bytes=0-72796/4533322
Content-Length: 72797

<bytes 0-72796 of the file>

```

<span data-ttu-id="10c1b-123">Aqui, 0 e 72796 são os índices inicial e final do segmento de arquivo, e 4533322 é o tamanho do documento.</span><span class="sxs-lookup"><span data-stu-id="10c1b-123">Here, 0 and 72796 are the start and end indexes of the file segment and 4533322 is the size of document.</span></span>
### <a name="http-response"></a><span data-ttu-id="10c1b-124">Resposta HTTP:</span><span class="sxs-lookup"><span data-stu-id="10c1b-124">HTTP response</span></span>

<span data-ttu-id="10c1b-125">Quando a solicitação for concluída, o servidor responderá com `202 Accepted` se houver mais intervalos de bytes que precisem ser carregados.</span><span class="sxs-lookup"><span data-stu-id="10c1b-125">When the request is complete, the server will respond with `202 Accepted` if there are more byte ranges that need to be uploaded.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->

```http
HTTP/1.1 202 Accepted
Content-Type: application/json

{
  "expirationDateTime": "2020-10-25T02:19:38.1694207Z",
  "nextExpectedRanges": ["72797-4533321"]
}
```

<span data-ttu-id="10c1b-126">O aplicativo pode usar o valor de **nextExpectedRanges** para determinar onde iniciar o próximo intervalo de bytes.</span><span class="sxs-lookup"><span data-stu-id="10c1b-126">Your app can use the **nextExpectedRanges** value to determine where to start the next byte range.</span></span> <span data-ttu-id="10c1b-127">Você pode ver vários intervalos especificados, indicando as partes do arquivo que o servidor ainda não recebeu.</span><span class="sxs-lookup"><span data-stu-id="10c1b-127">You might see multiple ranges specified, indicating parts of the file that the server has not yet received.</span></span> <span data-ttu-id="10c1b-128">A propriedade **nextExpectedRanges** indica intervalos do arquivo que não foram recebidos, e não um padrão para como seu aplicativo deve carregar o arquivo.</span><span class="sxs-lookup"><span data-stu-id="10c1b-128">The **nextExpectedRanges** property indicates ranges of the file that have not been received and not a pattern for how your app should upload the file.</span></span>

<!-- { "blockType": "ignored", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->

```http
HTTP/1.1 202 Accepted
Content-Type: application/json

{
  "expirationDateTime": "2020-10-25T02:19:38.1694207Z",
  "nextExpectedRanges": [
  "72797-72897",
  "78929-4533322"
  ]
}
```

### <a name="remarks"></a><span data-ttu-id="10c1b-129">Comentários</span><span class="sxs-lookup"><span data-stu-id="10c1b-129">Remarks</span></span>

* <span data-ttu-id="10c1b-p106">Em falhas quando o cliente enviou um fragmento que o servidor já havia recebido, o servidor responderá com `HTTP 416 Requested Range Not Satisfiable`. Você pode [solicitar o status do upload](#get-the-upload-session) para obter uma lista mais detalhada dos intervalos que estão faltando.</span><span class="sxs-lookup"><span data-stu-id="10c1b-p106">On failures when the client sent a fragment the server had already received, the server will respond with `HTTP 416 Requested Range Not Satisfiable`. You can [request upload status](#get-the-upload-session) to get a more detailed list of missing ranges.</span></span>
* <span data-ttu-id="10c1b-132">Incluir o Cabeçalho de Autorização ao emitir a chamada `PUT`pode resultar em uma resposta`HTTP 401 Unauthorized`.</span><span class="sxs-lookup"><span data-stu-id="10c1b-132">Including the Authorization header when issuing the `PUT` call might result in a `HTTP 401 Unauthorized` response.</span></span> <span data-ttu-id="10c1b-133">O Cabeçalho de Autorização e o token do portador devem ser enviados apenas durante a criação da sessão de upload.</span><span class="sxs-lookup"><span data-stu-id="10c1b-133">The Authorization header and bearer token should only be sent when creating upload session.</span></span> <span data-ttu-id="10c1b-134">Não deve ser incluído ao enviar dados para a sessão de upload.</span><span class="sxs-lookup"><span data-stu-id="10c1b-134">It should be not be included when uploading data to upload session.</span></span>

## <a name="completing-a-file"></a><span data-ttu-id="10c1b-135">Concluindo um arquivo</span><span class="sxs-lookup"><span data-stu-id="10c1b-135">Completing a file</span></span>

<span data-ttu-id="10c1b-136">Quando o último intervalo de bytes de um arquivo for recebido, o servidor responderá com um `HTTP 201 Created`.</span><span class="sxs-lookup"><span data-stu-id="10c1b-136">When the last byte range of a file is received, the server will response with an `HTTP 201 Created`.</span></span> <span data-ttu-id="10c1b-137">O corpo da resposta também incluirá o conjunto de propriedades para o **printDocument** associado.</span><span class="sxs-lookup"><span data-stu-id="10c1b-137">The response body will also include the property set for the associated **printDocument**.</span></span>

<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-final", "scopes": "printjob.readwrite" } -->

```http
PUT https://print.print.microsoft.com/uploadSessions/5400be13-5a4e-4c20-be70-90c85bfe5d6e?tempauthtoken={token}
Content-Length: 10
Content-Range: bytes 4533312-4533321/4533322

<final bytes of the file>
```

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.printDocument", "truncated": true } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
   "id": "9001bcd9-e36a-4f51-bfc6-140c3ad7f9f7",
   "documentName": "TestFile.pdf",
   "contentType": "application/pdf", 
   "size": 4533322
}
```

><span data-ttu-id="10c1b-138">**Observação:** A sessão de upload é excluída após a conclusão do upload do documento.</span><span class="sxs-lookup"><span data-stu-id="10c1b-138">**Note:** Upload session is deleted after document upload is complete.</span></span>

## <a name="get-the-upload-session"></a><span data-ttu-id="10c1b-139">Obtenha a sessão de upload</span><span class="sxs-lookup"><span data-stu-id="10c1b-139">Get the upload session</span></span>

<span data-ttu-id="10c1b-140">Para obter a sessão de upload, envie uma solicitação GET para o URL de upload.</span><span class="sxs-lookup"><span data-stu-id="10c1b-140">To get upload session, send a GET request to the upload URL.</span></span> 

### <a name="request"></a><span data-ttu-id="10c1b-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="10c1b-141">Request</span></span>
<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-resume", "scopes": "files.readwrite" } -->

```http
GET https://print.print.microsoft.com/uploadSessions/5400be13-5a4e-4c20-be70-90c85bfe5d6e?tempauthtoken={token}
```

### <a name="response"></a><span data-ttu-id="10c1b-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="10c1b-142">Response</span></span>

<!-- { "blockType": "response" } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "expirationDateTime": "2020-10-25T02:19:38.1694207Z",
  "nextExpectedRanges": [
  "72797-72897",
  "78929-4533322"
  ]
}
```

## <a name="cancel-the-upload-session"></a><span data-ttu-id="10c1b-143">Cancelar a sessão de upload</span><span class="sxs-lookup"><span data-stu-id="10c1b-143">Cancel the upload session</span></span>

<span data-ttu-id="10c1b-144">Para cancelar uma sessão de upload, envie uma solicitação DELETE para o URL de upload.</span><span class="sxs-lookup"><span data-stu-id="10c1b-144">To cancel an upload session, send a DELETE request to the upload URL.</span></span> <span data-ttu-id="10c1b-145">Isso deve ser usado em cenários em que o upload é interrompido, por exemplo, se o usuário cancelar a transferência.</span><span class="sxs-lookup"><span data-stu-id="10c1b-145">This should be used in scenarios where the upload is aborted, for example, if the user cancels the transfer.</span></span>

<span data-ttu-id="10c1b-146">Os arquivos temporários e a sessão de carregamento que os acompanha são automaticamente limpos decorrido o valor de **expirationDateTime**.</span><span class="sxs-lookup"><span data-stu-id="10c1b-146">Temporary files and their accompanying upload session are automatically cleaned up after the **expirationDateTime** has passed.</span></span>

### <a name="request"></a><span data-ttu-id="10c1b-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="10c1b-147">Request</span></span>

<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-cancel", "scopes": "printjob.readwrite" } -->

```http
DELETE https://print.print.microsoft.com/uploadSessions/5400be13-5a4e-4c20-be70-90c85bfe5d6e?tempauthtoken={token}
```

### <a name="response"></a><span data-ttu-id="10c1b-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="10c1b-148">Response</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```
