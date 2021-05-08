---
title: 'deploymentAudience: updateAudienceById'
description: Atualize os membros e as coleções de exclusões de uma deploymentAudience com recursos updatableAsset do mesmo tipo.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 81404ad4807f045b75b3b161ec361f06b622f78b
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240571"
---
# <a name="deploymentaudience-updateaudiencebyid"></a><span data-ttu-id="43f15-103">deploymentAudience: updateAudienceById</span><span class="sxs-lookup"><span data-stu-id="43f15-103">deploymentAudience: updateAudienceById</span></span>
<span data-ttu-id="43f15-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="43f15-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="43f15-105">Atualize os membros e as coleções de exclusões de [uma deploymentAudience](../resources/windowsupdates-deploymentaudience.md) com [recursos updatableAsset](../resources/windowsupdates-updatableasset.md) do mesmo tipo.</span><span class="sxs-lookup"><span data-stu-id="43f15-105">Update the members and exclusions collections of a [deploymentAudience](../resources/windowsupdates-deploymentaudience.md) with [updatableAsset](../resources/windowsupdates-updatableasset.md) resources of the same type.</span></span>

<span data-ttu-id="43f15-106">Adicionar um [azureADDevice](../resources/windowsupdates-azureaddevice.md) aos membros ou coleções de exclusões de um público de implantação cria automaticamente um objeto de dispositivo do Azure AD se ainda não existir.</span><span class="sxs-lookup"><span data-stu-id="43f15-106">Adding an [azureADDevice](../resources/windowsupdates-azureaddevice.md) to the members or exclusions collections of a deployment audience automatically creates an Azure AD device object if it does not already exist.</span></span>

<span data-ttu-id="43f15-107">Se o mesmo [updatableAsset](../resources/windowsupdates-updatableasset.md)  for incluído  nas exclusões e coleções de membros de uma **deploymentAudience,** a implantação não se aplicará a esse ativo.</span><span class="sxs-lookup"><span data-stu-id="43f15-107">If the same [updatableAsset](../resources/windowsupdates-updatableasset.md) gets included in the **exclusions** and **members** collections of a **deploymentAudience**, deployment will not apply to that asset.</span></span>

<span data-ttu-id="43f15-108">Você também pode usar o [método updateAudience](windowsupdates-deploymentaudience-updateaudience.md) para atualizar **a deploymentAudience**.</span><span class="sxs-lookup"><span data-stu-id="43f15-108">You can also use the method [updateAudience](windowsupdates-deploymentaudience-updateaudience.md) to update the **deploymentAudience**.</span></span>

