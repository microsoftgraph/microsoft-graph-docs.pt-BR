---
title: 'updatableAssetGroup: removeMembers'
description: Remova membros de um updatableAssetGroup.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 2964bfc1fad02d81bab33936fde1e2cf03293830
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067897"
---
# <a name="updatableassetgroup-removemembers"></a><span data-ttu-id="0bfbd-103">updatableAssetGroup: removeMembers</span><span class="sxs-lookup"><span data-stu-id="0bfbd-103">updatableAssetGroup: removeMembers</span></span>
<span data-ttu-id="0bfbd-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="0bfbd-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0bfbd-105">Remover membros de [um updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span><span class="sxs-lookup"><span data-stu-id="0bfbd-105">Remove members from an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span></span>

<span data-ttu-id="0bfbd-106">Você também pode usar o [método removeMembersById](windowsupdates-updatableassetgroup-removemembersbyid.md) para remover membros.</span><span class="sxs-lookup"><span data-stu-id="0bfbd-106">You can also use the method [removeMembersById](windowsupdates-updatableassetgroup-removemembersbyid.md) to remove members.</span></span>

## <a name="permissions"></a><span data-ttu-id="0bfbd-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="0bfbd-107">Permissions</span></span>
<span data-ttu-id="0bfbd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0bfbd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0bfbd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0bfbd-110">Permission type</span></span>|<span data-ttu-id="0bfbd-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0bfbd-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0bfbd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0bfbd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0bfbd-113">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0bfbd-113">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="0bfbd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0bfbd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0bfbd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0bfbd-115">Not supported.</span></span>|
|<span data-ttu-id="0bfbd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0bfbd-116">Application</span></span>|<span data-ttu-id="0bfbd-117">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0bfbd-117">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0bfbd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0bfbd-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /updatableAssetGroup/{updatableAssetGroupId}/removeMembers
```

## <a name="request-headers"></a><span data-ttu-id="0bfbd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0bfbd-119">Request headers</span></span>
|<span data-ttu-id="0bfbd-120">Nome</span><span class="sxs-lookup"><span data-stu-id="0bfbd-120">Name</span></span>|<span data-ttu-id="0bfbd-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="0bfbd-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0bfbd-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0bfbd-122">Authorization</span></span>|<span data-ttu-id="0bfbd-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0bfbd-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="0bfbd-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0bfbd-125">Content-Type</span></span>|<span data-ttu-id="0bfbd-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0bfbd-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0bfbd-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0bfbd-128">Request body</span></span>
<span data-ttu-id="0bfbd-129">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="0bfbd-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="0bfbd-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="0bfbd-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="0bfbd-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="0bfbd-131">Parameter</span></span>|<span data-ttu-id="0bfbd-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="0bfbd-132">Type</span></span>|<span data-ttu-id="0bfbd-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="0bfbd-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0bfbd-134">assets</span><span class="sxs-lookup"><span data-stu-id="0bfbd-134">assets</span></span>|<span data-ttu-id="0bfbd-135">[coleção microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="0bfbd-135">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="0bfbd-136">Lista de **recursos updatableAsset** para remover como membros do **updatableAssetGroup**.</span><span class="sxs-lookup"><span data-stu-id="0bfbd-136">List of **updatableAsset** resources to remove as members of the **updatableAssetGroup**.</span></span>|

## <a name="response"></a><span data-ttu-id="0bfbd-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="0bfbd-137">Response</span></span>

<span data-ttu-id="0bfbd-138">Se tiver êxito, esta ação retornará um código de resposta `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="0bfbd-138">If successful, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="0bfbd-139">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0bfbd-139">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0bfbd-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0bfbd-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0bfbd-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0bfbd-141">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "updatableassetgroup_removemembers"
}
-->
``` http
POST https://graph.microsoft.com/beta/updatableAssetGroup/{updatableAssetGroupId}/removeMembers
Content-Type: application/json

{
  "assets": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "String (identifier)"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="0bfbd-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="0bfbd-142">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

