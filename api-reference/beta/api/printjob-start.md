---
title: 'printJob: start'
description: Envia o trabalho de impressão para a impressora ou printerShare associada. Ele será impresso assim que quaisquer trabalhos pendentes existentes são concluídos, anulados ou cancelados.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: d2cb4a5413d592d170e31a882be93d900deca8c1
ms.sourcegitcommit: a0a5690ad9c109149e0b8c8baba164648ff5c226
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/08/2021
ms.locfileid: "49784780"
---
# <a name="printjob-start"></a><span data-ttu-id="007ea-104">printJob: start</span><span class="sxs-lookup"><span data-stu-id="007ea-104">printJob: start</span></span>

<span data-ttu-id="007ea-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="007ea-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="007ea-106">Envia o trabalho de impressão para a impressora [ou](../resources/printer.md) [printerShare associada.](../resources/printershare.md)</span><span class="sxs-lookup"><span data-stu-id="007ea-106">Submits the print job to the associated [printer](../resources/printer.md) or [printerShare](../resources/printershare.md).</span></span> <span data-ttu-id="007ea-107">Ele será impresso depois que quaisquer trabalhos pendentes existentes **são** concluídos, anulados ou cancelados.</span><span class="sxs-lookup"><span data-stu-id="007ea-107">It will be printed after any existing pending **jobs** are completed, aborted, or canceled.</span></span>

## <a name="permissions"></a><span data-ttu-id="007ea-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="007ea-108">Permissions</span></span>
<span data-ttu-id="007ea-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="007ea-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="007ea-111">Além das permissões a seguir, o usuário ou locatário do aplicativo deve ter uma [](printer-get.md) assinatura de Impressão Universal ativa e ter uma permissão que conceda Obter impressora ou [Obter printerShare,](printershare-get.md) dependendo se impressora ou printerShare está sendo usada.</span><span class="sxs-lookup"><span data-stu-id="007ea-111">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) or [Get printerShare](printershare-get.md) depending upon whether printer or printerShare is being used.</span></span>

|<span data-ttu-id="007ea-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="007ea-112">Permission type</span></span> | <span data-ttu-id="007ea-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="007ea-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="007ea-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="007ea-114">Delegated (work or school account)</span></span>| <span data-ttu-id="007ea-115">PrintJob.Create, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="007ea-115">PrintJob.Create, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="007ea-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="007ea-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="007ea-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="007ea-117">Not Supported.</span></span>|
|<span data-ttu-id="007ea-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="007ea-118">Application</span></span>| <span data-ttu-id="007ea-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="007ea-119">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="007ea-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="007ea-120">HTTP request</span></span>
```http
POST /print/shares/{id}/jobs/{id}/start
```
## <a name="request-headers"></a><span data-ttu-id="007ea-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="007ea-121">Request headers</span></span>
| <span data-ttu-id="007ea-122">Nome</span><span class="sxs-lookup"><span data-stu-id="007ea-122">Name</span></span>          | <span data-ttu-id="007ea-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="007ea-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="007ea-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="007ea-124">Authorization</span></span> | <span data-ttu-id="007ea-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="007ea-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="007ea-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="007ea-127">Request body</span></span>

<span data-ttu-id="007ea-128">Não envie um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="007ea-128">Do not submit a request body for this method.</span></span> 

## <a name="response"></a><span data-ttu-id="007ea-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="007ea-129">Response</span></span>
<span data-ttu-id="007ea-130">Se bem-sucedido, este método retorna um código de resposta e um `200 OK` [objeto printJobStatus](../resources/printjobstatus.md) no corpo.</span><span class="sxs-lookup"><span data-stu-id="007ea-130">If successful, this method returns a `200 OK` response code and a [printJobStatus](../resources/printjobstatus.md) object in the body.</span></span>

## <a name="example"></a><span data-ttu-id="007ea-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="007ea-131">Example</span></span>
<span data-ttu-id="007ea-132">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="007ea-132">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="007ea-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="007ea-133">Request</span></span>

```http
POST https://graph.microsoft.com/beta/print/shares/{id}/jobs/{id}/start
```

##### <a name="response"></a><span data-ttu-id="007ea-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="007ea-134">Response</span></span>
<span data-ttu-id="007ea-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="007ea-135">The following is an example of the response.</span></span> 
><span data-ttu-id="007ea-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="007ea-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK

{
    "state": "processing",
    "description": "The print job is currently being processed.",
    "isAcquiredByPrinter": false,
    "details": ["interpreting"]
}
```


