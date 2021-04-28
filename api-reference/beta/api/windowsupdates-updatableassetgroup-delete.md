---
title: Excluir updatableAssetGroup
description: Exclua um objeto updatableAssetGroup.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 207f9df658365e747089a2d77bf15dcb1d50e795
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067891"
---
# <a name="delete-updatableassetgroup"></a><span data-ttu-id="f972b-103">Excluir updatableAssetGroup</span><span class="sxs-lookup"><span data-stu-id="f972b-103">Delete updatableAssetGroup</span></span>
<span data-ttu-id="f972b-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="f972b-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f972b-105">[Exclua um objeto updatableAssetGroup.](../resources/windowsupdates-updatableassetgroup.md)</span><span class="sxs-lookup"><span data-stu-id="f972b-105">Delete an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) object.</span></span>

<span data-ttu-id="f972b-106">Quando um [objeto updatableAssetGroup,](../resources/windowsupdates-updatableassetgroup.md) seus objetos [updatableAsset](../resources/windowsupdates-updatableasset.md) do membro não são excluídos.</span><span class="sxs-lookup"><span data-stu-id="f972b-106">When an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) object, its member [updatableAsset](../resources/windowsupdates-updatableasset.md) objects are not deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="f972b-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f972b-107">Permissions</span></span>
<span data-ttu-id="f972b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f972b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f972b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f972b-110">Permission type</span></span>|<span data-ttu-id="f972b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f972b-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f972b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f972b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f972b-113">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f972b-113">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="f972b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f972b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f972b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f972b-115">Not supported.</span></span>|
|<span data-ttu-id="f972b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f972b-116">Application</span></span>|<span data-ttu-id="f972b-117">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f972b-117">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f972b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f972b-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /admin/windows/updates/updatableAssets/{updatableAssetGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="f972b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f972b-119">Request headers</span></span>
|<span data-ttu-id="f972b-120">Nome</span><span class="sxs-lookup"><span data-stu-id="f972b-120">Name</span></span>|<span data-ttu-id="f972b-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f972b-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f972b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f972b-122">Authorization</span></span>|<span data-ttu-id="f972b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f972b-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f972b-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f972b-125">Request body</span></span>
<span data-ttu-id="f972b-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f972b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f972b-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="f972b-127">Response</span></span>

<span data-ttu-id="f972b-p103">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f972b-p103">If successful, this method returns a `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f972b-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f972b-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f972b-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f972b-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_updatableassetgroup"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/{updatableAssetGroupId}
```


### <a name="response"></a><span data-ttu-id="f972b-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="f972b-132">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

