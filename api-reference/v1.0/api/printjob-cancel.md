---
title: 'printJob: cancel'
description: Cancele um trabalho de impressão.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 8733a267f20c2f346ed7163d8d0af2a25725dece
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516856"
---
# <a name="printjob-cancel"></a><span data-ttu-id="9f713-103">printJob: cancel</span><span class="sxs-lookup"><span data-stu-id="9f713-103">printJob: cancel</span></span>
<span data-ttu-id="9f713-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f713-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="9f713-105">Cancele um trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="9f713-105">Cancel a print job.</span></span> <span data-ttu-id="9f713-106">Trabalhos de impressão só podem ser cancelados em nome de um usuário, usando permissões delegadas.</span><span class="sxs-lookup"><span data-stu-id="9f713-106">Print jobs can be canceled only on behalf of a user, using delegated permissions.</span></span>

## <a name="permissions"></a><span data-ttu-id="9f713-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="9f713-107">Permissions</span></span>
<span data-ttu-id="9f713-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f713-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="9f713-110">Além das permissões a seguir, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa e ter uma permissão que conceda [acesso à](printer-get.md) impressora.</span><span class="sxs-lookup"><span data-stu-id="9f713-110">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) access.</span></span>

|<span data-ttu-id="9f713-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9f713-111">Permission type</span></span> | <span data-ttu-id="9f713-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9f713-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="9f713-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9f713-113">Delegated (work or school account)</span></span>| <span data-ttu-id="9f713-114">PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f713-114">PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="9f713-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9f713-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f713-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9f713-116">Not Supported.</span></span>|
|<span data-ttu-id="9f713-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9f713-117">Application</span></span>| <span data-ttu-id="9f713-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9f713-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9f713-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9f713-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/printers/{printerId}/jobs/{printJobId}/cancel
```

## <a name="request-headers"></a><span data-ttu-id="9f713-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9f713-120">Request headers</span></span>
|<span data-ttu-id="9f713-121">Nome</span><span class="sxs-lookup"><span data-stu-id="9f713-121">Name</span></span>|<span data-ttu-id="9f713-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f713-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9f713-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9f713-123">Authorization</span></span>|<span data-ttu-id="9f713-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9f713-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f713-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9f713-126">Request body</span></span>
<span data-ttu-id="9f713-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9f713-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f713-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f713-128">Response</span></span>
<span data-ttu-id="9f713-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9f713-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9f713-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9f713-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9f713-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9f713-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "printjob_cancel"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/printers/{printerId}/jobs/{printJobId}/cancel
```

### <a name="response"></a><span data-ttu-id="9f713-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f713-133">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

