---
title: Get printJob
description: Recupere as propriedades e as relações de um trabalho de impressão.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 976624807ab6cbf8a104790665c481e3f54f9750
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776001"
---
# <a name="get-printjob"></a><span data-ttu-id="e19aa-103">Get printJob</span><span class="sxs-lookup"><span data-stu-id="e19aa-103">Get printJob</span></span>
<span data-ttu-id="e19aa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e19aa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="e19aa-105">Recupere as propriedades e as relações de um trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="e19aa-105">Retrieve the properties and relationships of a print job.</span></span>

## <a name="permissions"></a><span data-ttu-id="e19aa-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="e19aa-106">Permissions</span></span>
<span data-ttu-id="e19aa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e19aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="e19aa-109">Além das permissões a seguir, o usuário ou locatário do aplicativo deve ter uma [](printer-get.md) assinatura de Impressão Universal ativa e ter uma permissão que conceda Obter impressora ou Obter acesso a [PrinterShare,](printershare-get.md) dependendo se a impressora ou impressoraShare está sendo usada.</span><span class="sxs-lookup"><span data-stu-id="e19aa-109">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) or [Get printerShare](printershare-get.md) access depending upon whether printer or printerShare is being used.</span></span>

|<span data-ttu-id="e19aa-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e19aa-110">Permission type</span></span> | <span data-ttu-id="e19aa-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e19aa-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="e19aa-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e19aa-112">Delegated (work or school account)</span></span>| <span data-ttu-id="e19aa-113">PrintJob.ReadBasic, PrintJob.Read, PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e19aa-113">PrintJob.ReadBasic, PrintJob.Read, PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="e19aa-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e19aa-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e19aa-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e19aa-115">Not Supported.</span></span>|
|<span data-ttu-id="e19aa-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e19aa-116">Application</span></span>| <span data-ttu-id="e19aa-117">PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e19aa-117">PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e19aa-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e19aa-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="e19aa-119">Para obter um trabalho de uma impressora:</span><span class="sxs-lookup"><span data-stu-id="e19aa-119">To get a job from a printer:</span></span>
```http
GET /print/printers/{id}/jobs/{id}
```

