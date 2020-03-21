---
title: 'printJob: startPrintJob'
description: Envia o trabalho de impressão para a impressora associada. Ela será impressa após qualquer trabalho pendente existente ser concluído, anulado ou cancelado.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: a5c558be384fcecad72e08e9d8aa45b0b397da06
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895544"
---
# <a name="printjob-startprintjob"></a><span data-ttu-id="e4a94-104">printJob: startPrintJob</span><span class="sxs-lookup"><span data-stu-id="e4a94-104">printJob: startPrintJob</span></span>

<span data-ttu-id="e4a94-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4a94-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4a94-106">Envia o trabalho de impressão para a [impressora](../resources/printer.md)associada.</span><span class="sxs-lookup"><span data-stu-id="e4a94-106">Submits the print job to the associated [printer](../resources/printer.md).</span></span> <span data-ttu-id="e4a94-107">Ela será impressa após qualquer **trabalho** pendente existente ser concluído, anulado ou cancelado.</span><span class="sxs-lookup"><span data-stu-id="e4a94-107">It will be printed after any existing pending **jobs** are completed, aborted, or canceled.</span></span>

## <a name="permissions"></a><span data-ttu-id="e4a94-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="e4a94-108">Permissions</span></span>
<span data-ttu-id="e4a94-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4a94-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="e4a94-111">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="e4a94-111">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="e4a94-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e4a94-112">Permission type</span></span> | <span data-ttu-id="e4a94-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e4a94-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="e4a94-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e4a94-114">Delegated (work or school account)</span></span>| <span data-ttu-id="e4a94-115">Users. Read. All</span><span class="sxs-lookup"><span data-stu-id="e4a94-115">Users.Read.All</span></span> |
|<span data-ttu-id="e4a94-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e4a94-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4a94-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4a94-117">Not Supported.</span></span>|
|<span data-ttu-id="e4a94-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e4a94-118">Application</span></span>|<span data-ttu-id="e4a94-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4a94-119">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4a94-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e4a94-120">HTTP request</span></span>
```http
POST /print/printers/{id}/jobs/{id}/startPrintJob
```
## <a name="request-headers"></a><span data-ttu-id="e4a94-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e4a94-121">Request headers</span></span>
| <span data-ttu-id="e4a94-122">Nome</span><span class="sxs-lookup"><span data-stu-id="e4a94-122">Name</span></span>          | <span data-ttu-id="e4a94-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4a94-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="e4a94-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e4a94-124">Authorization</span></span> | <span data-ttu-id="e4a94-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e4a94-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e4a94-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e4a94-127">Request body</span></span>

<span data-ttu-id="e4a94-128">Não envie um corpo de solicitação para este metho.</span><span class="sxs-lookup"><span data-stu-id="e4a94-128">Do not submit a request body for this metho.</span></span> 

## <a name="response"></a><span data-ttu-id="e4a94-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4a94-129">Response</span></span>
<span data-ttu-id="e4a94-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [printJobStatus](../resources/printjobstatus.md) no corpo.</span><span class="sxs-lookup"><span data-stu-id="e4a94-130">If successful, this method returns a `200 OK` response code and a [printJobStatus](../resources/printjobstatus.md) object in the body.</span></span>

## <a name="example"></a><span data-ttu-id="e4a94-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e4a94-131">Example</span></span>
<span data-ttu-id="e4a94-132">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="e4a94-132">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e4a94-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e4a94-133">Request</span></span>

```http
POST https://graph.microsoft.com/beta/print/printers/{id}/jobs/{id}/startPrintJob
```

##### <a name="response"></a><span data-ttu-id="e4a94-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4a94-134">Response</span></span>
<span data-ttu-id="e4a94-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e4a94-135">The following is an example of the response.</span></span> 
><span data-ttu-id="e4a94-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e4a94-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK

{
    "processingState": "processing",
    "processingStateDescription": "The print job is currently being processed.",
    "acquiredByPrinter": false
}
```
