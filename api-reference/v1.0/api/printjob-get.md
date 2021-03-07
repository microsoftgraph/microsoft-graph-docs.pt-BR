---
title: Get printJob
description: Recupere as propriedades e as relações de um trabalho de impressão.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: c97ffa869a14fbceedd0fc2e5b8f737792490d1c
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517021"
---
# <a name="get-printjob"></a><span data-ttu-id="8f49a-103">Get printJob</span><span class="sxs-lookup"><span data-stu-id="8f49a-103">Get printJob</span></span>
<span data-ttu-id="8f49a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f49a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="8f49a-105">Recupere as propriedades e as relações de um trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="8f49a-105">Retrieve the properties and relationships of a print job.</span></span>

## <a name="permissions"></a><span data-ttu-id="8f49a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8f49a-106">Permissions</span></span>
<span data-ttu-id="8f49a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f49a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="8f49a-109">Além das permissões a seguir, o usuário ou locatário do aplicativo deve ter uma [](printer-get.md) assinatura de Impressão Universal ativa e ter uma permissão que conceda Obter impressora ou Obter acesso a [PrinterShare,](printershare-get.md) dependendo se a impressora ou impressoraShare está sendo usada.</span><span class="sxs-lookup"><span data-stu-id="8f49a-109">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) or [Get printerShare](printershare-get.md) access depending upon whether printer or printerShare is being used.</span></span>

|<span data-ttu-id="8f49a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8f49a-110">Permission type</span></span> | <span data-ttu-id="8f49a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8f49a-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="8f49a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8f49a-112">Delegated (work or school account)</span></span>| <span data-ttu-id="8f49a-113">PrintJob.ReadBasic, PrintJob.Read, PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f49a-113">PrintJob.ReadBasic, PrintJob.Read, PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="8f49a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8f49a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f49a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8f49a-115">Not Supported.</span></span>|
|<span data-ttu-id="8f49a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8f49a-116">Application</span></span>| <span data-ttu-id="8f49a-117">PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f49a-117">PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8f49a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8f49a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="8f49a-119">Para obter um trabalho de uma impressora:</span><span class="sxs-lookup"><span data-stu-id="8f49a-119">To get a job from a printer:</span></span>
```http
GET /print/printers/{id}/jobs/{id}
```

<span data-ttu-id="8f49a-120">Para obter um trabalho de um compartilhamento de impressora:</span><span class="sxs-lookup"><span data-stu-id="8f49a-120">To get a job from a printer share:</span></span>
```http
GET /print/shares/{id}/jobs/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8f49a-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8f49a-121">Optional query parameters</span></span>
<span data-ttu-id="8f49a-122">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8f49a-122">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="8f49a-123">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="8f49a-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="8f49a-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8f49a-124">Request headers</span></span>
|<span data-ttu-id="8f49a-125">Nome</span><span class="sxs-lookup"><span data-stu-id="8f49a-125">Name</span></span>|<span data-ttu-id="8f49a-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f49a-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8f49a-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="8f49a-127">Authorization</span></span>|<span data-ttu-id="8f49a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8f49a-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f49a-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8f49a-130">Request body</span></span>
<span data-ttu-id="8f49a-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8f49a-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8f49a-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f49a-132">Response</span></span>

<span data-ttu-id="8f49a-133">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [printJob](../resources/printjob.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8f49a-133">If successful, this method returns a `200 OK` response code and a [printJob](../resources/printjob.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8f49a-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8f49a-134">Examples</span></span>

### <a name="example-1-get-print-job"></a><span data-ttu-id="8f49a-135">Exemplo 1: Obter trabalho de impressão</span><span class="sxs-lookup"><span data-stu-id="8f49a-135">Example 1: Get print job</span></span>

#### <a name="request"></a><span data-ttu-id="8f49a-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8f49a-136">Request</span></span>
<span data-ttu-id="8f49a-137">A seguir, um exemplo de uma solicitação para obter metadados para um trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="8f49a-137">The following is an example of a request to get metadata for a print job.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_printjob"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/print/printers/{printerId}/jobs/{printJobId}
```

#### <a name="response"></a><span data-ttu-id="8f49a-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f49a-138">Response</span></span>
<span data-ttu-id="8f49a-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8f49a-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2-get-print-job-with-task-list"></a><span data-ttu-id="8f49a-140">Exemplo 2: Obter trabalho de impressão com lista de tarefas</span><span class="sxs-lookup"><span data-stu-id="8f49a-140">Example 2: Get print job with task list</span></span>

#### <a name="request"></a><span data-ttu-id="8f49a-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8f49a-141">Request</span></span>
<span data-ttu-id="8f49a-142">A seguir está uma solicitação para [](../resources/printtask.md) obter um trabalho de impressão e todas as tarefas que estão sendo executadas ou executadas em relação a ele.</span><span class="sxs-lookup"><span data-stu-id="8f49a-142">The following is a request to get a print job and any [tasks](../resources/printtask.md) that are executing, or have executed, against it.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_printjob_withtasks"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/print/printers/{printerId}/jobs/{printJobId}?$expand=tasks
```

#### <a name="response"></a><span data-ttu-id="8f49a-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f49a-143">Response</span></span>
<span data-ttu-id="8f49a-144">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8f49a-144">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-3-get-a-print-job-and-its-associated-document-data"></a><span data-ttu-id="8f49a-145">Exemplo 3: Obter um trabalho de impressão e seus dados de documento associados</span><span class="sxs-lookup"><span data-stu-id="8f49a-145">Example 3: Get a print job and its associated document data</span></span>

#### <a name="request"></a><span data-ttu-id="8f49a-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8f49a-146">Request</span></span>
<span data-ttu-id="8f49a-147">A seguir, um exemplo de uma solicitação para obter um trabalho de impressão e seus dados de documento associados.</span><span class="sxs-lookup"><span data-stu-id="8f49a-147">The following is an example of a request to get a print job and its associated document data.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_printjob_withdocumentdata"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/print/printers/{printerId}/jobs/{printJobId}?$expand=documents
```

#### <a name="response"></a><span data-ttu-id="8f49a-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f49a-148">Response</span></span>
<span data-ttu-id="8f49a-149">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8f49a-149">**Note:** The response object shown here might be shortened for readability.</span></span>
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
