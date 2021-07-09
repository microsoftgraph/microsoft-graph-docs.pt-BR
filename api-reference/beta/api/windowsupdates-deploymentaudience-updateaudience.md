---
title: 'deploymentAudience: updateAudience'
description: Atualize os membros e as coleções de exclusões de uma deploymentAudience.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 23fe655e076987ffb33591eb8aaa1600ed4a8fa4
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2021
ms.locfileid: "53351122"
---
# <a name="deploymentaudience-updateaudience"></a><span data-ttu-id="41782-103">deploymentAudience: updateAudience</span><span class="sxs-lookup"><span data-stu-id="41782-103">deploymentAudience: updateAudience</span></span>

<span data-ttu-id="41782-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="41782-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41782-105">Atualizar os membros e coleções de exclusões de [uma deploymentAudience](../resources/windowsupdates-deploymentaudience.md).</span><span class="sxs-lookup"><span data-stu-id="41782-105">Update the members and exclusions collections of a [deploymentAudience](../resources/windowsupdates-deploymentaudience.md).</span></span>

<span data-ttu-id="41782-106">Adicionar um [azureADDevice](../resources/windowsupdates-azureaddevice.md) aos membros ou coleções de exclusões de um público de implantação cria automaticamente um objeto de dispositivo do Azure AD, se ainda não existir.</span><span class="sxs-lookup"><span data-stu-id="41782-106">Adding an [azureADDevice](../resources/windowsupdates-azureaddevice.md) to the members or exclusions collections of a deployment audience automatically creates an Azure AD device object, if it does not already exist.</span></span>

<span data-ttu-id="41782-107">Se o mesmo [updatableAsset](../resources/windowsupdates-updatableasset.md)  for incluído  nas exclusões e coleções de membros de uma **deploymentAudience,** a implantação não se aplicará a esse ativo.</span><span class="sxs-lookup"><span data-stu-id="41782-107">If the same [updatableAsset](../resources/windowsupdates-updatableasset.md) gets included in the **exclusions** and **members** collections of a **deploymentAudience**, deployment will not apply to that asset.</span></span>

<span data-ttu-id="41782-108">Se todos **os objetos updateableAsset** são do mesmo tipo, você também pode usar o método [updateAudienceById](windowsupdates-deploymentaudience-updateaudiencebyid.md) para atualizar **a deploymentAudience**.</span><span class="sxs-lookup"><span data-stu-id="41782-108">If all **updatableAsset** objects are the same type, you can also use the method [updateAudienceById](windowsupdates-deploymentaudience-updateaudiencebyid.md) to update the **deploymentAudience**.</span></span>

