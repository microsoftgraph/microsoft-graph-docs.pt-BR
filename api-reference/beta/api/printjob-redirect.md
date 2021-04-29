---
title: 'printJob: redirecionamento'
description: Redirecionar um trabalho de impressão para uma impressora diferente.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 916725283b86c59907ddd89e5441902fa0f8c756
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080173"
---
# <a name="printjob-redirect"></a><span data-ttu-id="7b456-103">printJob: redirecionamento</span><span class="sxs-lookup"><span data-stu-id="7b456-103">printJob: redirect</span></span>

<span data-ttu-id="7b456-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b456-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b456-105">Redirecionar [um trabalho de impressão](../resources/printjob.md) para uma impressora [diferente.](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="7b456-105">Redirect a [print job](../resources/printjob.md) to a different [printer](../resources/printer.md).</span></span>

<span data-ttu-id="7b456-106">Redirecionar um trabalho de impressão só terá êxito se houver [um printTask](../resources/printTask.md) em um estado no trabalho de impressão associado, iniciado por um gatilho criado pelo aplicativo `processing` solicitante.</span><span class="sxs-lookup"><span data-stu-id="7b456-106">Redirecting a print job will only succeed if there is a [printTask](../resources/printTask.md) in a `processing` state on the associated print job, started by a trigger that the requesting app created.</span></span> 

<span data-ttu-id="7b456-107">Para obter detalhes sobre como usar essa API para adicionar suporte à impressão pull à Impressão Universal, consulte [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="7b456-107">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="7b456-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="7b456-108">Permissions</span></span>
<span data-ttu-id="7b456-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b456-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="7b456-111">Para usar o serviço Impressão Universal, o usuário ou locatário do aplicativo deve [](printer-get.md) ter uma assinatura de Impressão Universal ativa, uma permissão que concede acesso a Obter impressora e uma das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="7b456-111">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, a permission that grants [Get printer](printer-get.md) access, and one of the permissions listed in the following table.</span></span>

|<span data-ttu-id="7b456-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7b456-112">Permission type</span></span> | <span data-ttu-id="7b456-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7b456-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="7b456-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7b456-114">Delegated (work or school account)</span></span>| <span data-ttu-id="7b456-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7b456-115">Not supported.</span></span> |
|<span data-ttu-id="7b456-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7b456-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b456-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7b456-117">Not Supported.</span></span>|
|<span data-ttu-id="7b456-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7b456-118">Application</span></span>| <span data-ttu-id="7b456-119">PrintJob.Manage.All</span><span class="sxs-lookup"><span data-stu-id="7b456-119">PrintJob.Manage.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7b456-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7b456-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/redirect
```
## <a name="request-headers"></a><span data-ttu-id="7b456-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7b456-121">Request headers</span></span>
| <span data-ttu-id="7b456-122">Nome</span><span class="sxs-lookup"><span data-stu-id="7b456-122">Name</span></span>          | <span data-ttu-id="7b456-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b456-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="7b456-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="7b456-124">Authorization</span></span> | <span data-ttu-id="7b456-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7b456-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7b456-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7b456-127">Request body</span></span>
<span data-ttu-id="7b456-128">No corpo da solicitação, fornece a ID da impressora para a onde o trabalho de impressão deve ser redirecionado.</span><span class="sxs-lookup"><span data-stu-id="7b456-128">In the request body, supply the ID of the printer that the print job should be redirected to.</span></span>

| <span data-ttu-id="7b456-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7b456-129">Property</span></span>     | <span data-ttu-id="7b456-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="7b456-130">Type</span></span>        | <span data-ttu-id="7b456-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b456-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7b456-132">destinationPrinterId</span><span class="sxs-lookup"><span data-stu-id="7b456-132">destinationPrinterId</span></span>|<span data-ttu-id="7b456-133">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="7b456-133">String</span></span>|<span data-ttu-id="7b456-134">A ID da impressora para a que o trabalho de impressão deve ser redirecionado.</span><span class="sxs-lookup"><span data-stu-id="7b456-134">The ID of the printer the print job should be redirected to.</span></span>|
|<span data-ttu-id="7b456-135">configuração</span><span class="sxs-lookup"><span data-stu-id="7b456-135">configuration</span></span>|<span data-ttu-id="7b456-136">microsoft.graph.printJobConfiguration</span><span class="sxs-lookup"><span data-stu-id="7b456-136">microsoft.graph.printJobConfiguration</span></span>|<span data-ttu-id="7b456-137">Configuração atualizada do trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="7b456-137">Updated configuration of print job.</span></span>|

## <a name="response"></a><span data-ttu-id="7b456-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b456-138">Response</span></span>
<span data-ttu-id="7b456-139">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto printJob](../resources/printjob.md) na fila para a impressora de destino.</span><span class="sxs-lookup"><span data-stu-id="7b456-139">If successful, this method returns a `200 OK` response code and a [printJob](../resources/printjob.md) object queued for the destination printer.</span></span>

## <a name="example"></a><span data-ttu-id="7b456-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7b456-140">Example</span></span>
<span data-ttu-id="7b456-141">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="7b456-141">The following example shows how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="7b456-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7b456-142">Request</span></span>
<span data-ttu-id="7b456-143">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7b456-143">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7b456-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="7b456-144">HTTP</span></span>](#tab/http)

# <a name="http"></a>[<span data-ttu-id="7b456-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="7b456-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printjob-redirect"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/d5ef6ec4-07ca-4212-baf9-d45be126bfbb/jobs/44353/redirect

{
  "destinationPrinterId": "9a3b3956-ce5b-4d06-a605-5b0bd3e9ddea",
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
# <a name="c"></a>[<span data-ttu-id="7b456-146">C#</span><span class="sxs-lookup"><span data-stu-id="7b456-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printjob-redirect-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7b456-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7b456-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printjob-redirect-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7b456-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7b456-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printjob-redirect-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7b456-149">Java</span><span class="sxs-lookup"><span data-stu-id="7b456-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printjob-redirect-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a><span data-ttu-id="7b456-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b456-150">Response</span></span>
<span data-ttu-id="7b456-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7b456-151">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 437

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#printJob",
  "@odata.type": "#microsoft.graph.printJob",
  "id": "44354",
  "createdDateTime": "2020-06-30T17:19:09Z",
  "createdBy": {
    "id": "",
    "displayName": "",
    "userPrincipalName": ""
  },
  "status": {
    "state": "processing",
    "description": "The print job is currently being processed by the printer.",
    "details": ["interpreting"]
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
  "description": "printJob: redirect",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


