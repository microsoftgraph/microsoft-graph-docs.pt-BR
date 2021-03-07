---
title: 'printJob: start'
description: Envia o trabalho de impressão para a impressora ou printerShare associada. Ele será impresso depois que quaisquer trabalhos pendentes existentes são concluídos, cancelados ou cancelados.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 187e62e1de9f380f651433596b7d76fd91161c2c
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517017"
---
# <a name="printjob-start"></a><span data-ttu-id="e97de-104">printJob: start</span><span class="sxs-lookup"><span data-stu-id="e97de-104">printJob: start</span></span>
<span data-ttu-id="e97de-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e97de-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="e97de-106">Envia o trabalho de impressão para a impressora [associada](../resources/printer.md) ou [printerShare](../resources/printershare.md).</span><span class="sxs-lookup"><span data-stu-id="e97de-106">Submits the print job to the associated [printer](../resources/printer.md) or [printerShare](../resources/printershare.md).</span></span> <span data-ttu-id="e97de-107">Ele será impresso depois que quaisquer trabalhos pendentes existentes **são** concluídos, abortados ou cancelados.</span><span class="sxs-lookup"><span data-stu-id="e97de-107">It will be printed after any existing pending **jobs** are completed, aborted, or canceled.</span></span>

## <a name="permissions"></a><span data-ttu-id="e97de-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="e97de-108">Permissions</span></span>
<span data-ttu-id="e97de-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e97de-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="e97de-111">Além das permissões a seguir, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa e ter uma permissão que conceda [Obter](printer-get.md) impressora ou [Obter printerShare,](printershare-get.md) dependendo se a impressora ou impressoraShare está sendo usada.</span><span class="sxs-lookup"><span data-stu-id="e97de-111">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) or [Get printerShare](printershare-get.md) depending upon whether printer or printerShare is being used.</span></span>

|<span data-ttu-id="e97de-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e97de-112">Permission type</span></span> | <span data-ttu-id="e97de-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e97de-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="e97de-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e97de-114">Delegated (work or school account)</span></span>| <span data-ttu-id="e97de-115">PrintJob.Create, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e97de-115">PrintJob.Create, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="e97de-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e97de-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e97de-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e97de-117">Not Supported.</span></span>|
|<span data-ttu-id="e97de-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e97de-118">Application</span></span>| <span data-ttu-id="e97de-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e97de-119">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e97de-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e97de-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/shares/{printerShareId}/jobs/{printJobId}/start
```

## <a name="request-headers"></a><span data-ttu-id="e97de-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e97de-121">Request headers</span></span>
|<span data-ttu-id="e97de-122">Nome</span><span class="sxs-lookup"><span data-stu-id="e97de-122">Name</span></span>|<span data-ttu-id="e97de-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="e97de-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e97de-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e97de-124">Authorization</span></span>|<span data-ttu-id="e97de-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e97de-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e97de-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e97de-127">Request body</span></span>
<span data-ttu-id="e97de-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e97de-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e97de-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e97de-129">Response</span></span>
<span data-ttu-id="e97de-130">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [printJobStatus](../resources/printjobstatus.md) no corpo.</span><span class="sxs-lookup"><span data-stu-id="e97de-130">If successful, this method returns a `200 OK` response code and a [printJobStatus](../resources/printjobstatus.md) object in the body.</span></span>

## <a name="examples"></a><span data-ttu-id="e97de-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e97de-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e97de-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e97de-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "printjob_start"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/shares/{printerShareId}/jobs/{printJobId}/start
```

### <a name="response"></a><span data-ttu-id="e97de-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e97de-133">Response</span></span>
<span data-ttu-id="e97de-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e97de-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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

