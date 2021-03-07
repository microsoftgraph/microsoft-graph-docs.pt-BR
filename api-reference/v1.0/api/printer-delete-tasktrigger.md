---
title: Excluir printTaskTrigger
description: Exclua o gatilho de tarefas de uma impressora.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: e5b4a12e052c3eba729918c40a91ed39542bceb8
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516854"
---
# <a name="delete-printtasktrigger"></a><span data-ttu-id="3e476-103">Excluir printTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="3e476-103">Delete printTaskTrigger</span></span>
<span data-ttu-id="3e476-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e476-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="3e476-105">[Exclua o gatilho de](../resources/printtasktrigger.md) tarefas de uma [impressora](../resources/printer.md) para impedir que eventos de impressão relacionados acionem tarefas na impressora especificada.</span><span class="sxs-lookup"><span data-stu-id="3e476-105">Delete the [task trigger](../resources/printtasktrigger.md) of a [printer](../resources/printer.md) to prevent related print events from triggering tasks on the specified printer.</span></span>

## <a name="permissions"></a><span data-ttu-id="3e476-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3e476-106">Permissions</span></span>
<span data-ttu-id="3e476-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e476-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="3e476-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura de Impressão Universal ativa.</span><span class="sxs-lookup"><span data-stu-id="3e476-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="3e476-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3e476-110">Permission type</span></span> | <span data-ttu-id="3e476-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3e476-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="3e476-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3e476-112">Delegated (work or school account)</span></span>| <span data-ttu-id="3e476-113">Printer.ReadWrite.All, Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="3e476-113">Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="3e476-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3e476-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e476-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3e476-115">Not Supported.</span></span>|
|<span data-ttu-id="3e476-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3e476-116">Application</span></span>|<span data-ttu-id="3e476-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3e476-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3e476-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3e476-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /print/printers/{printerId}/taskTriggers/{printTaskTriggerId}
```

## <a name="request-headers"></a><span data-ttu-id="3e476-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3e476-119">Request headers</span></span>
|<span data-ttu-id="3e476-120">Nome</span><span class="sxs-lookup"><span data-stu-id="3e476-120">Name</span></span>|<span data-ttu-id="3e476-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e476-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3e476-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3e476-122">Authorization</span></span>|<span data-ttu-id="3e476-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3e476-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e476-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3e476-125">Request body</span></span>
<span data-ttu-id="3e476-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3e476-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3e476-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e476-127">Response</span></span>

<span data-ttu-id="3e476-128">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3e476-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="3e476-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3e476-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3e476-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3e476-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_printtasktrigger"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/print/printers/{printerId}/taskTriggers/{printTaskTriggerId}
```

### <a name="response"></a><span data-ttu-id="3e476-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e476-131">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

