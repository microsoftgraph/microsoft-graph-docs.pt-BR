---
title: Excluir implantação
description: Excluir um objeto de implantação.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 305e905c254fc2a5acf66747f147cc009b41ae6a
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067822"
---
# <a name="delete-deployment"></a><span data-ttu-id="4d9d5-103">Excluir implantação</span><span class="sxs-lookup"><span data-stu-id="4d9d5-103">Delete deployment</span></span>
<span data-ttu-id="4d9d5-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="4d9d5-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d9d5-105">Excluir um [objeto de](../resources/windowsupdates-deployment.md) implantação.</span><span class="sxs-lookup"><span data-stu-id="4d9d5-105">Delete a [deployment](../resources/windowsupdates-deployment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4d9d5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4d9d5-106">Permissions</span></span>
<span data-ttu-id="4d9d5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d9d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d9d5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4d9d5-109">Permission type</span></span>|<span data-ttu-id="4d9d5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4d9d5-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d9d5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4d9d5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4d9d5-112">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d9d5-112">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="4d9d5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4d9d5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d9d5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4d9d5-114">Not supported.</span></span>|
|<span data-ttu-id="4d9d5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4d9d5-115">Application</span></span>|<span data-ttu-id="4d9d5-116">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d9d5-116">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d9d5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4d9d5-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /admin/windows/updates/deployments/{deploymentId}
```

## <a name="request-headers"></a><span data-ttu-id="4d9d5-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4d9d5-118">Request headers</span></span>
|<span data-ttu-id="4d9d5-119">Nome</span><span class="sxs-lookup"><span data-stu-id="4d9d5-119">Name</span></span>|<span data-ttu-id="4d9d5-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d9d5-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4d9d5-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4d9d5-121">Authorization</span></span>|<span data-ttu-id="4d9d5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4d9d5-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d9d5-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4d9d5-124">Request body</span></span>
<span data-ttu-id="4d9d5-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4d9d5-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4d9d5-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d9d5-126">Response</span></span>

<span data-ttu-id="4d9d5-p103">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4d9d5-p103">If successful, this method returns a `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4d9d5-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4d9d5-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4d9d5-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4d9d5-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_deployment"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/admin/windows/updates/deployments/{deploymentId}
```


### <a name="response"></a><span data-ttu-id="4d9d5-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d9d5-131">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

