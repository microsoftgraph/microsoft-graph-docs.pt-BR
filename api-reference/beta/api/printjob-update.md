---
title: Atualizar printJob
description: Atualize a configuração de um trabalho de impressão.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 801db44363d8ba620577594ae358167e55cce4cc
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50518135"
---
# <a name="update-printjob"></a><span data-ttu-id="af2a3-103">Atualizar printJob</span><span class="sxs-lookup"><span data-stu-id="af2a3-103">Update printJob</span></span>

<span data-ttu-id="af2a3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af2a3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af2a3-105">Atualizar um [trabalho de impressão](../resources/printjob.md).</span><span class="sxs-lookup"><span data-stu-id="af2a3-105">Update a [print job](../resources/printjob.md).</span></span> <span data-ttu-id="af2a3-106">Somente a **propriedade de** configuração pode ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="af2a3-106">Only the **configuration** property can be updated.</span></span>

<span data-ttu-id="af2a3-107">A atualização de um trabalho de impressão só terá êxito se um [printTask](../resources/printTask.md) em um estado, iniciado por um gatilho criado pelo aplicativo solicitante, estiver associado ao `processing` trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="af2a3-107">Updating a print job will only succeed if a [printTask](../resources/printTask.md) in a `processing` state, started by a trigger that the requesting app created, is associated with the print job.</span></span> <span data-ttu-id="af2a3-108">Para obter detalhes sobre como registrar um gatilho de tarefas, consulte [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="af2a3-108">For details about how to register a task trigger, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="af2a3-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="af2a3-109">Permissions</span></span>
<span data-ttu-id="af2a3-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af2a3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="af2a3-112">Para usar o serviço impressão universal, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa, a permissão Printer.Read.All ou Printer.ReadWrite.All e uma das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="af2a3-112">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, either the Printer.Read.All or Printer.ReadWrite.All application permission, and one of the permissions listed in the following table.</span></span>

|<span data-ttu-id="af2a3-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="af2a3-113">Permission type</span></span> | <span data-ttu-id="af2a3-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="af2a3-114">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="af2a3-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="af2a3-115">Delegated (work or school account)</span></span>| <span data-ttu-id="af2a3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="af2a3-116">Not supported.</span></span> |
|<span data-ttu-id="af2a3-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="af2a3-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af2a3-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="af2a3-118">Not Supported.</span></span>|
|<span data-ttu-id="af2a3-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="af2a3-119">Application</span></span>| <span data-ttu-id="af2a3-120">PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All, PrintJob.Manage.All</span><span class="sxs-lookup"><span data-stu-id="af2a3-120">PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All, PrintJob.Manage.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="af2a3-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="af2a3-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/printers/{id}/jobs/{id}
```
## <a name="request-headers"></a><span data-ttu-id="af2a3-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="af2a3-122">Request headers</span></span>
| <span data-ttu-id="af2a3-123">Nome</span><span class="sxs-lookup"><span data-stu-id="af2a3-123">Name</span></span>          | <span data-ttu-id="af2a3-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="af2a3-124">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="af2a3-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="af2a3-125">Authorization</span></span> | <span data-ttu-id="af2a3-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="af2a3-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="af2a3-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="af2a3-128">Request body</span></span>
<span data-ttu-id="af2a3-129">No corpo da solicitação, fornece os valores dos campos [printJob relevantes.](../resources/printjob.md)</span><span class="sxs-lookup"><span data-stu-id="af2a3-129">In the request body, supply the values of the relevant [printJob](../resources/printjob.md) fields.</span></span> <span data-ttu-id="af2a3-130">As propriedades existentes que não estão incluídas no corpo da solicitação manterão seus valores anteriores.</span><span class="sxs-lookup"><span data-stu-id="af2a3-130">Existing properties that are not included in the request body will maintain their previous values.</span></span> <span data-ttu-id="af2a3-131">Somente a propriedade "configuration" pode ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="af2a3-131">Only the "configuration" property can be updated.</span></span>

## <a name="response"></a><span data-ttu-id="af2a3-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="af2a3-132">Response</span></span>
<span data-ttu-id="af2a3-133">Se tiver êxito, este método retornará um código `200 OK` de resposta com um objeto [printJob](../resources/printjob.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="af2a3-133">If successful, this method returns a `200 OK` response code with an updated [printJob](../resources/printjob.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af2a3-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="af2a3-134">Example</span></span>
<span data-ttu-id="af2a3-135">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="af2a3-135">The following example shows how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="af2a3-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="af2a3-136">Request</span></span>
<span data-ttu-id="af2a3-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="af2a3-137">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "printjob-update"
}-->
```http
PATCH https://graph.microsoft.com/beta/print/printers/d5ef6ec4-07ca-4212-baf9-d45be126bfbb/jobs/44353

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

### <a name="response"></a><span data-ttu-id="af2a3-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="af2a3-138">Response</span></span>
<span data-ttu-id="af2a3-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="af2a3-139">The following is an example of the response.</span></span> 
><span data-ttu-id="af2a3-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="af2a3-140">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 225

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers('d5ef6ec4-07ca-4212-baf9-d45be126bfbb')/jobs/$entity",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update print job",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


