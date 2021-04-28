---
title: Excluir updatableAsset
description: Exclua um objeto updatableAsset.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 7dd7aaf3317eef98568ba89fc3e2c158e64e2784
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067776"
---
# <a name="delete-updatableasset"></a><span data-ttu-id="25572-103">Excluir updatableAsset</span><span class="sxs-lookup"><span data-stu-id="25572-103">Delete updatableAsset</span></span>
<span data-ttu-id="25572-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="25572-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25572-105">[Exclua um objeto updatableAsset.](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="25572-105">Delete an [updatableAsset](../resources/windowsupdates-updatableasset.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="25572-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="25572-106">Permissions</span></span>
<span data-ttu-id="25572-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25572-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25572-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="25572-109">Permission type</span></span>|<span data-ttu-id="25572-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="25572-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="25572-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="25572-111">Delegated (work or school account)</span></span>|<span data-ttu-id="25572-112">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25572-112">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="25572-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="25572-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="25572-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="25572-114">Not supported.</span></span>|
|<span data-ttu-id="25572-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="25572-115">Application</span></span>|<span data-ttu-id="25572-116">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25572-116">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="25572-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="25572-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /admin/windows/updates/updatableAssets/{updatableAssetId}
```

## <a name="request-headers"></a><span data-ttu-id="25572-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="25572-118">Request headers</span></span>
|<span data-ttu-id="25572-119">Nome</span><span class="sxs-lookup"><span data-stu-id="25572-119">Name</span></span>|<span data-ttu-id="25572-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="25572-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="25572-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="25572-121">Authorization</span></span>|<span data-ttu-id="25572-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="25572-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="25572-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="25572-124">Request body</span></span>
<span data-ttu-id="25572-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="25572-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="25572-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="25572-126">Response</span></span>

<span data-ttu-id="25572-p103">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="25572-p103">If successful, this method returns a `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="25572-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="25572-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="25572-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="25572-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_updatableasset"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/{updatableAssetId}
```

### <a name="response"></a><span data-ttu-id="25572-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="25572-131">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

