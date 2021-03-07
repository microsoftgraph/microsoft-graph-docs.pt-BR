---
title: 'printDocument: createUploadSession'
description: Crie uma sessão de carregamento para carregar de forma iterativa intervalos de arquivo binário de printDocument.
localization_priority: Normal
author: nilakhan
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 9de1372e4c4e9bb6819c06a563eda6763a407d0e
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517027"
---
# <a name="printdocument-createuploadsession"></a><span data-ttu-id="98dca-103">printDocument: createUploadSession</span><span class="sxs-lookup"><span data-stu-id="98dca-103">printDocument: createUploadSession</span></span>
<span data-ttu-id="98dca-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98dca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="98dca-105">Crie uma sessão de carregamento que permita que um aplicativo carregue de forma iterativa intervalos de um arquivo binário vinculado ao documento de impressão.</span><span class="sxs-lookup"><span data-stu-id="98dca-105">Create an upload session that allows an app to iteratively upload ranges of a binary file linked to the print document.</span></span>

<span data-ttu-id="98dca-106">Como parte da resposta, essa ação retorna uma URL de carregamento que pode ser usada em consultas `PUT` sequenciais subsequentes.</span><span class="sxs-lookup"><span data-stu-id="98dca-106">As part of the response, this action returns an upload URL that can be used in subsequent sequential `PUT` queries.</span></span> <span data-ttu-id="98dca-107">Os headers de solicitação para cada operação podem ser usados para especificar o intervalo exato de `PUT` bytes a serem carregados.</span><span class="sxs-lookup"><span data-stu-id="98dca-107">Request headers for each `PUT` operation can be used to specify the exact range of bytes to be uploaded.</span></span> <span data-ttu-id="98dca-108">Isso permite que a transferência seja retomada, caso a conexão de rede seja largada durante o carregamento.</span><span class="sxs-lookup"><span data-stu-id="98dca-108">This allows transfer to be resumed, in case the network connection is dropped during upload.</span></span> 

## <a name="permissions"></a><span data-ttu-id="98dca-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="98dca-109">Permissions</span></span>
<span data-ttu-id="98dca-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98dca-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="98dca-112">Além das permissões a seguir, o usuário ou locatário do aplicativo deve ter uma [](printer-get.md) assinatura de Impressão Universal ativa e ter uma permissão que conceda Obter impressora ou Obter acesso a [PrinterShare,](printershare-get.md) dependendo se a impressora ou impressoraShare está sendo usada.</span><span class="sxs-lookup"><span data-stu-id="98dca-112">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) or [Get printerShare](printershare-get.md) access depending upon whether printer or printerShare is being used.</span></span>

| <span data-ttu-id="98dca-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="98dca-113">Permission type</span></span>                        | <span data-ttu-id="98dca-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="98dca-114">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="98dca-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="98dca-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="98dca-116">PrintJob.Create, PrintJob.ReadWrite, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98dca-116">PrintJob.Create, PrintJob.ReadWrite, PrintJob.ReadWrite.All</span></span> |
| <span data-ttu-id="98dca-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="98dca-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98dca-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="98dca-118">Not Supported.</span></span> |
| <span data-ttu-id="98dca-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="98dca-119">Application</span></span>                            | <span data-ttu-id="98dca-120">PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98dca-120">PrintJob.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="98dca-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="98dca-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

<span data-ttu-id="98dca-122">Para criar uma sessão de carregamento usando **impressora**:</span><span class="sxs-lookup"><span data-stu-id="98dca-122">To create an upload session using **printer**:</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/documents/{id}/createUploadSession
```

<span data-ttu-id="98dca-123">Para criar uma sessão de carregamento usando **printerShare**:</span><span class="sxs-lookup"><span data-stu-id="98dca-123">To create an upload session using **printerShare**:</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST /print/shares/{id}/jobs/{id}/documents/{id}/createUploadSession
```

## <a name="request-headers"></a><span data-ttu-id="98dca-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="98dca-124">Request headers</span></span>
|<span data-ttu-id="98dca-125">Nome</span><span class="sxs-lookup"><span data-stu-id="98dca-125">Name</span></span>|<span data-ttu-id="98dca-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="98dca-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="98dca-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="98dca-127">Authorization</span></span>|<span data-ttu-id="98dca-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="98dca-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="98dca-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="98dca-130">Content-Type</span></span>|<span data-ttu-id="98dca-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="98dca-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="98dca-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="98dca-133">Request body</span></span>
<span data-ttu-id="98dca-134">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="98dca-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="98dca-135">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="98dca-135">Parameter</span></span>    | <span data-ttu-id="98dca-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="98dca-136">Type</span></span>        | <span data-ttu-id="98dca-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="98dca-137">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="98dca-138">propriedades</span><span class="sxs-lookup"><span data-stu-id="98dca-138">properties</span></span>|[<span data-ttu-id="98dca-139">printDocumentUploadProperties</span><span class="sxs-lookup"><span data-stu-id="98dca-139">printDocumentUploadProperties</span></span>](../resources/printDocumentUploadProperties.md)|<span data-ttu-id="98dca-140">Representa propriedades do arquivo binário a ser carregado.</span><span class="sxs-lookup"><span data-stu-id="98dca-140">Represents properties of the binary file to be uploaded.</span></span>|

