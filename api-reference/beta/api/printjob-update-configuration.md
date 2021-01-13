---
title: Atualizar a configuração do printJob
description: Atualizar a configuração de um trabalho de impressão
author: tomsato-ms
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 1f4d2f1c5573e7f4ad4ae150c598788ab40163ab
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/13/2021
ms.locfileid: "49843574"
---
# <a name="update-printjob-configuration"></a><span data-ttu-id="910fb-103">Atualizar a configuração do printJob</span><span class="sxs-lookup"><span data-stu-id="910fb-103">Update printJob configuration</span></span>

<span data-ttu-id="910fb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="910fb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="910fb-105">Atualizar a [propriedade de](../resources/printjobconfiguration.md) configuração de um trabalho [de impressão.](../resources/printjob.md)</span><span class="sxs-lookup"><span data-stu-id="910fb-105">Update the [configuration](../resources/printjobconfiguration.md) property of a [print job](../resources/printjob.md).</span></span>

<span data-ttu-id="910fb-106">Atualizar uma configuração de trabalho de impressão só será bem-sucedida se houver uma [printTask](../resources/printTask.md) em estado no trabalho de impressão associado, iniciado por um gatilho que solicita o `processing` aplicativo criado.</span><span class="sxs-lookup"><span data-stu-id="910fb-106">Updating a print job configuration will only succeed if there is a [printTask](../resources/printTask.md) in `processing` state on the associated print job, started by a trigger that requesting app created.</span></span> <span data-ttu-id="910fb-107">Para obter detalhes sobre como registrar um gatilho de tarefa, consulte Estendendo a impressão universal para dar suporte [à impressão pull.](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)</span><span class="sxs-lookup"><span data-stu-id="910fb-107">For details about how to register a task trigger, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="910fb-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="910fb-108">Permissions</span></span>
<span data-ttu-id="910fb-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="910fb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="910fb-111">Para usar o serviço de Impressão Universal, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa, a permissão de aplicativo Printer.Read.All ou Printer.ReadWrite.All e uma das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="910fb-111">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, either the Printer.Read.All or Printer.ReadWrite.All application permission, and one of the permissions listed in the following table.</span></span>

|<span data-ttu-id="910fb-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="910fb-112">Permission type</span></span> | <span data-ttu-id="910fb-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="910fb-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="910fb-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="910fb-114">Delegated (work or school account)</span></span>| <span data-ttu-id="910fb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="910fb-115">Not supported.</span></span> |
|<span data-ttu-id="910fb-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="910fb-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="910fb-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="910fb-117">Not Supported.</span></span>|
|<span data-ttu-id="910fb-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="910fb-118">Application</span></span>| <span data-ttu-id="910fb-119">PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="910fb-119">PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="910fb-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="910fb-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/printers/{id}/jobs/{id}/configuration
```
## <a name="request-headers"></a><span data-ttu-id="910fb-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="910fb-121">Request headers</span></span>
| <span data-ttu-id="910fb-122">Nome</span><span class="sxs-lookup"><span data-stu-id="910fb-122">Name</span></span>          | <span data-ttu-id="910fb-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="910fb-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="910fb-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="910fb-124">Authorization</span></span> | <span data-ttu-id="910fb-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="910fb-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="910fb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="910fb-127">Request body</span></span>
<span data-ttu-id="910fb-128">No corpo da solicitação, fornece os valores dos campos [printJobConfiguration](../resources/printjobconfiguration.md) relevantes.</span><span class="sxs-lookup"><span data-stu-id="910fb-128">In the request body, supply the values of the relevant [printJobConfiguration](../resources/printjobconfiguration.md) fields.</span></span> <span data-ttu-id="910fb-129">Propriedades existentes que não estão incluídas no corpo da solicitação manterão seus valores anteriores.</span><span class="sxs-lookup"><span data-stu-id="910fb-129">Existing properties that are not included in the request body will maintain their previous values.</span></span>

## <a name="response"></a><span data-ttu-id="910fb-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="910fb-130">Response</span></span>
<span data-ttu-id="910fb-131">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="910fb-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="910fb-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="910fb-132">Example</span></span>
<span data-ttu-id="910fb-133">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="910fb-133">The following example shows how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="910fb-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="910fb-134">Request</span></span>
<span data-ttu-id="910fb-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="910fb-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="910fb-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="910fb-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printjob-update-configuration"
}-->
```http
PATCH https://graph.microsoft.com/beta/print/printers/d5ef6ec4-07ca-4212-baf9-d45be126bfbb/jobs/44353/configuration

{
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
```
# <a name="c"></a>[<span data-ttu-id="910fb-137">C#</span><span class="sxs-lookup"><span data-stu-id="910fb-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printjob-update-configuration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="910fb-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="910fb-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printjob-update-configuration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="910fb-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="910fb-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printjob-update-configuration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="910fb-140">Java</span><span class="sxs-lookup"><span data-stu-id="910fb-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printjob-update-configuration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a><span data-ttu-id="910fb-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="910fb-141">Response</span></span>
<span data-ttu-id="910fb-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="910fb-142">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update print job configuration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


