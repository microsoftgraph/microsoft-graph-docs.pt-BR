---
title: 'Documento de documentos: uploadData'
description: Carregar um único segmento binário do documento.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 320d55cd049bdd558e8f847e2ac01593cc2f5ca7
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980976"
---
# <a name="printdocument-uploaddata"></a><span data-ttu-id="c91ff-103">Documento de documentos: uploadData</span><span class="sxs-lookup"><span data-stu-id="c91ff-103">printDocument: uploadData</span></span>

<span data-ttu-id="c91ff-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c91ff-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c91ff-105">Carregar um único segmento binário do **documento**.</span><span class="sxs-lookup"><span data-stu-id="c91ff-105">Upload a single binary segment of the **printDocument**.</span></span>

<span data-ttu-id="c91ff-106">É possível carregar o arquivo inteiro ou dividir o arquivo em vários intervalos de bytes, desde que nenhuma solicitação seja maior do que 1 MB.</span><span class="sxs-lookup"><span data-stu-id="c91ff-106">You can upload the entire file, or split the file into multiple byte ranges, as long as no request is larger than 1 MB.</span></span>

<span data-ttu-id="c91ff-107">É possível fazer o upload dos segmentos do arquivo em qualquer ordem e o upload pode ser feito em paralelo, com até quatro solicitações simultâneas.</span><span class="sxs-lookup"><span data-stu-id="c91ff-107">The segments of the file can be uploaded in any order and can be uploaded in parallel, with up to four concurrent requests.</span></span> <span data-ttu-id="c91ff-108">Quando todos os segmentos binários do documento são carregados, o arquivo binário é vinculado ao **printJob**.</span><span class="sxs-lookup"><span data-stu-id="c91ff-108">When all the binary segments of document are uploaded, the binary file is linked to the **printJob**.</span></span>

## <a name="permissions"></a><span data-ttu-id="c91ff-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="c91ff-109">Permissions</span></span>
<span data-ttu-id="c91ff-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c91ff-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="c91ff-112">Além das permissões a seguir, o locatário do usuário ou do aplicativo deve ter uma assinatura universal de impressão ativa e ter uma permissão que conceda obter acesso à [impressora](printer-get.md) .</span><span class="sxs-lookup"><span data-stu-id="c91ff-112">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) access.</span></span>

