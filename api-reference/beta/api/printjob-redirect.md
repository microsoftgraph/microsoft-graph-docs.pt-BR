---
title: 'printJob: Redirect'
description: Redirecionar um trabalho de impressão para uma impressora diferente.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: a3c09827b349b2402aeb8f1a37be64643b87d1d5
ms.sourcegitcommit: d9c167f6be71bdb4a023c5ace2733b9854c846d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2020
ms.locfileid: "49617070"
---
# <a name="printjob-redirect"></a><span data-ttu-id="e750c-103">printJob: Redirect</span><span class="sxs-lookup"><span data-stu-id="e750c-103">printJob: redirect</span></span>

<span data-ttu-id="e750c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e750c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e750c-105">Redirecionar um [trabalho de impressão](../resources/printjob.md) para uma [impressora](../resources/printer.md)diferente.</span><span class="sxs-lookup"><span data-stu-id="e750c-105">Redirect a [print job](../resources/printjob.md) to a different [printer](../resources/printer.md).</span></span>

<span data-ttu-id="e750c-106">Para obter detalhes sobre como usar essa API para adicionar suporte à impressão pull à impressão universal, consulte [Estendeing universal print to support pull Printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="e750c-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="e750c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="e750c-107">Permissions</span></span>
<span data-ttu-id="e750c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e750c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="e750c-110">Para usar o serviço de impressão universal, o usuário ou o locatário do aplicativo deve ter uma assinatura universal de impressão ativa, uma permissão que conceda obter acesso à [impressora](printer-get.md) e uma das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="e750c-110">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, a permission that grants [Get printer](printer-get.md) access, and one of the permissions listed in the following table.</span></span>

|<span data-ttu-id="e750c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e750c-111">Permission type</span></span> | <span data-ttu-id="e750c-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e750c-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="e750c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e750c-113">Delegated (work or school account)</span></span>| <span data-ttu-id="e750c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e750c-114">Not supported.</span></span> |
|<span data-ttu-id="e750c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e750c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e750c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e750c-116">Not Supported.</span></span>|
|<span data-ttu-id="e750c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e750c-117">Application</span></span>| <span data-ttu-id="e750c-118">PrintJob.Manage.All</span><span class="sxs-lookup"><span data-stu-id="e750c-118">PrintJob.Manage.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e750c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e750c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/redirect
```
## <a name="request-headers"></a><span data-ttu-id="e750c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e750c-120">Request headers</span></span>
| <span data-ttu-id="e750c-121">Nome</span><span class="sxs-lookup"><span data-stu-id="e750c-121">Name</span></span>          | <span data-ttu-id="e750c-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e750c-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="e750c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e750c-123">Authorization</span></span> | <span data-ttu-id="e750c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e750c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e750c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e750c-126">Request body</span></span>
<span data-ttu-id="e750c-127">No corpo da solicitação, forneça a ID da impressora para a qual o trabalho de impressão deve ser redirecionado.</span><span class="sxs-lookup"><span data-stu-id="e750c-127">In the request body, supply the ID of the printer that the print job should be redirected to.</span></span>

| <span data-ttu-id="e750c-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e750c-128">Property</span></span>     | <span data-ttu-id="e750c-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="e750c-129">Type</span></span>        | <span data-ttu-id="e750c-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="e750c-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e750c-131">destinationPrinterId</span><span class="sxs-lookup"><span data-stu-id="e750c-131">destinationPrinterId</span></span>|<span data-ttu-id="e750c-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e750c-132">String</span></span>|<span data-ttu-id="e750c-133">A ID da impressora para a qual o trabalho de impressão deve ser redirecionado.</span><span class="sxs-lookup"><span data-stu-id="e750c-133">The ID of the printer the print job should be redirected to.</span></span>|
|<span data-ttu-id="e750c-134">configuration</span><span class="sxs-lookup"><span data-stu-id="e750c-134">configuration</span></span>|<span data-ttu-id="e750c-135">Microsoft. Graph. printJobConfiguration</span><span class="sxs-lookup"><span data-stu-id="e750c-135">microsoft.graph.printJobConfiguration</span></span>|<span data-ttu-id="e750c-136">Configuração atualizada do trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="e750c-136">Updated configuration of print job.</span></span>|

## <a name="response"></a><span data-ttu-id="e750c-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="e750c-137">Response</span></span>
<span data-ttu-id="e750c-138">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [printJob](../resources/printjob.md) enfileirados para a impressora de destino.</span><span class="sxs-lookup"><span data-stu-id="e750c-138">If successful, this method returns a `200 OK` response code and a [printJob](../resources/printjob.md) object queued for the destination printer.</span></span>

## <a name="example"></a><span data-ttu-id="e750c-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e750c-139">Example</span></span>
<span data-ttu-id="e750c-140">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="e750c-140">The following example shows how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="e750c-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e750c-141">Request</span></span>
<span data-ttu-id="e750c-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e750c-142">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "printjob-redirect"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/d5ef6ec4-07ca-4212-baf9-d45be126bfbb/jobs/44353/redirect

{
  "destinationPrinterId": "9a3b3956-ce5b-4d06-a605-5b0bd3e9ddea"
}
```

### <a name="response"></a><span data-ttu-id="e750c-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="e750c-143">Response</span></span>
<span data-ttu-id="e750c-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e750c-144">The following is an example of the response.</span></span> 
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
    "processingState": "processing",
    "processingStateDescription": "The print job is currently being processed by the printer."
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


