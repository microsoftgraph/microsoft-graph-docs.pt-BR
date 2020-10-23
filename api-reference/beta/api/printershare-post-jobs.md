---
title: Criar printJob para um printerShare
description: Criar um novo printJob para um printerShare.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: f991c2b4e50577f13144b7da178cd93308dec532
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48704872"
---
# <a name="create-printjob-for-a-printershare"></a><span data-ttu-id="7a389-103">Criar printJob para um printerShare</span><span class="sxs-lookup"><span data-stu-id="7a389-103">Create printJob for a printerShare</span></span>

<span data-ttu-id="7a389-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a389-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a389-105">Criar um novo [printJob](../resources/printJob.md) para um [printerShare](../resources/printerShare.md).</span><span class="sxs-lookup"><span data-stu-id="7a389-105">Create a new [printJob](../resources/printJob.md) for a [printerShare](../resources/printerShare.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="7a389-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7a389-106">Permissions</span></span>
<span data-ttu-id="7a389-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a389-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="7a389-109">Além das permissões a seguir, o locatário do usuário ou do aplicativo deve ter uma assinatura de impressão universal ativa e ter uma permissão que conceda [Get printerShare](printerShare-get.md) Access.</span><span class="sxs-lookup"><span data-stu-id="7a389-109">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printerShare](printerShare-get.md) access.</span></span> <span data-ttu-id="7a389-110">O usuário conectado deve ser um [administrador da impressora](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="7a389-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="7a389-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7a389-111">Permission type</span></span> | <span data-ttu-id="7a389-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7a389-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="7a389-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7a389-113">Delegated (work or school account)</span></span>| <span data-ttu-id="7a389-114">PrintJob. ReadWriteBasic, PrintJob. ReadWrite, PrintJob. ReadWriteBasic. All, PrintJob. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="7a389-114">PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="7a389-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7a389-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a389-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7a389-116">Not Supported.</span></span>|
|<span data-ttu-id="7a389-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7a389-117">Application</span></span>| <span data-ttu-id="7a389-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7a389-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7a389-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7a389-119">HTTP request</span></span>

```http
POST print/shares/{id}/jobs
```

## <a name="request-headers"></a><span data-ttu-id="7a389-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7a389-120">Request headers</span></span>
| <span data-ttu-id="7a389-121">Nome</span><span class="sxs-lookup"><span data-stu-id="7a389-121">Name</span></span>      |<span data-ttu-id="7a389-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a389-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7a389-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7a389-123">Authorization</span></span> | <span data-ttu-id="7a389-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7a389-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7a389-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="7a389-126">Content-type</span></span>  | <span data-ttu-id="7a389-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7a389-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a389-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7a389-129">Request body</span></span>
<span data-ttu-id="7a389-130">No corpo da solicitação, forneça uma representação JSON de um objeto [printJob](../resources/printjob.md) .</span><span class="sxs-lookup"><span data-stu-id="7a389-130">In the request body, supply a JSON representation of a [printJob](../resources/printjob.md) object.</span></span>
<span data-ttu-id="7a389-131">O objeto printJob só deve conter **configuração**.</span><span class="sxs-lookup"><span data-stu-id="7a389-131">The printJob object should only contain **configuration**.</span></span> <span data-ttu-id="7a389-132">Todas as propriedades de **configuração** são anuláveis.</span><span class="sxs-lookup"><span data-stu-id="7a389-132">All properties of **configuration** are nullable.</span></span>
<span data-ttu-id="7a389-133">Todos os outros campos incluindo as IDs de trabalho e de documento são definidos automaticamente durante a criação do recurso.</span><span class="sxs-lookup"><span data-stu-id="7a389-133">All other fields including job and document IDs are set automatically during resource creation.</span></span>

<span data-ttu-id="7a389-134">No momento, a impressão universal suporta apenas um **documento** impresso por objeto **printJob** .</span><span class="sxs-lookup"><span data-stu-id="7a389-134">Right now, Universal Print supports only one **printDocument** per **printJob** object.</span></span>

## <a name="response"></a><span data-ttu-id="7a389-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a389-135">Response</span></span>
<span data-ttu-id="7a389-136">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto printJob e o [documento](../resources/printDocument.md) de [impressão](../resources/printjob.md) associado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7a389-136">If successful, this method returns a `201 Created` response code and a [printJob](../resources/printjob.md) object and associated [printDocument](../resources/printDocument.md) in the response body.</span></span> 
## <a name="example"></a><span data-ttu-id="7a389-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7a389-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="7a389-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7a389-138">Request</span></span>
<span data-ttu-id="7a389-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7a389-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7a389-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="7a389-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_printjob"
}-->
```http
POST https://graph.microsoft.com/beta/print/shares/{id}/jobs
Content-type: application/json

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

---

### <a name="response"></a><span data-ttu-id="7a389-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a389-141">Response</span></span>
<span data-ttu-id="7a389-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7a389-142">The following is an example of the response.</span></span>
><span data-ttu-id="7a389-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7a389-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 1065

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printJobs/$entity",
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
