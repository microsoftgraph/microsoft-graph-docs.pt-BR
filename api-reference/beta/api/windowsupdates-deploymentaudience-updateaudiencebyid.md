---
title: 'deploymentAudience: updateAudienceById'
description: Atualize os membros e as coleções de exclusões de uma deploymentAudience com recursos updatableAsset do mesmo tipo.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 1b948e644628eedc08fe470641b612501dfb80af
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2021
ms.locfileid: "53351115"
---
# <a name="deploymentaudience-updateaudiencebyid"></a><span data-ttu-id="d5c74-103">deploymentAudience: updateAudienceById</span><span class="sxs-lookup"><span data-stu-id="d5c74-103">deploymentAudience: updateAudienceById</span></span>

<span data-ttu-id="d5c74-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="d5c74-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5c74-105">Atualize os membros e as coleções de exclusões de [uma deploymentAudience](../resources/windowsupdates-deploymentaudience.md) com [recursos updatableAsset](../resources/windowsupdates-updatableasset.md) do mesmo tipo.</span><span class="sxs-lookup"><span data-stu-id="d5c74-105">Update the members and exclusions collections of a [deploymentAudience](../resources/windowsupdates-deploymentaudience.md) with [updatableAsset](../resources/windowsupdates-updatableasset.md) resources of the same type.</span></span>

<span data-ttu-id="d5c74-106">Adicionar um [azureADDevice](../resources/windowsupdates-azureaddevice.md) aos membros ou coleções de exclusões de um público de implantação cria automaticamente um objeto de dispositivo do Azure AD se ainda não existir.</span><span class="sxs-lookup"><span data-stu-id="d5c74-106">Adding an [azureADDevice](../resources/windowsupdates-azureaddevice.md) to the members or exclusions collections of a deployment audience automatically creates an Azure AD device object if it does not already exist.</span></span>

<span data-ttu-id="d5c74-107">Se o mesmo [updatableAsset](../resources/windowsupdates-updatableasset.md)  for incluído  nas exclusões e coleções de membros de uma **deploymentAudience,** a implantação não se aplicará a esse ativo.</span><span class="sxs-lookup"><span data-stu-id="d5c74-107">If the same [updatableAsset](../resources/windowsupdates-updatableasset.md) gets included in the **exclusions** and **members** collections of a **deploymentAudience**, deployment will not apply to that asset.</span></span>

<span data-ttu-id="d5c74-108">Você também pode usar o [método updateAudience](windowsupdates-deploymentaudience-updateaudience.md) para atualizar **a deploymentAudience**.</span><span class="sxs-lookup"><span data-stu-id="d5c74-108">You can also use the method [updateAudience](windowsupdates-deploymentaudience-updateaudience.md) to update the **deploymentAudience**.</span></span>