## <a name="permissions"></a><span data-ttu-id="43f15-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="43f15-109">Permissions</span></span>
<span data-ttu-id="43f15-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43f15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43f15-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="43f15-112">Permission type</span></span>|<span data-ttu-id="43f15-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="43f15-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43f15-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="43f15-114">Delegated (work or school account)</span></span>|<span data-ttu-id="43f15-115">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43f15-115">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="43f15-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="43f15-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43f15-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="43f15-117">Not supported.</span></span>|
|<span data-ttu-id="43f15-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="43f15-118">Application</span></span>|<span data-ttu-id="43f15-119">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43f15-119">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="43f15-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="43f15-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/windows/updates/deployments/{deploymentId}/audience/updateAudienceById
```

## <a name="request-headers"></a><span data-ttu-id="43f15-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="43f15-121">Request headers</span></span>
|<span data-ttu-id="43f15-122">Nome</span><span class="sxs-lookup"><span data-stu-id="43f15-122">Name</span></span>|<span data-ttu-id="43f15-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="43f15-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="43f15-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="43f15-124">Authorization</span></span>|<span data-ttu-id="43f15-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="43f15-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="43f15-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="43f15-127">Content-Type</span></span>|<span data-ttu-id="43f15-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="43f15-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="43f15-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="43f15-130">Request body</span></span>
<span data-ttu-id="43f15-131">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="43f15-131">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="43f15-132">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="43f15-132">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="43f15-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="43f15-133">Parameter</span></span>|<span data-ttu-id="43f15-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="43f15-134">Type</span></span>|<span data-ttu-id="43f15-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="43f15-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43f15-136">memberEntityType</span><span class="sxs-lookup"><span data-stu-id="43f15-136">memberEntityType</span></span>|<span data-ttu-id="43f15-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="43f15-137">String</span></span>|<span data-ttu-id="43f15-138">O tipo completo dos ativos atualizáveis.</span><span class="sxs-lookup"><span data-stu-id="43f15-138">The full type of the updatable assets.</span></span> <span data-ttu-id="43f15-139">Os valores possíveis são: `#microsoft.graph.windowsUpdates.azureADDevice` e `#microsoft.graph.windowsUpdates.updatableAssetGroup`.</span><span class="sxs-lookup"><span data-stu-id="43f15-139">Possible values are: `#microsoft.graph.windowsUpdates.azureADDevice`, `#microsoft.graph.windowsUpdates.updatableAssetGroup`.</span></span>|
|<span data-ttu-id="43f15-140">addMembers</span><span class="sxs-lookup"><span data-stu-id="43f15-140">addMembers</span></span>|<span data-ttu-id="43f15-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="43f15-141">String collection</span></span>|<span data-ttu-id="43f15-142">Lista de identificadores correspondentes aos ativos atualizáveis a adicionar como membros da audiência de implantação.</span><span class="sxs-lookup"><span data-stu-id="43f15-142">List of identifiers corresponding to the updatable assets to add as members of the deployment audience.</span></span>|
|<span data-ttu-id="43f15-143">removeMembers</span><span class="sxs-lookup"><span data-stu-id="43f15-143">removeMembers</span></span>|<span data-ttu-id="43f15-144">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="43f15-144">String collection</span></span>|<span data-ttu-id="43f15-145">Lista de identificadores correspondentes aos ativos atualizáveis a ser removidos como membros da audiência de implantação.</span><span class="sxs-lookup"><span data-stu-id="43f15-145">List of identifiers corresponding to the updatable assets to remove as members of the deployment audience.</span></span>|
|<span data-ttu-id="43f15-146">addExclusions</span><span class="sxs-lookup"><span data-stu-id="43f15-146">addExclusions</span></span>|<span data-ttu-id="43f15-147">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="43f15-147">String collection</span></span>|<span data-ttu-id="43f15-148">Lista de identificadores correspondentes aos ativos atualizáveis para adicionar como exclusões do público de implantação.</span><span class="sxs-lookup"><span data-stu-id="43f15-148">List of identifiers corresponding to the updatable assets to add as exclusions from the deployment audience.</span></span>|
|<span data-ttu-id="43f15-149">removeExclusions</span><span class="sxs-lookup"><span data-stu-id="43f15-149">removeExclusions</span></span>|<span data-ttu-id="43f15-150">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="43f15-150">String collection</span></span>|<span data-ttu-id="43f15-151">Lista de identificadores correspondentes aos ativos atualizáveis para remover como exclusões do público de implantação.</span><span class="sxs-lookup"><span data-stu-id="43f15-151">List of identifiers corresponding to the updatable assets to remove as exclusions from the deployment audience.</span></span>|



## <a name="response"></a><span data-ttu-id="43f15-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="43f15-152">Response</span></span>

<span data-ttu-id="43f15-153">Se tiver êxito, esta ação retornará um código de resposta `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="43f15-153">If successful, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="43f15-154">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="43f15-154">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="43f15-155">Exemplos</span><span class="sxs-lookup"><span data-stu-id="43f15-155">Examples</span></span>

### <a name="request"></a><span data-ttu-id="43f15-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="43f15-156">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="43f15-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="43f15-157">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="43f15-158">C#</span><span class="sxs-lookup"><span data-stu-id="43f15-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/deploymentaudience-updateaudiencebyid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="43f15-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="43f15-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/deploymentaudience-updateaudiencebyid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="43f15-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="43f15-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/deploymentaudience-updateaudiencebyid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="43f15-161">Java</span><span class="sxs-lookup"><span data-stu-id="43f15-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/deploymentaudience-updateaudiencebyid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="43f15-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="43f15-162">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

