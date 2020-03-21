---
title: 'Documento de documentos: uploadData'
description: Carregar um único segmento binário do documento.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 7592de07f74aa6fb715a90b2becad57a0e14b194
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895577"
---
# <a name="printdocument-uploaddata"></a><span data-ttu-id="52cd0-103">Documento de documentos: uploadData</span><span class="sxs-lookup"><span data-stu-id="52cd0-103">printDocument: uploadData</span></span>

<span data-ttu-id="52cd0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52cd0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52cd0-105">Carregar um único segmento binário do **documento**.</span><span class="sxs-lookup"><span data-stu-id="52cd0-105">Upload a single binary segment of the **printDocument**.</span></span>

<span data-ttu-id="52cd0-106">É possível carregar o arquivo inteiro ou dividir o arquivo em vários intervalos de bytes, desde que nenhuma solicitação seja maior do que 1 MB.</span><span class="sxs-lookup"><span data-stu-id="52cd0-106">You can upload the entire file, or split the file into multiple byte ranges, as long as no request is larger than 1 MB.</span></span>

<span data-ttu-id="52cd0-107">Os segmentos do arquivo podem ser carregados em qualquer ordem e podem ser carregados em paralelo, com até quatro solicitações simultâneas.</span><span class="sxs-lookup"><span data-stu-id="52cd0-107">The segments of the file can be uploaded in any order and can be uploaded in parallel, with up to four concurrent requests.</span></span> <span data-ttu-id="52cd0-108">Quando todos os segmentos binários do documento são carregados, o arquivo binário é vinculado ao **printJob**.</span><span class="sxs-lookup"><span data-stu-id="52cd0-108">When all the binary segments of document are uploaded, the binary file is linked to the **printJob**.</span></span>

## <a name="permissions"></a><span data-ttu-id="52cd0-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="52cd0-109">Permissions</span></span>
<span data-ttu-id="52cd0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52cd0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="52cd0-112">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="52cd0-112">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="52cd0-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="52cd0-113">Permission type</span></span> | <span data-ttu-id="52cd0-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="52cd0-114">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="52cd0-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="52cd0-115">Delegated (work or school account)</span></span>| <span data-ttu-id="52cd0-116">Users. Read. All</span><span class="sxs-lookup"><span data-stu-id="52cd0-116">Users.Read.All</span></span> |
|<span data-ttu-id="52cd0-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="52cd0-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52cd0-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52cd0-118">Not Supported.</span></span>|
|<span data-ttu-id="52cd0-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="52cd0-119">Application</span></span>|<span data-ttu-id="52cd0-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52cd0-120">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="52cd0-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="52cd0-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/documents/{id}/uploadData
```
## <a name="request-headers"></a><span data-ttu-id="52cd0-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="52cd0-122">Request headers</span></span>
| <span data-ttu-id="52cd0-123">Nome</span><span class="sxs-lookup"><span data-stu-id="52cd0-123">Name</span></span>          | <span data-ttu-id="52cd0-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="52cd0-124">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="52cd0-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="52cd0-125">Authorization</span></span> | <span data-ttu-id="52cd0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="52cd0-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="52cd0-128">Intervalo</span><span class="sxs-lookup"><span data-stu-id="52cd0-128">Range</span></span> | <span data-ttu-id="52cd0-129">bytes = {startByteIndex}-{endByteIndex}</span><span class="sxs-lookup"><span data-stu-id="52cd0-129">bytes={startByteIndex}-{endByteIndex}‬</span></span>  |
| <span data-ttu-id="52cd0-130">Content-Length</span><span class="sxs-lookup"><span data-stu-id="52cd0-130">Content-Length</span></span> | <span data-ttu-id="52cd0-131">ContentLength</span><span class="sxs-lookup"><span data-stu-id="52cd0-131">{contentLength}‬</span></span>  |
| <span data-ttu-id="52cd0-132">Content-type</span><span class="sxs-lookup"><span data-stu-id="52cd0-132">Content-type</span></span>  | <span data-ttu-id="52cd0-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="52cd0-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="52cd0-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="52cd0-135">Request body</span></span>
<span data-ttu-id="52cd0-136">O corpo da solicitação é um blob binário contendo os bytes do documento que são especificados como um intervalo de bytes inclusivo `Range` no cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="52cd0-136">The request body is a binary blob containing the bytes of the document that are specified as an inclusive byte range in the `Range` header.</span></span> 

## <a name="response"></a><span data-ttu-id="52cd0-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="52cd0-137">Response</span></span>
<span data-ttu-id="52cd0-138">Se tiver êxito, este método retornará uma das seguintes respostas.</span><span class="sxs-lookup"><span data-stu-id="52cd0-138">If successful, this method returns one of the following responses.</span></span> <span data-ttu-id="52cd0-139">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="52cd0-139">It does not return anything in the response body.</span></span>

| <span data-ttu-id="52cd0-140">Condição</span><span class="sxs-lookup"><span data-stu-id="52cd0-140">Condition</span></span>     | <span data-ttu-id="52cd0-141">Código da resposta</span><span class="sxs-lookup"><span data-stu-id="52cd0-141">Response code</span></span> |
|:--------------|:--------------|
| <span data-ttu-id="52cd0-142">Um ou mais segmentos binários ainda precisam ser carregados</span><span class="sxs-lookup"><span data-stu-id="52cd0-142">One or more binary segments still need to be uploaded</span></span> | `202 Accepted` |
| <span data-ttu-id="52cd0-143">Todos os segmentos binários foram carregados com êxito</span><span class="sxs-lookup"><span data-stu-id="52cd0-143">All binary segments have been uploaded successfully</span></span> | `201 Created` |

## <a name="example"></a><span data-ttu-id="52cd0-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="52cd0-144">Example</span></span>
<span data-ttu-id="52cd0-145">O exemplo a seguir mostra como chamar essa API para carregar os primeiros 72797 bytes de um documento.</span><span class="sxs-lookup"><span data-stu-id="52cd0-145">The following example shows how to call this API to upload the first 72797 bytes of a document.</span></span>
##### <a name="request"></a><span data-ttu-id="52cd0-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="52cd0-146">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "printdocument-uploaddata"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/jobs/{id}/documents/{id}/uploadData
Range: bytes=0-72796
Content-Length: 72797
```
##### <a name="response"></a><span data-ttu-id="52cd0-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="52cd0-147">Response</span></span>

<span data-ttu-id="52cd0-148">Um ou mais segmentos ausentes:</span><span class="sxs-lookup"><span data-stu-id="52cd0-148">One or more segments missing:</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printDocument"
} -->
```http
HTTP/1.1 202 Accepted
```

<span data-ttu-id="52cd0-149">Todos os segmentos recebidos:</span><span class="sxs-lookup"><span data-stu-id="52cd0-149">All segments received:</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printDocument"
} -->
```http
HTTP/1.1 201 Created
```