|<span data-ttu-id="c91ff-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c91ff-113">Permission type</span></span> | <span data-ttu-id="c91ff-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c91ff-114">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="c91ff-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c91ff-115">Delegated (work or school account)</span></span>| <span data-ttu-id="c91ff-116">PrintJob. ReadWrite, PrintJob. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="c91ff-116">PrintJob.ReadWrite, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="c91ff-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c91ff-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c91ff-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c91ff-118">Not Supported.</span></span>|
|<span data-ttu-id="c91ff-119">Application</span><span class="sxs-lookup"><span data-stu-id="c91ff-119">Application</span></span>| <span data-ttu-id="c91ff-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c91ff-120">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c91ff-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c91ff-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/documents/{id}/uploadData
```
## <a name="request-headers"></a><span data-ttu-id="c91ff-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c91ff-122">Request headers</span></span>
| <span data-ttu-id="c91ff-123">Nome</span><span class="sxs-lookup"><span data-stu-id="c91ff-123">Name</span></span>          | <span data-ttu-id="c91ff-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="c91ff-124">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="c91ff-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="c91ff-125">Authorization</span></span> | <span data-ttu-id="c91ff-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c91ff-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c91ff-128">Range</span><span class="sxs-lookup"><span data-stu-id="c91ff-128">Range</span></span> | <span data-ttu-id="c91ff-129">bytes = {startByteIndex}-{endByteIndex}</span><span class="sxs-lookup"><span data-stu-id="c91ff-129">bytes={startByteIndex}-{endByteIndex}‬</span></span>  |
| <span data-ttu-id="c91ff-130">Comprimento do Conteúdo</span><span class="sxs-lookup"><span data-stu-id="c91ff-130">Content-Length</span></span> | <span data-ttu-id="c91ff-131">ContentLength</span><span class="sxs-lookup"><span data-stu-id="c91ff-131">{contentLength}‬</span></span>  |
| <span data-ttu-id="c91ff-132">Content-type</span><span class="sxs-lookup"><span data-stu-id="c91ff-132">Content-type</span></span>  | <span data-ttu-id="c91ff-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c91ff-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c91ff-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c91ff-135">Request body</span></span>
<span data-ttu-id="c91ff-136">O corpo da solicitação é um blob binário que contém os bytes do documento que são especificados como um intervalo de bytes inclusivo no cabeçalho `Range`.</span><span class="sxs-lookup"><span data-stu-id="c91ff-136">The request body is a binary blob containing the bytes of the document that are specified as an inclusive byte range in the `Range` header.</span></span> 

## <a name="response"></a><span data-ttu-id="c91ff-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="c91ff-137">Response</span></span>
<span data-ttu-id="c91ff-138">Se tiver êxito, este método retornará uma das seguintes respostas.</span><span class="sxs-lookup"><span data-stu-id="c91ff-138">If successful, this method returns one of the following responses.</span></span> <span data-ttu-id="c91ff-139">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c91ff-139">It does not return anything in the response body.</span></span>

| <span data-ttu-id="c91ff-140">Condição</span><span class="sxs-lookup"><span data-stu-id="c91ff-140">Condition</span></span>     | <span data-ttu-id="c91ff-141">Código da resposta</span><span class="sxs-lookup"><span data-stu-id="c91ff-141">Response code</span></span> |
|:--------------|:--------------|
| <span data-ttu-id="c91ff-142">Um ou mais segmentos binários ainda precisam ser carregados</span><span class="sxs-lookup"><span data-stu-id="c91ff-142">One or more binary segments still need to be uploaded</span></span> | `202 Accepted` |
| <span data-ttu-id="c91ff-143">Todos os segmentos binários foram carregados com êxito</span><span class="sxs-lookup"><span data-stu-id="c91ff-143">All binary segments have been uploaded successfully</span></span> | `201 Created` |

## <a name="example"></a><span data-ttu-id="c91ff-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c91ff-144">Example</span></span>
<span data-ttu-id="c91ff-145">O exemplo a seguir mostra como chamar essa API para carregar os primeiros 72797 bytes de um documento.</span><span class="sxs-lookup"><span data-stu-id="c91ff-145">The following example shows how to call this API to upload the first 72797 bytes of a document.</span></span>
##### <a name="request"></a><span data-ttu-id="c91ff-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c91ff-146">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c91ff-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="c91ff-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printdocument-uploaddata"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/jobs/{id}/documents/{id}/uploadData
Range: bytes=0-72796
Content-Length: 72797
```
# <a name="c"></a>[<span data-ttu-id="c91ff-148">C#</span><span class="sxs-lookup"><span data-stu-id="c91ff-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printdocument-uploaddata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c91ff-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c91ff-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printdocument-uploaddata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c91ff-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c91ff-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printdocument-uploaddata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c91ff-151">Java</span><span class="sxs-lookup"><span data-stu-id="c91ff-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printdocument-uploaddata-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c91ff-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="c91ff-152">Response</span></span>

<span data-ttu-id="c91ff-153">Um ou mais segmentos ausentes:</span><span class="sxs-lookup"><span data-stu-id="c91ff-153">One or more segments missing:</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printDocument"
} -->
```http
HTTP/1.1 202 Accepted
```

<span data-ttu-id="c91ff-154">Todos os segmentos recebidos:</span><span class="sxs-lookup"><span data-stu-id="c91ff-154">All segments received:</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printDocument"
} -->
```http
HTTP/1.1 201 Created
```


