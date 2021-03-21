---
title: Criar printJob para uma printerShare
description: Crie um novo printJob para um printerShare.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 18852d96fe1ba37447c600b20895359584b3580a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50959638"
---
# <a name="create-printjob-for-a-printershare"></a><span data-ttu-id="d2e06-103">Criar printJob para uma printerShare</span><span class="sxs-lookup"><span data-stu-id="d2e06-103">Create printJob for a printerShare</span></span>
<span data-ttu-id="d2e06-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2e06-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="d2e06-105">Criar um novo [printJob](../resources/printJob.md) para uma [printerShare](../resources/printerShare.md).</span><span class="sxs-lookup"><span data-stu-id="d2e06-105">Create a new [printJob](../resources/printJob.md) for a [printerShare](../resources/printerShare.md).</span></span> 

<span data-ttu-id="d2e06-106">Também cria um [novo printDocument](../resources/printDocument.md) associado ao printJob.</span><span class="sxs-lookup"><span data-stu-id="d2e06-106">Also creates a new [printDocument](../resources/printDocument.md) associated with the printJob.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2e06-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d2e06-107">Permissions</span></span>
<span data-ttu-id="d2e06-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2e06-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="d2e06-110">Além das permissões a seguir, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa e ter uma permissão que conceda [acesso a Get printerShare.](printerShare-get.md)</span><span class="sxs-lookup"><span data-stu-id="d2e06-110">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printerShare](printerShare-get.md) access.</span></span> <span data-ttu-id="d2e06-111">O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="d2e06-111">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="d2e06-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d2e06-112">Permission type</span></span> | <span data-ttu-id="d2e06-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d2e06-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="d2e06-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d2e06-114">Delegated (work or school account)</span></span>| <span data-ttu-id="d2e06-115">PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2e06-115">PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="d2e06-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d2e06-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2e06-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d2e06-117">Not Supported.</span></span>|
|<span data-ttu-id="d2e06-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d2e06-118">Application</span></span>| <span data-ttu-id="d2e06-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d2e06-119">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d2e06-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d2e06-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/shares/{printerShareId}/jobs
```

## <a name="request-headers"></a><span data-ttu-id="d2e06-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d2e06-121">Request headers</span></span>
|<span data-ttu-id="d2e06-122">Nome</span><span class="sxs-lookup"><span data-stu-id="d2e06-122">Name</span></span>|<span data-ttu-id="d2e06-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2e06-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d2e06-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d2e06-124">Authorization</span></span>|<span data-ttu-id="d2e06-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d2e06-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d2e06-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d2e06-127">Content-Type</span></span>|<span data-ttu-id="d2e06-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d2e06-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2e06-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d2e06-130">Request body</span></span>
<span data-ttu-id="d2e06-131">No corpo da solicitação, fornece uma representação JSON de um [objeto printJob.](../resources/printjob.md)</span><span class="sxs-lookup"><span data-stu-id="d2e06-131">In the request body, supply a JSON representation of a [printJob](../resources/printjob.md) object.</span></span> <span data-ttu-id="d2e06-132">O objeto printJob deve conter apenas a **propriedade configuration.**</span><span class="sxs-lookup"><span data-stu-id="d2e06-132">The printJob object should only contain **configuration** property.</span></span> <span data-ttu-id="d2e06-133">Todas as propriedades de **configuração** são anuladas.</span><span class="sxs-lookup"><span data-stu-id="d2e06-133">All properties of **configuration** are nullable.</span></span> <span data-ttu-id="d2e06-134">Todos os outros campos, incluindo IDs de trabalho e documento, são definidos automaticamente durante a criação de recursos e não devem ser fornecidos na solicitação.</span><span class="sxs-lookup"><span data-stu-id="d2e06-134">All other fields, including job and document IDs, are set automatically during resource creation and should not be provided in request.</span></span>

<span data-ttu-id="d2e06-135">No momento, a Impressão Universal dá suporte a apenas **um objeto printDocument** por **printJob.**</span><span class="sxs-lookup"><span data-stu-id="d2e06-135">Right now, Universal Print supports only one **printDocument** per **printJob** object.</span></span>

## <a name="response"></a><span data-ttu-id="d2e06-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2e06-136">Response</span></span>

<span data-ttu-id="d2e06-137">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto printJob](../resources/printjob.md) e [printDocument](../resources/printDocument.md) associado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d2e06-137">If successful, this method returns a `201 Created` response code and a [printJob](../resources/printjob.md) object and associated [printDocument](../resources/printDocument.md) in the response body.</span></span> 

## <a name="examples"></a><span data-ttu-id="d2e06-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d2e06-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d2e06-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d2e06-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d2e06-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="d2e06-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_printjob_from__2"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/shares/{printerShareId}/jobs
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
# <a name="c"></a>[<span data-ttu-id="d2e06-141">C#</span><span class="sxs-lookup"><span data-stu-id="d2e06-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-printjob-from--2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d2e06-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d2e06-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-printjob-from--2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d2e06-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d2e06-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-printjob-from--2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d2e06-144">Java</span><span class="sxs-lookup"><span data-stu-id="d2e06-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-printjob-from--2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="d2e06-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2e06-145">Response</span></span>
<span data-ttu-id="d2e06-146">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d2e06-146">**Note:** The response object shown here might be shortened for readability.</span></span>
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

