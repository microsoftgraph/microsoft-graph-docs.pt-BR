---
title: Get printJob
description: Recupere as propriedades e os relacionamentos de um trabalho de impressão.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 4a9c1b8f2fc5688f896b5fd6885926e8432e67b2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48035453"
---
# <a name="get-printjob"></a><span data-ttu-id="4ccbd-103">Get printJob</span><span class="sxs-lookup"><span data-stu-id="4ccbd-103">Get printJob</span></span>

<span data-ttu-id="4ccbd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ccbd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ccbd-105">Recupere as propriedades e os relacionamentos de um trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="4ccbd-105">Retrieve the properties and relationships of a print job.</span></span>

## <a name="permissions"></a><span data-ttu-id="4ccbd-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4ccbd-106">Permissions</span></span>
<span data-ttu-id="4ccbd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ccbd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="4ccbd-109">Além das permissões a seguir, o locatário do usuário ou do aplicativo deve ter uma assinatura universal de impressão ativa e ter uma permissão que conceda obter acesso à [impressora](printer-get.md) .</span><span class="sxs-lookup"><span data-stu-id="4ccbd-109">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) access.</span></span>

|<span data-ttu-id="4ccbd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4ccbd-110">Permission type</span></span> | <span data-ttu-id="4ccbd-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4ccbd-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="4ccbd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4ccbd-112">Delegated (work or school account)</span></span>| <span data-ttu-id="4ccbd-113">PrintJob. ReadBasic, PrintJob. Read, PrintJob. ReadBasic. All, PrintJob. Read. All, PrintJob. ReadWriteBasic, PrintJob. ReadWrite, PrintJob. ReadWriteBasic. All, PrintJob. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="4ccbd-113">PrintJob.ReadBasic, PrintJob.Read, PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="4ccbd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4ccbd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ccbd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4ccbd-115">Not Supported.</span></span>|
|<span data-ttu-id="4ccbd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4ccbd-116">Application</span></span>| <span data-ttu-id="4ccbd-117">PrintJob. ReadBasic. All, PrintJob. Read. All, PrintJob. ReadWriteBasic. All, PrintJob. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="4ccbd-117">PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4ccbd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4ccbd-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/jobs/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4ccbd-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4ccbd-119">Optional query parameters</span></span>
<span data-ttu-id="4ccbd-120">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4ccbd-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="4ccbd-121">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="4ccbd-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="4ccbd-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4ccbd-122">Request headers</span></span>
| <span data-ttu-id="4ccbd-123">Nome</span><span class="sxs-lookup"><span data-stu-id="4ccbd-123">Name</span></span>      |<span data-ttu-id="4ccbd-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ccbd-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4ccbd-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="4ccbd-125">Authorization</span></span> | <span data-ttu-id="4ccbd-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4ccbd-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4ccbd-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4ccbd-128">Request body</span></span>
<span data-ttu-id="4ccbd-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4ccbd-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="4ccbd-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ccbd-130">Response</span></span>
<span data-ttu-id="4ccbd-131">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [printJob](../resources/printjob.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4ccbd-131">If successful, this method returns a `200 OK` response code and a [printJob](../resources/printjob.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="4ccbd-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4ccbd-132">Examples</span></span>

### <a name="example-1-get-print-job"></a><span data-ttu-id="4ccbd-133">Exemplo 1: obter trabalho de impressão</span><span class="sxs-lookup"><span data-stu-id="4ccbd-133">Example 1: Get print job</span></span>

#### <a name="request"></a><span data-ttu-id="4ccbd-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4ccbd-134">Request</span></span>
<span data-ttu-id="4ccbd-135">Veja a seguir um exemplo de uma solicitação para obter metadados para um trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="4ccbd-135">The following is an example of a request to get metadata for a print job.</span></span>

# <a name="http"></a>[<span data-ttu-id="4ccbd-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="4ccbd-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printjob"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb/jobs/5182
```
# <a name="c"></a>[<span data-ttu-id="4ccbd-137">C#</span><span class="sxs-lookup"><span data-stu-id="4ccbd-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printjob-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4ccbd-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4ccbd-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printjob-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4ccbd-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4ccbd-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printjob-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="4ccbd-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ccbd-140">Response</span></span>
<span data-ttu-id="4ccbd-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4ccbd-141">The following is an example of the response.</span></span>
><span data-ttu-id="4ccbd-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4ccbd-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 408

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers('c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb')/jobs/$entity",
  "id": "5182",
  "createdDateTime": "2020-02-04T00:00:00.0000000Z",
  "createdBy": {},
  "status": {
    "processingState": "completed",
    "processingStateDescription": "The print job has completed successfully and no further processing will take place."
  }
}
```

### <a name="example-2-get-print-job-with-task-list"></a><span data-ttu-id="4ccbd-144">Exemplo 2: obter trabalho de impressão com a lista de tarefas</span><span class="sxs-lookup"><span data-stu-id="4ccbd-144">Example 2: Get print job with task list</span></span>

#### <a name="request"></a><span data-ttu-id="4ccbd-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4ccbd-145">Request</span></span>
<span data-ttu-id="4ccbd-146">Veja a seguir uma solicitação para obter um trabalho de impressão e todas [as tarefas](../resources/printtask.md) que estão em execução ou foram executadas nele.</span><span class="sxs-lookup"><span data-stu-id="4ccbd-146">The following is a request to get a print job and any [tasks](../resources/printtask.md) that are executing, or have executed, against it.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_printjob_withtasks"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb/jobs/5182?$expand=tasks
```

#### <a name="response"></a><span data-ttu-id="4ccbd-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ccbd-147">Response</span></span>
<span data-ttu-id="4ccbd-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4ccbd-148">The following is an example of the response.</span></span>
><span data-ttu-id="4ccbd-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4ccbd-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 774

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers('c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb')/jobs(tasks())/$entity",
  "id": "5182",
  "createdDateTime": "2020-06-30T17:18:52.3930472Z",
  "createdBy": {
    "id": "",
    "displayName": "",
    "userPrincipalName": ""
  },
  "status": {
    "processingState": "pendingHeld",
    "processingStateDescription": "The job is not a candidate for processing yet."
  },
  "tasks": [
    {
      "id": "d036638b-1272-4bba-9227-732463823ed3",
      "parentUrl": "https://graph.microsoft.com/beta/print/printers/c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb/jobs/5182",
      "status": {
        "state": "processing",
        "description": "The task is being processed."
      }
    }
  ]
}
```

### <a name="example-3-get-a-print-job-and-its-associated-document-data"></a><span data-ttu-id="4ccbd-151">Exemplo 3: obter um trabalho de impressão e seus dados de documento associados</span><span class="sxs-lookup"><span data-stu-id="4ccbd-151">Example 3: Get a print job and its associated document data</span></span>

#### <a name="request"></a><span data-ttu-id="4ccbd-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4ccbd-152">Request</span></span>
<span data-ttu-id="4ccbd-153">Veja a seguir um exemplo de uma solicitação para obter um trabalho de impressão e seus dados de documento associados.</span><span class="sxs-lookup"><span data-stu-id="4ccbd-153">The following is an example of a request to get a print job and its associated document data.</span></span>
# <a name="http"></a>[<span data-ttu-id="4ccbd-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="4ccbd-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printjob_withdocumentdata"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/86b6d420-7e6b-4797-a05c-af4e56cd81bd/jobs/31216?$expand=documents
```
# <a name="c"></a>[<span data-ttu-id="4ccbd-155">C#</span><span class="sxs-lookup"><span data-stu-id="4ccbd-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printjob-withdocumentdata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4ccbd-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4ccbd-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printjob-withdocumentdata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4ccbd-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4ccbd-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printjob-withdocumentdata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="4ccbd-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ccbd-158">Response</span></span>
<span data-ttu-id="4ccbd-159">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4ccbd-159">The following is an example of the response.</span></span>
><span data-ttu-id="4ccbd-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4ccbd-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1688

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers('86b6d420-7e6b-4797-a05c-af4e56cd81bd')/jobs(documents())/$entity",
  "id": "31216",
  "createdDateTime": "2020-06-26T04:20:06.5715544Z",
  "createdBy": {
    "id": "",
    "displayName": "",
    "ipAddress": null,
    "userPrincipalName": "",
    "oDataType": null
  },
  "status": {
  "processingState": "aborted",
  "processingStateDescription": "The print job has been aborted by a user or the printer and no further processing will take place."
  },
  "documents@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers('86b6d420-7e6b-4797-a05c-af4e56cd81bd')/jobs('31216')/documents",
  "documents": [
    {
      "id": "ca96c367-c3ad-478a-bbce-fbd1cd856e73",
      "displayName": "",
      "contentType": "application/oxps",
      "size": 276604,
      "configuration": {
        "quality": "medium",
        "dpi": 300,
        "feedDirection": null,
        "orientation": "landscape",
        "duplexMode": "oneSided",
        "copies": 2,
        "colorMode": "color",
        "inputBin": null,
        "outputBin": null,
        "mediaSize": null,
        "mediaType": null,
        "finishings": [],
        "pagesPerSheet": null,
        "multipageLayout": "clockwiseFromTopLeft",
        "collate": true,
        "scaling": null,
        "fitPdfToPage": null,
        "margin": null,
        "pageRanges": []
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get printJob",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


