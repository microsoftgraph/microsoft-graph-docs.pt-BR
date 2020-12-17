---
title: Atualizar configuração de printJob
description: Atualizar a configuração de um trabalho de impressão
author: tomsato-ms
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 23d61d24367bc5c69d4613ac30deed9244a5ac08
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706219"
---
# <a name="update-printjob-configuration"></a><span data-ttu-id="ef0c9-103">Atualizar configuração de printJob</span><span class="sxs-lookup"><span data-stu-id="ef0c9-103">Update printJob configuration</span></span>

<span data-ttu-id="ef0c9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef0c9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef0c9-105">Atualize a propriedade de [configuração](../resources/printjobconfiguration.md) de um [trabalho de impressão](../resources/printjob.md).</span><span class="sxs-lookup"><span data-stu-id="ef0c9-105">Update the [configuration](../resources/printjobconfiguration.md) property of a [print job](../resources/printjob.md).</span></span>

<span data-ttu-id="ef0c9-106">Atualizar uma configuração de trabalho de impressão requer que o trabalho de impressão esteja em estado mantido registrando um gatilho de tarefa para a impressora.</span><span class="sxs-lookup"><span data-stu-id="ef0c9-106">Updating a print job configuration requires the print job to be in a held state by registering a task trigger for the printer.</span></span> <span data-ttu-id="ef0c9-107">Para obter detalhes sobre como registrar um disparador de tarefas, consulte [estendendo a impressão universal para dar suporte à impressão pull](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="ef0c9-107">For details about how to register a task trigger, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="ef0c9-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="ef0c9-108">Permissions</span></span>
<span data-ttu-id="ef0c9-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef0c9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="ef0c9-111">Para usar o serviço de impressão universal, o usuário ou o locatário do aplicativo deve ter uma assinatura universal de impressão ativa, uma permissão que conceda obter acesso à [impressora](printer-get.md) e uma das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="ef0c9-111">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, a permission that grants [Get printer](printer-get.md) access, and one of the permissions listed in the following table.</span></span>

|<span data-ttu-id="ef0c9-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ef0c9-112">Permission type</span></span> | <span data-ttu-id="ef0c9-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ef0c9-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="ef0c9-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ef0c9-114">Delegated (work or school account)</span></span>| <span data-ttu-id="ef0c9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ef0c9-115">Not supported.</span></span> |
|<span data-ttu-id="ef0c9-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ef0c9-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef0c9-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ef0c9-117">Not Supported.</span></span>|
|<span data-ttu-id="ef0c9-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ef0c9-118">Application</span></span>| <span data-ttu-id="ef0c9-119">PrintJob.Manage.All</span><span class="sxs-lookup"><span data-stu-id="ef0c9-119">PrintJob.Manage.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ef0c9-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ef0c9-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/printers/{id}/jobs/{id}/configuration
```
## <a name="request-headers"></a><span data-ttu-id="ef0c9-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ef0c9-121">Request headers</span></span>
| <span data-ttu-id="ef0c9-122">Nome</span><span class="sxs-lookup"><span data-stu-id="ef0c9-122">Name</span></span>          | <span data-ttu-id="ef0c9-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef0c9-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ef0c9-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="ef0c9-124">Authorization</span></span> | <span data-ttu-id="ef0c9-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ef0c9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ef0c9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ef0c9-127">Request body</span></span>
<span data-ttu-id="ef0c9-128">No corpo da solicitação, forneça os valores dos campos [printJobConfiguration](../resources/printjobconfiguration.md) relevantes.</span><span class="sxs-lookup"><span data-stu-id="ef0c9-128">In the request body, supply the values of the relevant [printJobConfiguration](../resources/printjobconfiguration.md) fields.</span></span> <span data-ttu-id="ef0c9-129">As propriedades existentes que não estão incluídas no corpo da solicitação manterão seus valores anteriores.</span><span class="sxs-lookup"><span data-stu-id="ef0c9-129">Existing properties that are not included in the request body will maintain their previous values.</span></span>

## <a name="response"></a><span data-ttu-id="ef0c9-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef0c9-130">Response</span></span>
<span data-ttu-id="ef0c9-131">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ef0c9-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ef0c9-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ef0c9-132">Example</span></span>
<span data-ttu-id="ef0c9-133">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="ef0c9-133">The following example shows how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="ef0c9-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ef0c9-134">Request</span></span>
<span data-ttu-id="ef0c9-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ef0c9-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "printjob-update-configuration"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/d5ef6ec4-07ca-4212-baf9-d45be126bfbb/jobs/44353/configuration

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

### <a name="response"></a><span data-ttu-id="ef0c9-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef0c9-136">Response</span></span>
<span data-ttu-id="ef0c9-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ef0c9-137">The following is an example of the response.</span></span> 
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


