---
title: 'deploymentAudience: updateAudienceById'
description: Atualize os membros e as coleções de exclusões de uma deploymentAudience com recursos updatableAsset do mesmo tipo.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 60970c5d6b02d8c9de79e206eab2360a156c5eee
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067777"
---
# <a name="deploymentaudience-updateaudiencebyid"></a><span data-ttu-id="4eb91-103">deploymentAudience: updateAudienceById</span><span class="sxs-lookup"><span data-stu-id="4eb91-103">deploymentAudience: updateAudienceById</span></span>
<span data-ttu-id="4eb91-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="4eb91-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4eb91-105">Atualize os membros e as coleções de exclusões de [uma deploymentAudience](../resources/windowsupdates-deploymentaudience.md) com [recursos updatableAsset](../resources/windowsupdates-updatableasset.md) do mesmo tipo.</span><span class="sxs-lookup"><span data-stu-id="4eb91-105">Update the members and exclusions collections of a [deploymentAudience](../resources/windowsupdates-deploymentaudience.md) with [updatableAsset](../resources/windowsupdates-updatableasset.md) resources of the same type.</span></span>

<span data-ttu-id="4eb91-106">Adicionar um [azureADDevice](../resources/windowsupdates-azureaddevice.md) aos membros ou coleções de exclusões de um público de implantação cria automaticamente um objeto de dispositivo do Azure AD se ainda não existir.</span><span class="sxs-lookup"><span data-stu-id="4eb91-106">Adding an [azureADDevice](../resources/windowsupdates-azureaddevice.md) to the members or exclusions collections of a deployment audience automatically creates an Azure AD device object if it does not already exist.</span></span>

<span data-ttu-id="4eb91-107">Se o mesmo [updatableAsset](../resources/windowsupdates-updatableasset.md)  for incluído  nas exclusões e coleções de membros de uma **deploymentAudience,** a implantação não se aplicará a esse ativo.</span><span class="sxs-lookup"><span data-stu-id="4eb91-107">If the same [updatableAsset](../resources/windowsupdates-updatableasset.md) gets included in the **exclusions** and **members** collections of a **deploymentAudience**, deployment will not apply to that asset.</span></span>

<span data-ttu-id="4eb91-108">Você também pode usar o [método updateAudience](windowsupdates-deploymentaudience-updateaudience.md) para atualizar **a deploymentAudience**.</span><span class="sxs-lookup"><span data-stu-id="4eb91-108">You can also use the method [updateAudience](windowsupdates-deploymentaudience-updateaudience.md) to update the **deploymentAudience**.</span></span>

