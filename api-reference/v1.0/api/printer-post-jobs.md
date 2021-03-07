---
title: Criar printJob
description: Crie um novo printJob para uma impressora.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: dfbe431bdf50c5ecc6d6f15278da203139e37629
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516835"
---
# <a name="create-printjob"></a><span data-ttu-id="fd505-103">Criar printJob</span><span class="sxs-lookup"><span data-stu-id="fd505-103">Create printJob</span></span>
<span data-ttu-id="fd505-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd505-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="fd505-105">Criar um novo [printJob](../resources/printJob.md) para uma [impressora](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="fd505-105">Create a new [printJob](../resources/printJob.md) for a [printer](../resources/printer.md).</span></span> 

<span data-ttu-id="fd505-106">Também cria um [novo printDocument](../resources/printDocument.md) associado ao printJob.</span><span class="sxs-lookup"><span data-stu-id="fd505-106">Also creates a new [printDocument](../resources/printDocument.md) associated with the printJob.</span></span>

## <a name="permissions"></a><span data-ttu-id="fd505-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="fd505-107">Permissions</span></span>
<span data-ttu-id="fd505-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd505-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="fd505-110">Além das permissões a seguir, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa e ter uma permissão que conceda [acesso à](printer-get.md) impressora.</span><span class="sxs-lookup"><span data-stu-id="fd505-110">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) access.</span></span> <span data-ttu-id="fd505-111">O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="fd505-111">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="fd505-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fd505-112">Permission type</span></span> | <span data-ttu-id="fd505-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fd505-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="fd505-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fd505-114">Delegated (work or school account)</span></span>| <span data-ttu-id="fd505-115">PrintJob.Create, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd505-115">PrintJob.Create, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="fd505-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fd505-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd505-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fd505-117">Not Supported.</span></span>|
|<span data-ttu-id="fd505-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fd505-118">Application</span></span>| <span data-ttu-id="fd505-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fd505-119">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fd505-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fd505-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/printers/{printerId}/jobs
```

## <a name="request-headers"></a><span data-ttu-id="fd505-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fd505-121">Request headers</span></span>
|<span data-ttu-id="fd505-122">Nome</span><span class="sxs-lookup"><span data-stu-id="fd505-122">Name</span></span>|<span data-ttu-id="fd505-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd505-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="fd505-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="fd505-124">Authorization</span></span>|<span data-ttu-id="fd505-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fd505-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="fd505-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fd505-127">Content-Type</span></span>|<span data-ttu-id="fd505-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fd505-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd505-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fd505-130">Request body</span></span>
<span data-ttu-id="fd505-131">No corpo da solicitação, fornece uma representação JSON de um [objeto printJob.](../resources/printjob.md)</span><span class="sxs-lookup"><span data-stu-id="fd505-131">In the request body, supply a JSON representation of a [printJob](../resources/printjob.md) object.</span></span> <span data-ttu-id="fd505-132">O objeto printJob deve conter apenas uma **propriedade de configuração.**</span><span class="sxs-lookup"><span data-stu-id="fd505-132">The printJob object should only contain a **configuration** property.</span></span> <span data-ttu-id="fd505-133">Todas as propriedades de **configuração** são anuladas.</span><span class="sxs-lookup"><span data-stu-id="fd505-133">All properties of **configuration** are nullable.</span></span> <span data-ttu-id="fd505-134">Todos os outros campos, incluindo IDs de trabalho e documento, são definidos automaticamente durante a criação de recursos e não devem ser fornecidos na solicitação.</span><span class="sxs-lookup"><span data-stu-id="fd505-134">All other fields, including job and document IDs, are set automatically during resource creation and should not be provided in request.</span></span>

<span data-ttu-id="fd505-135">No momento, a Impressão Universal dá suporte a apenas **um objeto printDocument** por **printJob.**</span><span class="sxs-lookup"><span data-stu-id="fd505-135">Right now, Universal Print supports only one **printDocument** per **printJob** object.</span></span>

## <a name="response"></a><span data-ttu-id="fd505-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd505-136">Response</span></span>

<span data-ttu-id="fd505-137">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto printJob](../resources/printjob.md) e [printDocument](../resources/printDocument.md) associado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fd505-137">If successful, this method returns a `201 Created` response code and a [printJob](../resources/printjob.md) object and associated [printDocument](../resources/printDocument.md) in the response body.</span></span> 

## <a name="examples"></a><span data-ttu-id="fd505-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fd505-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fd505-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fd505-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_printjob_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/printers/{printerId}/jobs
Content-Type: application/json
Content-length: 376

{
  "configuration": {
    "@odata.type": "microsoft.graph.printJobConfiguration",
    "feedOrientation": "longEdgeFirst",
    "pageRanges": [
      {
        "@odata.type": "microsoft.graph.integerRange",
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


### <a name="response"></a><span data-ttu-id="fd505-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd505-140">Response</span></span>
<span data-ttu-id="fd505-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="fd505-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/printJobs/$entity",
  "id": "1825",
  "createdDateTime": "2020-10-14T05:16:49-07:00",
  "isFetchable": false,
  "redirectedFrom": null,
  "redirectedTo": null,
  "createdBy": {
    "id": "{userId}",
    "displayName": "{username}",
    "ipAddress": null,
    "userPrincipalName": "{userupn}"
  },
  "status": {
    "state": "paused",
    "description": "The job is not a candidate for processing yet.",
    "isAcquiredByPrinter": false,
    "details": [
      "uploadPending"
    ]
  },
  "configuration": {
    "quality": "medium",
    "dpi": 600,
    "feedOrientation": "longEdgeFirst",
    "orientation": "landscape",
    "duplexMode": "oneSided",
    "copies": 1,
    "colorMode": "blackAndWhite",
    "inputBin": "by-pass-tray",
    "outputBin": "output-tray",
    "mediaSize": "A4",
    "mediaType": "stationery",
    "finishings": null,
    "pagesPerSheet": 1,
    "multipageLayout": "clockwiseFromBottomLeft",
    "collate": false,
    "scaling": "shrinkToFit",
    "fitPdfToPage": false,
    "pageRanges": [
      {
        "start": 1,
        "end": 1
      }
    ],
    "margin": {
      "top": 0,
      "bottom": 0,
      "left": 0,
      "right": 0
    }
  },
  "documents": [
    {
      "id": "1477576d-5dab-4ea9-865c-c0b82cd70bd5",
      "displayName": "",
      "contentType": "",
      "size": 0
    }
  ]
}
```

