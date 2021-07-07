---
title: 'updatableAssetGroup: removeMembers'
description: Remova membros de um updatableAssetGroup.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 80ab7cab56a72633d7a4cb6f1c81d51cf0263d98
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2021
ms.locfileid: "53317179"
---
# <a name="updatableassetgroup-removemembers"></a><span data-ttu-id="7cb51-103">updatableAssetGroup: removeMembers</span><span class="sxs-lookup"><span data-stu-id="7cb51-103">updatableAssetGroup: removeMembers</span></span>
<span data-ttu-id="7cb51-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="7cb51-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7cb51-105">Remover membros de [um updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span><span class="sxs-lookup"><span data-stu-id="7cb51-105">Remove members from an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span></span>

<span data-ttu-id="7cb51-106">Você também pode usar o [método removeMembersById](windowsupdates-updatableassetgroup-removemembersbyid.md) para remover membros.</span><span class="sxs-lookup"><span data-stu-id="7cb51-106">You can also use the method [removeMembersById](windowsupdates-updatableassetgroup-removemembersbyid.md) to remove members.</span></span>

## <a name="permissions"></a><span data-ttu-id="7cb51-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="7cb51-107">Permissions</span></span>
<span data-ttu-id="7cb51-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7cb51-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7cb51-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7cb51-110">Permission type</span></span>|<span data-ttu-id="7cb51-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7cb51-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7cb51-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7cb51-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7cb51-113">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7cb51-113">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="7cb51-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7cb51-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7cb51-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7cb51-115">Not supported.</span></span>|
|<span data-ttu-id="7cb51-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7cb51-116">Application</span></span>|<span data-ttu-id="7cb51-117">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7cb51-117">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7cb51-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7cb51-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/windows/updates/updatableAssets/{updatableAssetGroupId}/removeMembers
```

## <a name="request-headers"></a><span data-ttu-id="7cb51-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7cb51-119">Request headers</span></span>
|<span data-ttu-id="7cb51-120">Nome</span><span class="sxs-lookup"><span data-stu-id="7cb51-120">Name</span></span>|<span data-ttu-id="7cb51-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="7cb51-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7cb51-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7cb51-122">Authorization</span></span>|<span data-ttu-id="7cb51-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7cb51-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="7cb51-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7cb51-125">Content-Type</span></span>|<span data-ttu-id="7cb51-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7cb51-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7cb51-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7cb51-128">Request body</span></span>
<span data-ttu-id="7cb51-129">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="7cb51-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="7cb51-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="7cb51-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="7cb51-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="7cb51-131">Parameter</span></span>|<span data-ttu-id="7cb51-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="7cb51-132">Type</span></span>|<span data-ttu-id="7cb51-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="7cb51-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7cb51-134">assets</span><span class="sxs-lookup"><span data-stu-id="7cb51-134">assets</span></span>|<span data-ttu-id="7cb51-135">[coleção microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="7cb51-135">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="7cb51-136">Lista de **recursos updatableAsset** para remover como membros do **updatableAssetGroup**.</span><span class="sxs-lookup"><span data-stu-id="7cb51-136">List of **updatableAsset** resources to remove as members of the **updatableAssetGroup**.</span></span>|

## <a name="response"></a><span data-ttu-id="7cb51-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="7cb51-137">Response</span></span>

<span data-ttu-id="7cb51-138">Se tiver êxito, esta ação retornará um código de resposta `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="7cb51-138">If successful, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="7cb51-139">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7cb51-139">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7cb51-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7cb51-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7cb51-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7cb51-141">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "updatableassetgroup_removemembers"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/{updatableAssetGroupId}/removeMembers
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

### <a name="response"></a><span data-ttu-id="7cb51-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="7cb51-142">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```
