---
title: Criar printJob para uma impressora
description: Crie um novo printJob para uma impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: da2a664a6748f73b7dd5df78b7f5e75850860794
ms.sourcegitcommit: a0a5690ad9c109149e0b8c8baba164648ff5c226
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/08/2021
ms.locfileid: "49784841"
---
# <a name="create-printjob-for-a-printer"></a><span data-ttu-id="5bb5d-103">Criar printJob para uma impressora</span><span class="sxs-lookup"><span data-stu-id="5bb5d-103">Create printJob for a printer</span></span>

<span data-ttu-id="5bb5d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5bb5d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5bb5d-105">Crie um novo [printJob](../resources/printJob.md) para uma [impressora.](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="5bb5d-105">Create a new [printJob](../resources/printJob.md) for a [printer](../resources/printer.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="5bb5d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5bb5d-106">Permissions</span></span>
<span data-ttu-id="5bb5d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5bb5d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="5bb5d-109">Além das permissões a seguir, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa e ter uma permissão que conceda acesso [à](printer-get.md) impressora.</span><span class="sxs-lookup"><span data-stu-id="5bb5d-109">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) access.</span></span> <span data-ttu-id="5bb5d-110">O usuário assinado deve ser um Administrador [de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="5bb5d-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="5bb5d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5bb5d-111">Permission type</span></span> | <span data-ttu-id="5bb5d-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5bb5d-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="5bb5d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5bb5d-113">Delegated (work or school account)</span></span>| <span data-ttu-id="5bb5d-114">PrintJob.Create, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5bb5d-114">PrintJob.Create, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="5bb5d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5bb5d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5bb5d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5bb5d-116">Not Supported.</span></span>|
|<span data-ttu-id="5bb5d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5bb5d-117">Application</span></span>| <span data-ttu-id="5bb5d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5bb5d-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5bb5d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5bb5d-119">HTTP request</span></span>

```http
POST print/printers/{id}/jobs
```

## <a name="request-headers"></a><span data-ttu-id="5bb5d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5bb5d-120">Request headers</span></span>
| <span data-ttu-id="5bb5d-121">Nome</span><span class="sxs-lookup"><span data-stu-id="5bb5d-121">Name</span></span>      |<span data-ttu-id="5bb5d-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="5bb5d-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5bb5d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5bb5d-123">Authorization</span></span> | <span data-ttu-id="5bb5d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5bb5d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5bb5d-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="5bb5d-126">Content-type</span></span>  | <span data-ttu-id="5bb5d-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5bb5d-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5bb5d-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5bb5d-129">Request body</span></span>
<span data-ttu-id="5bb5d-130">No corpo da solicitação, fornece uma representação JSON de um [objeto printJob.](../resources/printjob.md)</span><span class="sxs-lookup"><span data-stu-id="5bb5d-130">In the request body, supply a JSON representation of a [printJob](../resources/printjob.md) object.</span></span> <span data-ttu-id="5bb5d-131">O objeto printJob só deve conter **configuração.**</span><span class="sxs-lookup"><span data-stu-id="5bb5d-131">The printJob object should only contain **configuration**.</span></span> <span data-ttu-id="5bb5d-132">Todas as propriedades da **configuração** são anuladas.</span><span class="sxs-lookup"><span data-stu-id="5bb5d-132">All properties of **configuration** are nullable.</span></span> <span data-ttu-id="5bb5d-133">Todos os outros campos, incluindo IDs de trabalho e documento, são definidos automaticamente durante a criação de recursos.</span><span class="sxs-lookup"><span data-stu-id="5bb5d-133">All other fields, including job and document IDs, are set automatically during resource creation.</span></span>

<span data-ttu-id="5bb5d-134">No momento, a Impressão Universal dá suporte a apenas um **printDocument** por **objeto printJob.**</span><span class="sxs-lookup"><span data-stu-id="5bb5d-134">Right now, Universal Print supports only one **printDocument** per **printJob** object.</span></span>

## <a name="response"></a><span data-ttu-id="5bb5d-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="5bb5d-135">Response</span></span>
<span data-ttu-id="5bb5d-136">Se bem-sucedido, este método retorna um código de resposta e um `201 Created` [objeto printJob](../resources/printjob.md) e [um printDocument](../resources/printDocument.md) associado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5bb5d-136">If successful, this method returns a `201 Created` response code and a [printJob](../resources/printjob.md) object and associated [printDocument](../resources/printDocument.md) in the response body.</span></span> 
## <a name="example"></a><span data-ttu-id="5bb5d-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5bb5d-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="5bb5d-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5bb5d-138">Request</span></span>
<span data-ttu-id="5bb5d-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5bb5d-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5bb5d-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="5bb5d-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_printjob"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/jobs
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
# <a name="c"></a>[<span data-ttu-id="5bb5d-141">C#</span><span class="sxs-lookup"><span data-stu-id="5bb5d-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-printjob-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5bb5d-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5bb5d-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-printjob-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5bb5d-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5bb5d-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-printjob-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5bb5d-144">Java</span><span class="sxs-lookup"><span data-stu-id="5bb5d-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-printjob-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="5bb5d-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="5bb5d-145">Response</span></span>
<span data-ttu-id="5bb5d-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5bb5d-146">The following is an example of the response.</span></span>
><span data-ttu-id="5bb5d-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5bb5d-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
