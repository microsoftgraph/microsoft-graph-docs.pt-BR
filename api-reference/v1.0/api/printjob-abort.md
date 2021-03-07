---
title: 'printJob: abort'
description: Aborte um trabalho de impressão.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: f179b30e7c07d9f577ab63c59142a68362a389f1
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517060"
---
# <a name="printjob-abort"></a><span data-ttu-id="07dea-103">printJob: abort</span><span class="sxs-lookup"><span data-stu-id="07dea-103">printJob: abort</span></span>

<span data-ttu-id="07dea-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07dea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="07dea-105">Aborte um trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="07dea-105">Abort a print job.</span></span> <span data-ttu-id="07dea-106">Somente aplicativos que usam permissões de aplicativo podem cancelar um trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="07dea-106">Only applications using application permissions can abort a print job.</span></span>

## <a name="permissions"></a><span data-ttu-id="07dea-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="07dea-107">Permissions</span></span>
<span data-ttu-id="07dea-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07dea-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="07dea-110">Além das permissões a seguir, o locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa e ter a permissão Printer.Read.All ou Printer.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="07dea-110">In addition to the following permissions, the app's tenant must have an active Universal Print subscription and have either the Printer.Read.All or Printer.ReadWrite.All application permission.</span></span>

|<span data-ttu-id="07dea-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="07dea-111">Permission type</span></span> | <span data-ttu-id="07dea-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="07dea-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="07dea-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="07dea-113">Delegated (work or school account)</span></span>| <span data-ttu-id="07dea-114">Não suportado</span><span class="sxs-lookup"><span data-stu-id="07dea-114">Not Supported</span></span> |
|<span data-ttu-id="07dea-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="07dea-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07dea-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07dea-116">Not Supported.</span></span>|
|<span data-ttu-id="07dea-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="07dea-117">Application</span></span>| <span data-ttu-id="07dea-118">PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All, PrintJob.Manage.All</span><span class="sxs-lookup"><span data-stu-id="07dea-118">PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All, PrintJob.Manage.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="07dea-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="07dea-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/printers/{printerId}/jobs/{printJobId}/abort
```

## <a name="request-headers"></a><span data-ttu-id="07dea-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="07dea-120">Request headers</span></span>
|<span data-ttu-id="07dea-121">Nome</span><span class="sxs-lookup"><span data-stu-id="07dea-121">Name</span></span>|<span data-ttu-id="07dea-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="07dea-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="07dea-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="07dea-123">Authorization</span></span>|<span data-ttu-id="07dea-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="07dea-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="07dea-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="07dea-126">Request body</span></span>
<span data-ttu-id="07dea-127">No corpo da solicitação, opcionalmente, você pode fornecer o motivo pelo qual o trabalho está sendo abortado.</span><span class="sxs-lookup"><span data-stu-id="07dea-127">In the request body, you can optionally provide the reason why the job is being aborted.</span></span>

| <span data-ttu-id="07dea-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="07dea-128">Property</span></span>     | <span data-ttu-id="07dea-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="07dea-129">Type</span></span>        | <span data-ttu-id="07dea-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="07dea-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="07dea-131">motivo</span><span class="sxs-lookup"><span data-stu-id="07dea-131">reason</span></span>|<span data-ttu-id="07dea-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="07dea-132">String</span></span>|<span data-ttu-id="07dea-133">Motivo pelo qual o trabalho está sendo abortado.</span><span class="sxs-lookup"><span data-stu-id="07dea-133">Reason why job is being aborted.</span></span>|

## <a name="response"></a><span data-ttu-id="07dea-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="07dea-134">Response</span></span>

<span data-ttu-id="07dea-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="07dea-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="07dea-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="07dea-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="07dea-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="07dea-138">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "printjob_abort"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/printers/{printerId}/jobs/{printJobId}/abort
Content-Type: application/json
Content-length: 26

{
  "reason": "String"
}
```

### <a name="response"></a><span data-ttu-id="07dea-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="07dea-139">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

