---
title: 'printJob: start'
description: Envia o trabalho de impressão para a impressora ou printerShare associada. Ele será impresso depois que quaisquer trabalhos pendentes existentes são concluídos, cancelados ou cancelados.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 288e3b8cfcd1458f7d71c8fb43ae57ac97237e56
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049874"
---
# <a name="printjob-start"></a><span data-ttu-id="8f4b6-104">printJob: start</span><span class="sxs-lookup"><span data-stu-id="8f4b6-104">printJob: start</span></span>

<span data-ttu-id="8f4b6-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f4b6-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f4b6-106">Envia o trabalho de impressão para a impressora [associada](../resources/printer.md) ou [printerShare](../resources/printershare.md).</span><span class="sxs-lookup"><span data-stu-id="8f4b6-106">Submits the print job to the associated [printer](../resources/printer.md) or [printerShare](../resources/printershare.md).</span></span> <span data-ttu-id="8f4b6-107">Ele será impresso depois que quaisquer trabalhos pendentes existentes **são** concluídos, abortados ou cancelados.</span><span class="sxs-lookup"><span data-stu-id="8f4b6-107">It will be printed after any existing pending **jobs** are completed, aborted, or canceled.</span></span>

## <a name="permissions"></a><span data-ttu-id="8f4b6-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="8f4b6-108">Permissions</span></span>
<span data-ttu-id="8f4b6-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f4b6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="8f4b6-111">Além das permissões a seguir, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa e ter uma permissão que conceda [Obter](printer-get.md) impressora ou [Obter printerShare,](printershare-get.md) dependendo se a impressora ou impressoraShare está sendo usada.</span><span class="sxs-lookup"><span data-stu-id="8f4b6-111">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) or [Get printerShare](printershare-get.md) depending upon whether printer or printerShare is being used.</span></span>

|<span data-ttu-id="8f4b6-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8f4b6-112">Permission type</span></span> | <span data-ttu-id="8f4b6-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8f4b6-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="8f4b6-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8f4b6-114">Delegated (work or school account)</span></span>| <span data-ttu-id="8f4b6-115">PrintJob.Create, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f4b6-115">PrintJob.Create, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="8f4b6-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8f4b6-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f4b6-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8f4b6-117">Not Supported.</span></span>|
|<span data-ttu-id="8f4b6-118">Application</span><span class="sxs-lookup"><span data-stu-id="8f4b6-118">Application</span></span>| <span data-ttu-id="8f4b6-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8f4b6-119">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8f4b6-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8f4b6-120">HTTP request</span></span>
```http
POST /print/shares/{id}/jobs/{id}/start
```
## <a name="request-headers"></a><span data-ttu-id="8f4b6-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8f4b6-121">Request headers</span></span>
| <span data-ttu-id="8f4b6-122">Nome</span><span class="sxs-lookup"><span data-stu-id="8f4b6-122">Name</span></span>          | <span data-ttu-id="8f4b6-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f4b6-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8f4b6-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="8f4b6-124">Authorization</span></span> | <span data-ttu-id="8f4b6-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8f4b6-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8f4b6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8f4b6-127">Request body</span></span>

<span data-ttu-id="8f4b6-128">Não envie um corpo de solicitação para este método.</span><span class="sxs-lookup"><span data-stu-id="8f4b6-128">Do not submit a request body for this method.</span></span> 

## <a name="response"></a><span data-ttu-id="8f4b6-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f4b6-129">Response</span></span>
<span data-ttu-id="8f4b6-130">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [printJobStatus](../resources/printjobstatus.md) no corpo.</span><span class="sxs-lookup"><span data-stu-id="8f4b6-130">If successful, this method returns a `200 OK` response code and a [printJobStatus](../resources/printjobstatus.md) object in the body.</span></span>

## <a name="example"></a><span data-ttu-id="8f4b6-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8f4b6-131">Example</span></span>
<span data-ttu-id="8f4b6-132">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="8f4b6-132">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8f4b6-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8f4b6-133">Request</span></span>

```http
POST https://graph.microsoft.com/beta/print/shares/{id}/jobs/{id}/start
```

##### <a name="response"></a><span data-ttu-id="8f4b6-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f4b6-134">Response</span></span>
<span data-ttu-id="8f4b6-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8f4b6-135">The following is an example of the response.</span></span> 
><span data-ttu-id="8f4b6-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8f4b6-136">**Note:** The response object shown here might be shortened for readability.</span></span>

```http
HTTP/1.1 200 OK

{
    "state": "processing",
    "description": "The print job is currently being processed.",
    "isAcquiredByPrinter": false,
    "details": ["interpreting"]
}
```