<span data-ttu-id="98dca-141">O valor da **propriedade contentType** no corpo da solicitação deve ser suportado pela impressora/printerShare.</span><span class="sxs-lookup"><span data-stu-id="98dca-141">The value of the **contentType** property in the request body should be supported by the printer/printerShare.</span></span> <span data-ttu-id="98dca-142">Você pode obter os tipos de conteúdo com suporte ao obter [printerCapabilities](../resources/printercapabilities.md) da impressora/printerShare.</span><span class="sxs-lookup"><span data-stu-id="98dca-142">You can get the supported content types by getting [printerCapabilities](../resources/printercapabilities.md) of the printer/printerShare.</span></span> 

<span data-ttu-id="98dca-143">Para **conversão de OXPS para PDF,** você precisa passar `application/oxps` como contentType para printer/printerShare que oferece suporte `application/pdf` a .</span><span class="sxs-lookup"><span data-stu-id="98dca-143">For **OXPS to PDF** conversion, you need to pass `application/oxps` as contentType for printer/printerShare that supports `application/pdf`.</span></span> <span data-ttu-id="98dca-144">Impressão Universal converte **OXPS em PDF**, quando **todas** as seguintes condições são atendidas:</span><span class="sxs-lookup"><span data-stu-id="98dca-144">Universal Print converts **OXPS to PDF**, when **all** the following conditions are met:</span></span> 
1.  <span data-ttu-id="98dca-145">O compartilhamento de impressora/impressora é `application/pdf` compatível **com printerCapabilities**.</span><span class="sxs-lookup"><span data-stu-id="98dca-145">The printer/printer share supports `application/pdf` in **printerCapabilities**.</span></span> 
2.  <span data-ttu-id="98dca-146">O compartilhamento de impressora/impressora NÃO é `application/oxps` suportado em **printerCapabilities**.</span><span class="sxs-lookup"><span data-stu-id="98dca-146">The printer/printer share does NOT support `application/oxps` in **printerCapabilities**.</span></span> 
3.  <span data-ttu-id="98dca-147">O valor da **propriedade contentType** no corpo da solicitação é `application/oxps` .</span><span class="sxs-lookup"><span data-stu-id="98dca-147">The value for the **contentType** property in the request body is `application/oxps`.</span></span>

## <a name="response"></a><span data-ttu-id="98dca-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="98dca-148">Response</span></span>

<span data-ttu-id="98dca-149">Se tiver êxito, este método retornará um código de resposta e um `200 OK` novo [objeto uploadSession](../resources/uploadsession.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="98dca-149">If successful, this method returns a `200 OK` response code and a new [uploadSession](../resources/uploadsession.md) object in the response body.</span></span>

><span data-ttu-id="98dca-150">**Observação**: a **propriedade uploadUrl** retornada como parte do objeto de resposta **uploadSession** é uma URL opaca para consultas subsequentes para carregar intervalos de `PUT` byte do arquivo.</span><span class="sxs-lookup"><span data-stu-id="98dca-150">**Note**: The **uploadUrl** property returned as part of the **uploadSession** response object is an opaque URL for subsequent `PUT` queries to upload byte ranges of the file.</span></span> <span data-ttu-id="98dca-151">Ele contém o token de auth apropriado para consultas `PUT` subsequentes que expiram por **expirationDateTime**.</span><span class="sxs-lookup"><span data-stu-id="98dca-151">It contains the appropriate auth token for subsequent `PUT` queries that expire by **expirationDateTime**.</span></span> <span data-ttu-id="98dca-152">Não altere essa URL.</span><span class="sxs-lookup"><span data-stu-id="98dca-152">Do not change this URL.</span></span>

## <a name="examples"></a><span data-ttu-id="98dca-153">Exemplos</span><span class="sxs-lookup"><span data-stu-id="98dca-153">Examples</span></span>

<span data-ttu-id="98dca-154">O exemplo a seguir mostra como criar uma sessão de carregamento que você pode usar nas operações subsequentes de carregamento de arquivo para o printDocument especificado.</span><span class="sxs-lookup"><span data-stu-id="98dca-154">The following example shows how to create an upload session that you can use in subsequent file upload operations to the specified printDocument.</span></span>

### <a name="request"></a><span data-ttu-id="98dca-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="98dca-155">Request</span></span>
<!-- {
  "blockType": "request"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/printers/{printerId}/jobs/{printJobId}/documents/{printDocumentId}/createUploadSession
Content-Type: application/json
Content-length: 96

{
  "properties": {
    "documentName": "TestFile.pdf",
    "contentType": "application/pdf", 
    "size": 4533322
  }
}
```


### <a name="response"></a><span data-ttu-id="98dca-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="98dca-156">Response</span></span>
<span data-ttu-id="98dca-157">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="98dca-157">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.uploadSession"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.uploadSession",
    "uploadUrl": "https://print.print.microsoft.com/uploadSessions/5400be13-5a4e-4c20-be70-90c85bfe5d6e?tempauthtoken={token}",
    "expirationDateTime": "2020-10-25T02:19:38.1694207Z",
    "nextExpectedRanges": [
        "0-4533321"
    ]
}
```

