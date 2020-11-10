---
title: Get printJob
description: Recupere as propriedades e os relacionamentos de um trabalho de impressão.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: eba94363ccb030096f9ee13a303a159c9383cb33
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968333"
---
# <a name="get-printjob"></a><span data-ttu-id="460c7-103">Get printJob</span><span class="sxs-lookup"><span data-stu-id="460c7-103">Get printJob</span></span>

<span data-ttu-id="460c7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="460c7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="460c7-105">Recupere as propriedades e os relacionamentos de um trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="460c7-105">Retrieve the properties and relationships of a print job.</span></span>

## <a name="permissions"></a><span data-ttu-id="460c7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="460c7-106">Permissions</span></span>
<span data-ttu-id="460c7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="460c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="460c7-109">Além das permissões a seguir, o locatário do usuário ou do aplicativo deve ter uma assinatura de impressão universal ativa e ter uma permissão que conceda [obter impressora](printer-get.md) ou obter o acesso do [printerShare](printershare-get.md) , dependendo se a impressora ou o printerShare está sendo usado.</span><span class="sxs-lookup"><span data-stu-id="460c7-109">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) or [Get printerShare](printershare-get.md) access depending upon whether printer or printerShare is being used.</span></span>

|<span data-ttu-id="460c7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="460c7-110">Permission type</span></span> | <span data-ttu-id="460c7-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="460c7-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="460c7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="460c7-112">Delegated (work or school account)</span></span>| <span data-ttu-id="460c7-113">PrintJob. ReadBasic, PrintJob. Read, PrintJob. ReadBasic. All, PrintJob. Read. All, PrintJob. ReadWriteBasic, PrintJob. ReadWrite, PrintJob. ReadWriteBasic. All, PrintJob. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="460c7-113">PrintJob.ReadBasic, PrintJob.Read, PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="460c7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="460c7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="460c7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="460c7-115">Not Supported.</span></span>|
|<span data-ttu-id="460c7-116">Application</span><span class="sxs-lookup"><span data-stu-id="460c7-116">Application</span></span>| <span data-ttu-id="460c7-117">PrintJob. ReadBasic. All, PrintJob. Read. All, PrintJob. ReadWriteBasic. All, PrintJob. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="460c7-117">PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="460c7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="460c7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="460c7-119">Para obter um trabalho de uma impressora:</span><span class="sxs-lookup"><span data-stu-id="460c7-119">To get a job from a printer:</span></span>
```http
GET /print/printers/{id}/jobs/{id}
```

<span data-ttu-id="460c7-120">Para obter um trabalho de um compartilhamento de impressora:</span><span class="sxs-lookup"><span data-stu-id="460c7-120">To get a job from a printer share:</span></span>
```http
GET /print/shares/{id}/jobs/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="460c7-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="460c7-121">Optional query parameters</span></span>
<span data-ttu-id="460c7-122">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="460c7-122">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="460c7-123">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="460c7-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="460c7-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="460c7-124">Request headers</span></span>
| <span data-ttu-id="460c7-125">Nome</span><span class="sxs-lookup"><span data-stu-id="460c7-125">Name</span></span>      |<span data-ttu-id="460c7-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="460c7-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="460c7-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="460c7-127">Authorization</span></span> | <span data-ttu-id="460c7-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="460c7-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="460c7-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="460c7-130">Request body</span></span>
<span data-ttu-id="460c7-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="460c7-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="460c7-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="460c7-132">Response</span></span>
<span data-ttu-id="460c7-133">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [printJob](../resources/printjob.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="460c7-133">If successful, this method returns a `200 OK` response code and a [printJob](../resources/printjob.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="460c7-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="460c7-134">Examples</span></span>

### <a name="example-1-get-print-job"></a><span data-ttu-id="460c7-135">Exemplo 1: obter trabalho de impressão</span><span class="sxs-lookup"><span data-stu-id="460c7-135">Example 1: Get print job</span></span>

#### <a name="request"></a><span data-ttu-id="460c7-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="460c7-136">Request</span></span>
<span data-ttu-id="460c7-137">Veja a seguir um exemplo de uma solicitação para obter metadados para um trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="460c7-137">The following is an example of a request to get metadata for a print job.</span></span>

# <a name="http"></a>[<span data-ttu-id="460c7-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="460c7-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printjob"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb/jobs/5182
```
# <a name="c"></a>[<span data-ttu-id="460c7-139">C#</span><span class="sxs-lookup"><span data-stu-id="460c7-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printjob-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="460c7-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="460c7-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printjob-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="460c7-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="460c7-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printjob-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="460c7-142">Java</span><span class="sxs-lookup"><span data-stu-id="460c7-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printjob-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="460c7-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="460c7-143">Response</span></span>
<span data-ttu-id="460c7-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="460c7-144">The following is an example of the response.</span></span>
><span data-ttu-id="460c7-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="460c7-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

### <a name="example-2-get-print-job-with-task-list"></a><span data-ttu-id="460c7-147">Exemplo 2: obter trabalho de impressão com a lista de tarefas</span><span class="sxs-lookup"><span data-stu-id="460c7-147">Example 2: Get print job with task list</span></span>

#### <a name="request"></a><span data-ttu-id="460c7-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="460c7-148">Request</span></span>
<span data-ttu-id="460c7-149">Veja a seguir uma solicitação para obter um trabalho de impressão e todas [as tarefas](../resources/printtask.md) que estão em execução ou foram executadas nele.</span><span class="sxs-lookup"><span data-stu-id="460c7-149">The following is a request to get a print job and any [tasks](../resources/printtask.md) that are executing, or have executed, against it.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_printjob_withtasks"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb/jobs/5182?$expand=tasks
```

#### <a name="response"></a><span data-ttu-id="460c7-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="460c7-150">Response</span></span>
<span data-ttu-id="460c7-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="460c7-151">The following is an example of the response.</span></span>
><span data-ttu-id="460c7-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="460c7-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

### <a name="example-3-get-a-print-job-and-its-associated-document-data"></a><span data-ttu-id="460c7-154">Exemplo 3: obter um trabalho de impressão e seus dados de documento associados</span><span class="sxs-lookup"><span data-stu-id="460c7-154">Example 3: Get a print job and its associated document data</span></span>

#### <a name="request"></a><span data-ttu-id="460c7-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="460c7-155">Request</span></span>
<span data-ttu-id="460c7-156">Veja a seguir um exemplo de uma solicitação para obter um trabalho de impressão e seus dados de documento associados.</span><span class="sxs-lookup"><span data-stu-id="460c7-156">The following is an example of a request to get a print job and its associated document data.</span></span>
# <a name="http"></a>[<span data-ttu-id="460c7-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="460c7-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printjob_withdocumentdata"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/86b6d420-7e6b-4797-a05c-af4e56cd81bd/jobs/31216?$expand=documents
```
# <a name="c"></a>[<span data-ttu-id="460c7-158">C#</span><span class="sxs-lookup"><span data-stu-id="460c7-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printjob-withdocumentdata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="460c7-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="460c7-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printjob-withdocumentdata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="460c7-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="460c7-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printjob-withdocumentdata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="460c7-161">Java</span><span class="sxs-lookup"><span data-stu-id="460c7-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printjob-withdocumentdata-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="460c7-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="460c7-162">Response</span></span>
<span data-ttu-id="460c7-163">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="460c7-163">The following is an example of the response.</span></span>
><span data-ttu-id="460c7-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="460c7-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


