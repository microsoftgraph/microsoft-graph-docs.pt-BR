---
title: 'updatableAssetGroup: removeMembersById'
description: Remova membros do mesmo tipo de um updatableAssetGroup.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 1ea11298a7aa19d60b69b98b07c003887aae30b3
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067888"
---
# <a name="updatableassetgroup-removemembersbyid"></a><span data-ttu-id="1c7e7-103">updatableAssetGroup: removeMembersById</span><span class="sxs-lookup"><span data-stu-id="1c7e7-103">updatableAssetGroup: removeMembersById</span></span>
<span data-ttu-id="1c7e7-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="1c7e7-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c7e7-105">Remover membros do mesmo tipo de um [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span><span class="sxs-lookup"><span data-stu-id="1c7e7-105">Remove members of the same type from an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span></span>

<span data-ttu-id="1c7e7-106">Você também pode usar o [método removeMembers para](windowsupdates-updatableassetgroup-removemembers.md) remover membros.</span><span class="sxs-lookup"><span data-stu-id="1c7e7-106">You can also use the method [removeMembers](windowsupdates-updatableassetgroup-removemembers.md) to remove members.</span></span>

## <a name="permissions"></a><span data-ttu-id="1c7e7-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="1c7e7-107">Permissions</span></span>
<span data-ttu-id="1c7e7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c7e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c7e7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1c7e7-110">Permission type</span></span>|<span data-ttu-id="1c7e7-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1c7e7-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c7e7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1c7e7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1c7e7-113">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c7e7-113">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="1c7e7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1c7e7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c7e7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1c7e7-115">Not supported.</span></span>|
|<span data-ttu-id="1c7e7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1c7e7-116">Application</span></span>|<span data-ttu-id="1c7e7-117">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c7e7-117">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c7e7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1c7e7-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/windows/updates/updatableAssets/{updatableAssetGroupId}/removeMembersById
```

## <a name="request-headers"></a><span data-ttu-id="1c7e7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1c7e7-119">Request headers</span></span>
|<span data-ttu-id="1c7e7-120">Nome</span><span class="sxs-lookup"><span data-stu-id="1c7e7-120">Name</span></span>|<span data-ttu-id="1c7e7-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c7e7-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1c7e7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1c7e7-122">Authorization</span></span>|<span data-ttu-id="1c7e7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1c7e7-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="1c7e7-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1c7e7-125">Content-Type</span></span>|<span data-ttu-id="1c7e7-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1c7e7-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c7e7-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1c7e7-128">Request body</span></span>
<span data-ttu-id="1c7e7-129">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="1c7e7-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="1c7e7-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="1c7e7-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="1c7e7-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="1c7e7-131">Parameter</span></span>|<span data-ttu-id="1c7e7-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="1c7e7-132">Type</span></span>|<span data-ttu-id="1c7e7-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c7e7-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c7e7-134">ids</span><span class="sxs-lookup"><span data-stu-id="1c7e7-134">ids</span></span>|<span data-ttu-id="1c7e7-135">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="1c7e7-135">String collection</span></span>|<span data-ttu-id="1c7e7-136">Lista de identificadores correspondentes aos [recursos updatableAsset](../resources/windowsupdates-updatableasset.md) a remover como membros do **updatableAssetGroup**.</span><span class="sxs-lookup"><span data-stu-id="1c7e7-136">List of identifiers corresponding to the [updatableAsset](../resources/windowsupdates-updatableasset.md) resources to remove as members of the **updatableAssetGroup**.</span></span>|
|<span data-ttu-id="1c7e7-137">memberEntityType</span><span class="sxs-lookup"><span data-stu-id="1c7e7-137">memberEntityType</span></span>|<span data-ttu-id="1c7e7-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1c7e7-138">String</span></span>|<span data-ttu-id="1c7e7-139">O tipo completo dos **recursos updatableAsset.**</span><span class="sxs-lookup"><span data-stu-id="1c7e7-139">The full type of the **updatableAsset** resources.</span></span> <span data-ttu-id="1c7e7-140">Os valores possíveis são: `#microsoft.graph.windowsUpdates.azureADDevice` .</span><span class="sxs-lookup"><span data-stu-id="1c7e7-140">Possible values are: `#microsoft.graph.windowsUpdates.azureADDevice`.</span></span>|

## <a name="response"></a><span data-ttu-id="1c7e7-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c7e7-141">Response</span></span>

<span data-ttu-id="1c7e7-142">Se tiver êxito, esta ação retornará um código de resposta `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="1c7e7-142">If successful, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="1c7e7-143">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1c7e7-143">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1c7e7-144">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1c7e7-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1c7e7-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1c7e7-145">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "updatableassetgroup_removemembersbyid"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/{updatableAssetGroupId}/removeMembersById
Content-Type: application/json

{
  "ids": [
    "String",
    "String",
    "String"
  ],
  "memberEntityType": "#microsoft.graph.windowsUpdates.azureADDevice"
}
```

### <a name="response"></a><span data-ttu-id="1c7e7-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c7e7-146">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