<span data-ttu-id="e19aa-120">Para obter um trabalho de um compartilhamento de impressora:</span><span class="sxs-lookup"><span data-stu-id="e19aa-120">To get a job from a printer share:</span></span>
```http
GET /print/shares/{id}/jobs/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e19aa-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e19aa-121">Optional query parameters</span></span>
<span data-ttu-id="e19aa-122">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e19aa-122">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="e19aa-123">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="e19aa-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e19aa-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e19aa-124">Request headers</span></span>
|<span data-ttu-id="e19aa-125">Nome</span><span class="sxs-lookup"><span data-stu-id="e19aa-125">Name</span></span>|<span data-ttu-id="e19aa-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="e19aa-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e19aa-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="e19aa-127">Authorization</span></span>|<span data-ttu-id="e19aa-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e19aa-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e19aa-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e19aa-130">Request body</span></span>
<span data-ttu-id="e19aa-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e19aa-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e19aa-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="e19aa-132">Response</span></span>

<span data-ttu-id="e19aa-133">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [printJob](../resources/printjob.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e19aa-133">If successful, this method returns a `200 OK` response code and a [printJob](../resources/printjob.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e19aa-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e19aa-134">Examples</span></span>

### <a name="example-1-get-print-job"></a><span data-ttu-id="e19aa-135">Exemplo 1: Obter trabalho de impressão</span><span class="sxs-lookup"><span data-stu-id="e19aa-135">Example 1: Get print job</span></span>

#### <a name="request"></a><span data-ttu-id="e19aa-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e19aa-136">Request</span></span>
<span data-ttu-id="e19aa-137">A seguir, um exemplo de uma solicitação para obter metadados para um trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="e19aa-137">The following is an example of a request to get metadata for a print job.</span></span>


# <a name="http"></a>[<span data-ttu-id="e19aa-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="e19aa-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printjob"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/print/printers/{printerId}/jobs/{printJobId}
```
# <a name="c"></a>[<span data-ttu-id="e19aa-139">C#</span><span class="sxs-lookup"><span data-stu-id="e19aa-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printjob-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e19aa-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e19aa-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printjob-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e19aa-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e19aa-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printjob-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e19aa-142">Java</span><span class="sxs-lookup"><span data-stu-id="e19aa-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printjob-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e19aa-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="e19aa-143">Response</span></span>
<span data-ttu-id="e19aa-144">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e19aa-144">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/printers('c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb')/jobs/$entity",
  "id": "5182",
  "createdDateTime": "2020-02-04T00:00:00.0000000Z",
  "createdBy": {    
  },
  "configuration": {    
  },
  "status": {
    "state": "completed",
    "description": "The print job has completed successfully and no further processing will take place.",
    "details": [      
    ],
    "isAcquiredByPrinter": true
  },
  "redirectedTo": null,
  "redirectedFrom": null,
  "isFetchable": false
}
```

### <a name="example-2-get-print-job-with-task-list"></a><span data-ttu-id="e19aa-145">Exemplo 2: Obter trabalho de impressão com lista de tarefas</span><span class="sxs-lookup"><span data-stu-id="e19aa-145">Example 2: Get print job with task list</span></span>

#### <a name="request"></a><span data-ttu-id="e19aa-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e19aa-146">Request</span></span>
<span data-ttu-id="e19aa-147">A seguir está uma solicitação para [](../resources/printtask.md) obter um trabalho de impressão e todas as tarefas que estão sendo executadas ou executadas em relação a ele.</span><span class="sxs-lookup"><span data-stu-id="e19aa-147">The following is a request to get a print job and any [tasks](../resources/printtask.md) that are executing, or have executed, against it.</span></span>


# <a name="http"></a>[<span data-ttu-id="e19aa-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="e19aa-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printjob_withtasks"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/print/printers/{printerId}/jobs/{printJobId}?$expand=tasks
```
# <a name="c"></a>[<span data-ttu-id="e19aa-149">C#</span><span class="sxs-lookup"><span data-stu-id="e19aa-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printjob-withtasks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e19aa-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e19aa-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printjob-withtasks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e19aa-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e19aa-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printjob-withtasks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e19aa-152">Java</span><span class="sxs-lookup"><span data-stu-id="e19aa-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printjob-withtasks-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e19aa-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="e19aa-153">Response</span></span>
<span data-ttu-id="e19aa-154">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e19aa-154">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/printers('c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb')/jobs/$entity",
  "id": "5182",
  "createdDateTime": "2020-02-04T00:00:00.0000000Z",
  "createdBy": {    
  },
  "configuration": {    
  },
  "status": {
    "state": "completed",
    "description": "The print job has completed successfully and no further processing will take place.",
    "details": [      
    ],
    "isAcquiredByPrinter": true
  },
  "redirectedTo": null,
  "redirectedFrom": null,
  "isFetchable": false,
  "tasks": [
    {
      "id": "d036638b-1272-4bba-9227-732463823ed3",
      "parentUrl": "https://graph.microsoft.com/v1.0/print/printers/c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb/jobs/5182",
      "status": {
        "state": "processing",
        "description": "The task is being processed."
      }
    }
  ]
}
```

### <a name="example-3-get-a-print-job-and-its-associated-document-data"></a><span data-ttu-id="e19aa-155">Exemplo 3: Obter um trabalho de impressão e seus dados de documento associados</span><span class="sxs-lookup"><span data-stu-id="e19aa-155">Example 3: Get a print job and its associated document data</span></span>

#### <a name="request"></a><span data-ttu-id="e19aa-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e19aa-156">Request</span></span>
<span data-ttu-id="e19aa-157">A seguir, um exemplo de uma solicitação para obter um trabalho de impressão e seus dados de documento associados.</span><span class="sxs-lookup"><span data-stu-id="e19aa-157">The following is an example of a request to get a print job and its associated document data.</span></span>


# <a name="http"></a>[<span data-ttu-id="e19aa-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="e19aa-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printjob_withdocumentdata"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/print/printers/{printerId}/jobs/{printJobId}?$expand=documents
```
# <a name="c"></a>[<span data-ttu-id="e19aa-159">C#</span><span class="sxs-lookup"><span data-stu-id="e19aa-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printjob-withdocumentdata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e19aa-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e19aa-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printjob-withdocumentdata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e19aa-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e19aa-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printjob-withdocumentdata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e19aa-162">Java</span><span class="sxs-lookup"><span data-stu-id="e19aa-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printjob-withdocumentdata-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e19aa-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="e19aa-163">Response</span></span>
<span data-ttu-id="e19aa-164">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e19aa-164">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/printers('c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb')/jobs/$entity",
  "id": "5182",
  "createdDateTime": "2020-02-04T00:00:00.0000000Z",
  "createdBy": {    
  },
  "configuration": {    
  },
  "status": {
    "state": "completed",
    "description": "The print job has completed successfully and no further processing will take place.",
    "details": [      
    ],
    "isAcquiredByPrinter": true
  },
  "redirectedTo": null,
  "redirectedFrom": null,
  "isFetchable": false,
  "documents@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/printers('c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb')/jobs('5182')/documents",
  "documents": [
    {
      "id": "ca96c367-c3ad-478a-bbce-fbd1cd856e73",
      "displayName": "",
      "contentType": "application/oxps",
      "size": 276604
    }
  ]
}
```
