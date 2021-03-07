---
title: Atualizar printJob
description: Atualizar trabalho de impressão
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 3fd3109f914e08d0dd152b2e22ce5f20a84b2d96
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516897"
---
# <a name="update-printjob"></a><span data-ttu-id="541ae-103">Atualizar printJob</span><span class="sxs-lookup"><span data-stu-id="541ae-103">Update printJob</span></span>
<span data-ttu-id="541ae-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="541ae-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="541ae-105">Atualizar um [trabalho de impressão](../resources/printjob.md).</span><span class="sxs-lookup"><span data-stu-id="541ae-105">Update a [print job](../resources/printjob.md).</span></span> <span data-ttu-id="541ae-106">Somente a **propriedade de** configuração pode ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="541ae-106">Only the **configuration** property can be updated.</span></span>

<span data-ttu-id="541ae-107">A atualização de um trabalho de impressão só terá êxito se houver [um printTask](../resources/printTask.md) em um estado no trabalho de impressão associado, iniciado por um gatilho criado pelo aplicativo `processing` solicitante.</span><span class="sxs-lookup"><span data-stu-id="541ae-107">Updating a print job will only succeed if there is a [printTask](../resources/printTask.md) in a `processing` state on the associated print job, started by a trigger that the requesting app created.</span></span> <span data-ttu-id="541ae-108">Para obter detalhes sobre como registrar um gatilho de tarefas, consulte [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="541ae-108">For details about how to register a task trigger, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="541ae-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="541ae-109">Permissions</span></span>
<span data-ttu-id="541ae-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="541ae-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="541ae-112">Para usar o serviço impressão universal, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa, a permissão Printer.Read.All ou Printer.ReadWrite.All e uma das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="541ae-112">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, either the Printer.Read.All or Printer.ReadWrite.All application permission, and one of the permissions listed in the following table.</span></span>

|<span data-ttu-id="541ae-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="541ae-113">Permission type</span></span> | <span data-ttu-id="541ae-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="541ae-114">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="541ae-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="541ae-115">Delegated (work or school account)</span></span>| <span data-ttu-id="541ae-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="541ae-116">Not supported.</span></span> |
|<span data-ttu-id="541ae-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="541ae-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="541ae-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="541ae-118">Not Supported.</span></span>|
|<span data-ttu-id="541ae-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="541ae-119">Application</span></span>| <span data-ttu-id="541ae-120">PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All, PrintJob.Manage.All</span><span class="sxs-lookup"><span data-stu-id="541ae-120">PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All, PrintJob.Manage.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="541ae-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="541ae-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /print/printers/{printerId}/jobs/{printJobId}
```

## <a name="request-headers"></a><span data-ttu-id="541ae-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="541ae-122">Request headers</span></span>
|<span data-ttu-id="541ae-123">Nome</span><span class="sxs-lookup"><span data-stu-id="541ae-123">Name</span></span>|<span data-ttu-id="541ae-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="541ae-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="541ae-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="541ae-125">Authorization</span></span>|<span data-ttu-id="541ae-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="541ae-p104">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="541ae-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="541ae-128">Content-Type</span></span>|<span data-ttu-id="541ae-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="541ae-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="541ae-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="541ae-131">Request body</span></span>
<span data-ttu-id="541ae-132">No corpo da solicitação, fornece os valores dos campos [printJob relevantes.](../resources/printjob.md)</span><span class="sxs-lookup"><span data-stu-id="541ae-132">In the request body, supply the values of the relevant [printJob](../resources/printjob.md) fields.</span></span> <span data-ttu-id="541ae-133">As propriedades existentes que não estão incluídas no corpo da solicitação manterão seus valores anteriores.</span><span class="sxs-lookup"><span data-stu-id="541ae-133">Existing properties that are not included in the request body will maintain their previous values.</span></span> 

<span data-ttu-id="541ae-134">Somente a **propriedade de** configuração pode ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="541ae-134">Only the **configuration** property can be updated.</span></span>

## <a name="response"></a><span data-ttu-id="541ae-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="541ae-135">Response</span></span>

<span data-ttu-id="541ae-136">Se tiver êxito, este método retornará um código `200 OK` de resposta com um objeto [printJob](../resources/printjob.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="541ae-136">If successful, this method returns a `200 OK` response code with an updated [printJob](../resources/printjob.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="541ae-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="541ae-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="541ae-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="541ae-138">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_printjob"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/print/printers/{printerId}/jobs/{printJobId}
Content-Type: application/json
Content-length: 376

{
  "configuration": {
    "feedOrientation": "longEdgeFirst",
    "pageRanges": [
      {
        "start": 1,
        "end": 1
      }
    ],
    "quality": "medium",
    "dpi": 600,
    "orientation": "landscape",
    "copies": 1,
    "duplexMode": "oneSided",
    "colorMode": "blackAndWhite",
    "inputBin": "by-pass-tray",
    "outputBin": "output-tray",
    "mediaSize": "A4",
    "margin": {
      "top": 0,
      "bottom": 0,
      "left": 0,
      "right": 0
    },
    "mediaType": "stationery",
    "finishings": null,
    "pagesPerSheet": 1,
    "multipageLayout": "clockwiseFromBottomLeft",
    "collate": false,
    "scaling": "shrinkToFit",
    "fitPdfToPage": false
  }
}
```

### <a name="response"></a><span data-ttu-id="541ae-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="541ae-139">Response</span></span>
<span data-ttu-id="541ae-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="541ae-140">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/printers('d5ef6ec4-07ca-4212-baf9-d45be126bfbb')/jobs/$entity",
  "id": "44353",
  "createdDateTime": "2020-06-26T04:20:06.5715544Z",
  "createdBy": {
    "id": "",
    "displayName": "",
    "userPrincipalName": ""
  },
  "status": {
    "state": "paused",
    "description": "The job is not a candidate for processing yet."
  },
  "configuration": {
    "feedOrientation": "longEdgeFirst",
    "pageRanges": [
      {
        "start": 1,
        "end": 1
      }
    ],
    "quality": "medium",
    "dpi": 600,
    "orientation": "landscape",
    "copies": 1,
    "duplexMode": "oneSided",
    "colorMode": "blackAndWhite",
    "inputBin": "by-pass-tray",
    "outputBin": "output-tray",
    "mediaSize": "A4",
    "margin": {
      "top": 0,
      "bottom": 0,
      "left": 0,
      "right": 0
    },
    "mediaType": "stationery",
    "finishings": null,
    "pagesPerSheet": 1,
    "multipageLayout": "clockwiseFromBottomLeft",
    "collate": false,
    "scaling": "shrinkToFit",
    "fitPdfToPage": false
  }
}
```