> [!NOTE]
> <span data-ttu-id="d5c74-109">Essa API tem um [problema conhecido relacionado](/Graph/known-issues#accessing-and-updating-deployment-audiences) a implantações criadas por meio do Intune.</span><span class="sxs-lookup"><span data-stu-id="d5c74-109">This API has a [known issue](/Graph/known-issues#accessing-and-updating-deployment-audiences) related to deployments created via Intune.</span></span>

## <a name="permissions"></a><span data-ttu-id="d5c74-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="d5c74-110">Permissions</span></span>
<span data-ttu-id="d5c74-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5c74-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5c74-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d5c74-113">Permission type</span></span>|<span data-ttu-id="d5c74-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d5c74-114">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5c74-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d5c74-115">Delegated (work or school account)</span></span>|<span data-ttu-id="d5c74-116">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5c74-116">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="d5c74-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d5c74-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5c74-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d5c74-118">Not supported.</span></span>|
|<span data-ttu-id="d5c74-119">Application</span><span class="sxs-lookup"><span data-stu-id="d5c74-119">Application</span></span>|<span data-ttu-id="d5c74-120">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5c74-120">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5c74-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d5c74-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/windows/updates/deployments/{deploymentId}/audience/updateAudienceById
```

## <a name="request-headers"></a><span data-ttu-id="d5c74-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d5c74-122">Request headers</span></span>
|<span data-ttu-id="d5c74-123">Nome</span><span class="sxs-lookup"><span data-stu-id="d5c74-123">Name</span></span>|<span data-ttu-id="d5c74-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5c74-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d5c74-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="d5c74-125">Authorization</span></span>|<span data-ttu-id="d5c74-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d5c74-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d5c74-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d5c74-128">Content-Type</span></span>|<span data-ttu-id="d5c74-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d5c74-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5c74-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d5c74-131">Request body</span></span>
<span data-ttu-id="d5c74-132">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="d5c74-132">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d5c74-133">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="d5c74-133">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d5c74-134">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d5c74-134">Parameter</span></span>|<span data-ttu-id="d5c74-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5c74-135">Type</span></span>|<span data-ttu-id="d5c74-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5c74-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5c74-137">memberEntityType</span><span class="sxs-lookup"><span data-stu-id="d5c74-137">memberEntityType</span></span>|<span data-ttu-id="d5c74-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d5c74-138">String</span></span>|<span data-ttu-id="d5c74-139">O tipo completo dos ativos atualizáveis.</span><span class="sxs-lookup"><span data-stu-id="d5c74-139">The full type of the updatable assets.</span></span> <span data-ttu-id="d5c74-140">Os valores possíveis são: `#microsoft.graph.windowsUpdates.azureADDevice` e `#microsoft.graph.windowsUpdates.updatableAssetGroup`.</span><span class="sxs-lookup"><span data-stu-id="d5c74-140">Possible values are: `#microsoft.graph.windowsUpdates.azureADDevice`, `#microsoft.graph.windowsUpdates.updatableAssetGroup`.</span></span>|
|<span data-ttu-id="d5c74-141">addMembers</span><span class="sxs-lookup"><span data-stu-id="d5c74-141">addMembers</span></span>|<span data-ttu-id="d5c74-142">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d5c74-142">String collection</span></span>|<span data-ttu-id="d5c74-143">Lista de identificadores correspondentes aos ativos atualizáveis a adicionar como membros da audiência de implantação.</span><span class="sxs-lookup"><span data-stu-id="d5c74-143">List of identifiers corresponding to the updatable assets to add as members of the deployment audience.</span></span>|
|<span data-ttu-id="d5c74-144">removeMembers</span><span class="sxs-lookup"><span data-stu-id="d5c74-144">removeMembers</span></span>|<span data-ttu-id="d5c74-145">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d5c74-145">String collection</span></span>|<span data-ttu-id="d5c74-146">Lista de identificadores correspondentes aos ativos atualizáveis a ser removidos como membros da audiência de implantação.</span><span class="sxs-lookup"><span data-stu-id="d5c74-146">List of identifiers corresponding to the updatable assets to remove as members of the deployment audience.</span></span>|
|<span data-ttu-id="d5c74-147">addExclusions</span><span class="sxs-lookup"><span data-stu-id="d5c74-147">addExclusions</span></span>|<span data-ttu-id="d5c74-148">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d5c74-148">String collection</span></span>|<span data-ttu-id="d5c74-149">Lista de identificadores correspondentes aos ativos atualizáveis para adicionar como exclusões do público de implantação.</span><span class="sxs-lookup"><span data-stu-id="d5c74-149">List of identifiers corresponding to the updatable assets to add as exclusions from the deployment audience.</span></span>|
|<span data-ttu-id="d5c74-150">removeExclusions</span><span class="sxs-lookup"><span data-stu-id="d5c74-150">removeExclusions</span></span>|<span data-ttu-id="d5c74-151">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d5c74-151">String collection</span></span>|<span data-ttu-id="d5c74-152">Lista de identificadores correspondentes aos ativos atualizáveis para remover como exclusões do público de implantação.</span><span class="sxs-lookup"><span data-stu-id="d5c74-152">List of identifiers corresponding to the updatable assets to remove as exclusions from the deployment audience.</span></span>|



## <a name="response"></a><span data-ttu-id="d5c74-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5c74-153">Response</span></span>

<span data-ttu-id="d5c74-154">Se tiver êxito, esta ação retornará um código de resposta `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="d5c74-154">If successful, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="d5c74-155">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d5c74-155">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d5c74-156">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d5c74-156">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d5c74-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d5c74-157">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d5c74-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="d5c74-158">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d5c74-159">C#</span><span class="sxs-lookup"><span data-stu-id="d5c74-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/deploymentaudience-updateaudiencebyid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d5c74-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d5c74-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/deploymentaudience-updateaudiencebyid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d5c74-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d5c74-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/deploymentaudience-updateaudiencebyid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d5c74-162">Java</span><span class="sxs-lookup"><span data-stu-id="d5c74-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/deploymentaudience-updateaudiencebyid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="d5c74-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5c74-163">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