## <a name="permissions"></a><span data-ttu-id="4eb91-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="4eb91-109">Permissions</span></span>
<span data-ttu-id="4eb91-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4eb91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4eb91-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4eb91-112">Permission type</span></span>|<span data-ttu-id="4eb91-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4eb91-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4eb91-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4eb91-114">Delegated (work or school account)</span></span>|<span data-ttu-id="4eb91-115">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4eb91-115">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="4eb91-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4eb91-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4eb91-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4eb91-117">Not supported.</span></span>|
|<span data-ttu-id="4eb91-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4eb91-118">Application</span></span>|<span data-ttu-id="4eb91-119">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4eb91-119">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4eb91-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4eb91-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/windows/updates/deployments/{deploymentId}/audience/updateAudienceById
```

## <a name="request-headers"></a><span data-ttu-id="4eb91-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4eb91-121">Request headers</span></span>
|<span data-ttu-id="4eb91-122">Nome</span><span class="sxs-lookup"><span data-stu-id="4eb91-122">Name</span></span>|<span data-ttu-id="4eb91-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="4eb91-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4eb91-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="4eb91-124">Authorization</span></span>|<span data-ttu-id="4eb91-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4eb91-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4eb91-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4eb91-127">Content-Type</span></span>|<span data-ttu-id="4eb91-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4eb91-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4eb91-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4eb91-130">Request body</span></span>
<span data-ttu-id="4eb91-131">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="4eb91-131">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="4eb91-132">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="4eb91-132">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="4eb91-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="4eb91-133">Parameter</span></span>|<span data-ttu-id="4eb91-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="4eb91-134">Type</span></span>|<span data-ttu-id="4eb91-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="4eb91-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4eb91-136">memberEntityType</span><span class="sxs-lookup"><span data-stu-id="4eb91-136">memberEntityType</span></span>|<span data-ttu-id="4eb91-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4eb91-137">String</span></span>|<span data-ttu-id="4eb91-138">O tipo completo dos ativos atualizáveis.</span><span class="sxs-lookup"><span data-stu-id="4eb91-138">The full type of the updatable assets.</span></span> <span data-ttu-id="4eb91-139">Os valores possíveis são: `#microsoft.graph.windowsUpdates.azureADDevice` e `#microsoft.graph.windowsUpdates.updatableAssetGroup`.</span><span class="sxs-lookup"><span data-stu-id="4eb91-139">Possible values are: `#microsoft.graph.windowsUpdates.azureADDevice`, `#microsoft.graph.windowsUpdates.updatableAssetGroup`.</span></span>|
|<span data-ttu-id="4eb91-140">addMembers</span><span class="sxs-lookup"><span data-stu-id="4eb91-140">addMembers</span></span>|<span data-ttu-id="4eb91-141">Coleção String</span><span class="sxs-lookup"><span data-stu-id="4eb91-141">String collection</span></span>|<span data-ttu-id="4eb91-142">Lista de identificadores correspondentes aos ativos atualizáveis a adicionar como membros da audiência de implantação.</span><span class="sxs-lookup"><span data-stu-id="4eb91-142">List of identifiers corresponding to the updatable assets to add as members of the deployment audience.</span></span>|
|<span data-ttu-id="4eb91-143">removeMembers</span><span class="sxs-lookup"><span data-stu-id="4eb91-143">removeMembers</span></span>|<span data-ttu-id="4eb91-144">Coleção String</span><span class="sxs-lookup"><span data-stu-id="4eb91-144">String collection</span></span>|<span data-ttu-id="4eb91-145">Lista de identificadores correspondentes aos ativos atualizáveis a ser removidos como membros da audiência de implantação.</span><span class="sxs-lookup"><span data-stu-id="4eb91-145">List of identifiers corresponding to the updatable assets to remove as members of the deployment audience.</span></span>|
|<span data-ttu-id="4eb91-146">addExclusions</span><span class="sxs-lookup"><span data-stu-id="4eb91-146">addExclusions</span></span>|<span data-ttu-id="4eb91-147">Coleção String</span><span class="sxs-lookup"><span data-stu-id="4eb91-147">String collection</span></span>|<span data-ttu-id="4eb91-148">Lista de identificadores correspondentes aos ativos atualizáveis para adicionar como exclusões do público de implantação.</span><span class="sxs-lookup"><span data-stu-id="4eb91-148">List of identifiers corresponding to the updatable assets to add as exclusions from the deployment audience.</span></span>|
|<span data-ttu-id="4eb91-149">removeExclusions</span><span class="sxs-lookup"><span data-stu-id="4eb91-149">removeExclusions</span></span>|<span data-ttu-id="4eb91-150">Coleção String</span><span class="sxs-lookup"><span data-stu-id="4eb91-150">String collection</span></span>|<span data-ttu-id="4eb91-151">Lista de identificadores correspondentes aos ativos atualizáveis para remover como exclusões do público de implantação.</span><span class="sxs-lookup"><span data-stu-id="4eb91-151">List of identifiers corresponding to the updatable assets to remove as exclusions from the deployment audience.</span></span>|



## <a name="response"></a><span data-ttu-id="4eb91-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="4eb91-152">Response</span></span>

<span data-ttu-id="4eb91-153">Se tiver êxito, esta ação retornará um código de resposta `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="4eb91-153">If successful, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="4eb91-154">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4eb91-154">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4eb91-155">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4eb91-155">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4eb91-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4eb91-156">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "deploymentaudience_updateaudiencebyid"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/deployments/{deploymentId}/audience/updateAudienceById
Content-Type: application/json
Content-length: 204

{
  "memberEntityType": "String",
  "addMembers": [
    "String"
  ],
  "removeMembers": [
    "String"
  ],
  "addExclusions": [
    "String"
  ],
  "removeExclusions": [
    "String"
  ]
}
```


### <a name="response"></a><span data-ttu-id="4eb91-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="4eb91-157">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

