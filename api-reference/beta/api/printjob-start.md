---
title: 'printJob: iniciar'
description: Envia o trabalho de impressão para a impressora ou o printerShare associado. Ela será impressa após qualquer trabalho pendente existente ser concluído, anulado ou cancelado.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: a78e55b0c3c317c350bcc321fe3463a4541693f1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48714763"
---
# <a name="printjob-start"></a><span data-ttu-id="4d3d1-104">printJob: iniciar</span><span class="sxs-lookup"><span data-stu-id="4d3d1-104">printJob: start</span></span>

<span data-ttu-id="4d3d1-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4d3d1-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d3d1-106">Envia o trabalho de impressão para a [impressora](../resources/printer.md) ou o [printerShare](../resources/printershare.md)associado.</span><span class="sxs-lookup"><span data-stu-id="4d3d1-106">Submits the print job to the associated [printer](../resources/printer.md) or [printerShare](../resources/printershare.md).</span></span> <span data-ttu-id="4d3d1-107">Ela será impressa após qualquer **trabalho** pendente existente ser concluído, anulado ou cancelado.</span><span class="sxs-lookup"><span data-stu-id="4d3d1-107">It will be printed after any existing pending **jobs** are completed, aborted, or canceled.</span></span>

## <a name="permissions"></a><span data-ttu-id="4d3d1-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="4d3d1-108">Permissions</span></span>
<span data-ttu-id="4d3d1-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d3d1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="4d3d1-111">Além das permissões a seguir, o locatário do usuário ou do aplicativo deve ter uma assinatura de impressão universal ativa e ter uma permissão que conceda [obter impressora](printer-get.md) ou [obter printerShare](printershare-get.md) dependendo da impressora ou do printerShare estar sendo usado.</span><span class="sxs-lookup"><span data-stu-id="4d3d1-111">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) or [Get printerShare](printershare-get.md) depending upon whether printer or printerShare is being used.</span></span>

|<span data-ttu-id="4d3d1-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4d3d1-112">Permission type</span></span> | <span data-ttu-id="4d3d1-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4d3d1-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="4d3d1-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4d3d1-114">Delegated (work or school account)</span></span>| <span data-ttu-id="4d3d1-115">PrintJob. ReadWriteBasic, PrintJob. ReadWrite, PrintJob. ReadWriteBasic. All, PrintJob. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="4d3d1-115">PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="4d3d1-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4d3d1-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d3d1-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4d3d1-117">Not Supported.</span></span>|
|<span data-ttu-id="4d3d1-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4d3d1-118">Application</span></span>| <span data-ttu-id="4d3d1-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4d3d1-119">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4d3d1-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4d3d1-120">HTTP request</span></span>
```http
POST /print/shares/{id}/jobs/{id}/start
```
## <a name="request-headers"></a><span data-ttu-id="4d3d1-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4d3d1-121">Request headers</span></span>
| <span data-ttu-id="4d3d1-122">Nome</span><span class="sxs-lookup"><span data-stu-id="4d3d1-122">Name</span></span>          | <span data-ttu-id="4d3d1-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d3d1-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4d3d1-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="4d3d1-124">Authorization</span></span> | <span data-ttu-id="4d3d1-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4d3d1-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4d3d1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4d3d1-127">Request body</span></span>

<span data-ttu-id="4d3d1-128">Não envie um corpo de solicitação para este método.</span><span class="sxs-lookup"><span data-stu-id="4d3d1-128">Do not submit a request body for this method.</span></span> 

## <a name="response"></a><span data-ttu-id="4d3d1-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d3d1-129">Response</span></span>
<span data-ttu-id="4d3d1-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [printJobStatus](../resources/printjobstatus.md) no corpo.</span><span class="sxs-lookup"><span data-stu-id="4d3d1-130">If successful, this method returns a `200 OK` response code and a [printJobStatus](../resources/printjobstatus.md) object in the body.</span></span>

## <a name="example"></a><span data-ttu-id="4d3d1-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4d3d1-131">Example</span></span>
<span data-ttu-id="4d3d1-132">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="4d3d1-132">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4d3d1-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4d3d1-133">Request</span></span>

```http
POST https://graph.microsoft.com/beta/print/shares/{id}/jobs/{id}/start
```

##### <a name="response"></a><span data-ttu-id="4d3d1-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d3d1-134">Response</span></span>
<span data-ttu-id="4d3d1-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4d3d1-135">The following is an example of the response.</span></span> 
><span data-ttu-id="4d3d1-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4d3d1-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK

{
    "state": "processing",
    "description": "The print job is currently being processed.",
    "isAcquiredByPrinter": false,
    "details": ["interpreting"]
}
```