> [!NOTE]
> <span data-ttu-id="41782-109">Essa API tem um [problema conhecido relacionado](/Graph/known-issues#accessing-and-updating-deployment-audiences) a implantações criadas por meio do Intune.</span><span class="sxs-lookup"><span data-stu-id="41782-109">This API has a [known issue](/Graph/known-issues#accessing-and-updating-deployment-audiences) related to deployments created via Intune.</span></span>

## <a name="permissions"></a><span data-ttu-id="41782-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="41782-110">Permissions</span></span>
<span data-ttu-id="41782-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41782-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41782-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="41782-113">Permission type</span></span>|<span data-ttu-id="41782-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="41782-114">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41782-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="41782-115">Delegated (work or school account)</span></span>|<span data-ttu-id="41782-116">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41782-116">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="41782-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="41782-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41782-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41782-118">Not supported.</span></span>|
|<span data-ttu-id="41782-119">Application</span><span class="sxs-lookup"><span data-stu-id="41782-119">Application</span></span>|<span data-ttu-id="41782-120">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41782-120">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="41782-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="41782-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/windows/updates/deployments/{deploymentId}/audience/updateAudience
```

## <a name="request-headers"></a><span data-ttu-id="41782-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="41782-122">Request headers</span></span>
|<span data-ttu-id="41782-123">Nome</span><span class="sxs-lookup"><span data-stu-id="41782-123">Name</span></span>|<span data-ttu-id="41782-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="41782-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="41782-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="41782-125">Authorization</span></span>|<span data-ttu-id="41782-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41782-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="41782-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="41782-128">Content-Type</span></span>|<span data-ttu-id="41782-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41782-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="41782-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="41782-131">Request body</span></span>
<span data-ttu-id="41782-132">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="41782-132">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="41782-133">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="41782-133">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="41782-134">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="41782-134">Parameter</span></span>|<span data-ttu-id="41782-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="41782-135">Type</span></span>|<span data-ttu-id="41782-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="41782-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41782-137">addMembers</span><span class="sxs-lookup"><span data-stu-id="41782-137">addMembers</span></span>|<span data-ttu-id="41782-138">[coleção microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="41782-138">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="41782-139">Lista de [recursos updatableAsset](../resources/windowsupdates-updatableasset.md) a adicionar como membros da audiência de implantação.</span><span class="sxs-lookup"><span data-stu-id="41782-139">List of [updatableAsset](../resources/windowsupdates-updatableasset.md) resources to add as members of the deployment audience.</span></span>|
|<span data-ttu-id="41782-140">removeMembers</span><span class="sxs-lookup"><span data-stu-id="41782-140">removeMembers</span></span>|<span data-ttu-id="41782-141">[coleção microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="41782-141">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="41782-142">Lista de ativos atualizáveis para remover como membros da audiência de implantação.</span><span class="sxs-lookup"><span data-stu-id="41782-142">List of updatable assets to remove as members of the deployment audience.</span></span>|
|<span data-ttu-id="41782-143">addExclusions</span><span class="sxs-lookup"><span data-stu-id="41782-143">addExclusions</span></span>|<span data-ttu-id="41782-144">[coleção microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="41782-144">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="41782-145">Lista de ativos atualizáveis para adicionar como exclusões da audiência de implantação.</span><span class="sxs-lookup"><span data-stu-id="41782-145">List of updatable assets to add as exclusions from the deployment audience.</span></span>|
|<span data-ttu-id="41782-146">removeExclusions</span><span class="sxs-lookup"><span data-stu-id="41782-146">removeExclusions</span></span>|<span data-ttu-id="41782-147">[coleção microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="41782-147">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="41782-148">Lista de ativos atualizáveis para remover como exclusões da audiência de implantação.</span><span class="sxs-lookup"><span data-stu-id="41782-148">List of updatable assets to remove as exclusions from the deployment audience.</span></span>|



## <a name="response"></a><span data-ttu-id="41782-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="41782-149">Response</span></span>

<span data-ttu-id="41782-150">Se tiver êxito, esta ação retornará um código de resposta `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="41782-150">If successful, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="41782-151">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="41782-151">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="41782-152">Exemplos</span><span class="sxs-lookup"><span data-stu-id="41782-152">Examples</span></span>

### <a name="request"></a><span data-ttu-id="41782-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="41782-153">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="41782-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="41782-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "deploymentaudience_updateaudience"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/deployments/{deploymentId}/audience/updateAudience
Content-Type: application/json
Content-length: 599

{
  "addMembers": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.updatableAsset",
      "id": "String (identifier)"
    }
  ],
  "removeMembers": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.updatableAsset",
      "id": "String (identifier)"
    }
  ],
  "addExclusions": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.updatableAsset",
      "id": "String (identifier)"
    }
  ],
  "removeExclusions": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.updatableAsset",
      "id": "String (identifier)"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="41782-155">C#</span><span class="sxs-lookup"><span data-stu-id="41782-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/deploymentaudience-updateaudience-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="41782-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="41782-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/deploymentaudience-updateaudience-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="41782-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="41782-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/deploymentaudience-updateaudience-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="41782-158">Java</span><span class="sxs-lookup"><span data-stu-id="41782-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/deploymentaudience-updateaudience-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="41782-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="41782-159">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

