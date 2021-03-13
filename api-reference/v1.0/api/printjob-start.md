---
title: 'printJob: start'
description: Envia o trabalho de impressão para a impressora ou printerShare associada. Ele será impresso depois que quaisquer trabalhos pendentes existentes são concluídos, cancelados ou cancelados.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: dd264c395538ee3d77fe22829edca27a6d7ad4b1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775917"
---
# <a name="printjob-start"></a><span data-ttu-id="40d1a-104">printJob: start</span><span class="sxs-lookup"><span data-stu-id="40d1a-104">printJob: start</span></span>
<span data-ttu-id="40d1a-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40d1a-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="40d1a-106">Envia o trabalho de impressão para a impressora [associada](../resources/printer.md) ou [printerShare](../resources/printershare.md).</span><span class="sxs-lookup"><span data-stu-id="40d1a-106">Submits the print job to the associated [printer](../resources/printer.md) or [printerShare](../resources/printershare.md).</span></span> <span data-ttu-id="40d1a-107">Ele será impresso depois que quaisquer trabalhos pendentes existentes **são** concluídos, abortados ou cancelados.</span><span class="sxs-lookup"><span data-stu-id="40d1a-107">It will be printed after any existing pending **jobs** are completed, aborted, or canceled.</span></span>

## <a name="permissions"></a><span data-ttu-id="40d1a-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="40d1a-108">Permissions</span></span>
<span data-ttu-id="40d1a-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40d1a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="40d1a-111">Além das permissões a seguir, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa e ter uma permissão que conceda [Obter](printer-get.md) impressora ou [Obter printerShare,](printershare-get.md) dependendo se a impressora ou impressoraShare está sendo usada.</span><span class="sxs-lookup"><span data-stu-id="40d1a-111">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) or [Get printerShare](printershare-get.md) depending upon whether printer or printerShare is being used.</span></span>

|<span data-ttu-id="40d1a-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="40d1a-112">Permission type</span></span> | <span data-ttu-id="40d1a-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="40d1a-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="40d1a-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="40d1a-114">Delegated (work or school account)</span></span>| <span data-ttu-id="40d1a-115">PrintJob.Create, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40d1a-115">PrintJob.Create, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="40d1a-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="40d1a-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40d1a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="40d1a-117">Not Supported.</span></span>|
|<span data-ttu-id="40d1a-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="40d1a-118">Application</span></span>| <span data-ttu-id="40d1a-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="40d1a-119">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="40d1a-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="40d1a-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/shares/{printerShareId}/jobs/{printJobId}/start
```

## <a name="request-headers"></a><span data-ttu-id="40d1a-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="40d1a-121">Request headers</span></span>
|<span data-ttu-id="40d1a-122">Nome</span><span class="sxs-lookup"><span data-stu-id="40d1a-122">Name</span></span>|<span data-ttu-id="40d1a-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="40d1a-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="40d1a-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="40d1a-124">Authorization</span></span>|<span data-ttu-id="40d1a-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="40d1a-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="40d1a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="40d1a-127">Request body</span></span>
<span data-ttu-id="40d1a-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="40d1a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40d1a-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="40d1a-129">Response</span></span>
<span data-ttu-id="40d1a-130">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [printJobStatus](../resources/printjobstatus.md) no corpo.</span><span class="sxs-lookup"><span data-stu-id="40d1a-130">If successful, this method returns a `200 OK` response code and a [printJobStatus](../resources/printjobstatus.md) object in the body.</span></span>

## <a name="examples"></a><span data-ttu-id="40d1a-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="40d1a-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="40d1a-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="40d1a-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="40d1a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="40d1a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printjob_start"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/shares/{printerShareId}/jobs/{printJobId}/start
```
# <a name="c"></a>[<span data-ttu-id="40d1a-134">C#</span><span class="sxs-lookup"><span data-stu-id="40d1a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printjob-start-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="40d1a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="40d1a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printjob-start-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="40d1a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="40d1a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printjob-start-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="40d1a-137">Java</span><span class="sxs-lookup"><span data-stu-id="40d1a-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printjob-start-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="40d1a-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="40d1a-138">Response</span></span>
<span data-ttu-id="40d1a-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="40d1a-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJobStatus"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "state": "processing",
    "description": "The print job is currently being processed.",
    "isAcquiredByPrinter": false,
    "details": ["interpreting"]
}
```

