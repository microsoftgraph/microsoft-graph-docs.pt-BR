---
title: 'deploymentAudience: updateAudience'
description: Atualize os membros e as coleções de exclusões de uma deploymentAudience.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: c07247f4f8ae3e53480de802a7b5fc1464114866
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241265"
---
# <a name="deploymentaudience-updateaudience"></a><span data-ttu-id="b4a2f-103">deploymentAudience: updateAudience</span><span class="sxs-lookup"><span data-stu-id="b4a2f-103">deploymentAudience: updateAudience</span></span>
<span data-ttu-id="b4a2f-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="b4a2f-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4a2f-105">Atualizar os membros e coleções de exclusões de [uma deploymentAudience](../resources/windowsupdates-deploymentaudience.md).</span><span class="sxs-lookup"><span data-stu-id="b4a2f-105">Update the members and exclusions collections of a [deploymentAudience](../resources/windowsupdates-deploymentaudience.md).</span></span>

<span data-ttu-id="b4a2f-106">Adicionar um [azureADDevice](../resources/windowsupdates-azureaddevice.md) aos membros ou coleções de exclusões de um público de implantação cria automaticamente um objeto de dispositivo do Azure AD, se ainda não existir.</span><span class="sxs-lookup"><span data-stu-id="b4a2f-106">Adding an [azureADDevice](../resources/windowsupdates-azureaddevice.md) to the members or exclusions collections of a deployment audience automatically creates an Azure AD device object, if it does not already exist.</span></span>

<span data-ttu-id="b4a2f-107">Se o mesmo [updatableAsset](../resources/windowsupdates-updatableasset.md)  for incluído  nas exclusões e coleções de membros de uma **deploymentAudience,** a implantação não se aplicará a esse ativo.</span><span class="sxs-lookup"><span data-stu-id="b4a2f-107">If the same [updatableAsset](../resources/windowsupdates-updatableasset.md) gets included in the **exclusions** and **members** collections of a **deploymentAudience**, deployment will not apply to that asset.</span></span>

<span data-ttu-id="b4a2f-108">Se todos **os objetos updateableAsset** são do mesmo tipo, você também pode usar o método [updateAudienceById](windowsupdates-deploymentaudience-updateaudiencebyid.md) para atualizar **a deploymentAudience**.</span><span class="sxs-lookup"><span data-stu-id="b4a2f-108">If all **updatableAsset** objects are the same type, you can also use the method [updateAudienceById](windowsupdates-deploymentaudience-updateaudiencebyid.md) to update the **deploymentAudience**.</span></span>

## <a name="permissions"></a><span data-ttu-id="b4a2f-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="b4a2f-109">Permissions</span></span>
<span data-ttu-id="b4a2f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4a2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4a2f-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b4a2f-112">Permission type</span></span>|<span data-ttu-id="b4a2f-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b4a2f-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4a2f-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b4a2f-114">Delegated (work or school account)</span></span>|<span data-ttu-id="b4a2f-115">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4a2f-115">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="b4a2f-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b4a2f-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4a2f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b4a2f-117">Not supported.</span></span>|
|<span data-ttu-id="b4a2f-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b4a2f-118">Application</span></span>|<span data-ttu-id="b4a2f-119">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4a2f-119">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4a2f-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b4a2f-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/windows/updates/deployments/{deploymentId}/audience/updateAudience
```

## <a name="request-headers"></a><span data-ttu-id="b4a2f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b4a2f-121">Request headers</span></span>
|<span data-ttu-id="b4a2f-122">Nome</span><span class="sxs-lookup"><span data-stu-id="b4a2f-122">Name</span></span>|<span data-ttu-id="b4a2f-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4a2f-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b4a2f-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="b4a2f-124">Authorization</span></span>|<span data-ttu-id="b4a2f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b4a2f-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b4a2f-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b4a2f-127">Content-Type</span></span>|<span data-ttu-id="b4a2f-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b4a2f-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4a2f-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b4a2f-130">Request body</span></span>
<span data-ttu-id="b4a2f-131">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="b4a2f-131">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b4a2f-132">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="b4a2f-132">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b4a2f-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b4a2f-133">Parameter</span></span>|<span data-ttu-id="b4a2f-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="b4a2f-134">Type</span></span>|<span data-ttu-id="b4a2f-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4a2f-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4a2f-136">addMembers</span><span class="sxs-lookup"><span data-stu-id="b4a2f-136">addMembers</span></span>|<span data-ttu-id="b4a2f-137">[coleção microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="b4a2f-137">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="b4a2f-138">Lista de [recursos updatableAsset](../resources/windowsupdates-updatableasset.md) a adicionar como membros da audiência de implantação.</span><span class="sxs-lookup"><span data-stu-id="b4a2f-138">List of [updatableAsset](../resources/windowsupdates-updatableasset.md) resources to add as members of the deployment audience.</span></span>|
|<span data-ttu-id="b4a2f-139">removeMembers</span><span class="sxs-lookup"><span data-stu-id="b4a2f-139">removeMembers</span></span>|<span data-ttu-id="b4a2f-140">[coleção microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="b4a2f-140">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="b4a2f-141">Lista de ativos atualizáveis para remover como membros da audiência de implantação.</span><span class="sxs-lookup"><span data-stu-id="b4a2f-141">List of updatable assets to remove as members of the deployment audience.</span></span>|
|<span data-ttu-id="b4a2f-142">addExclusions</span><span class="sxs-lookup"><span data-stu-id="b4a2f-142">addExclusions</span></span>|<span data-ttu-id="b4a2f-143">[coleção microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="b4a2f-143">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="b4a2f-144">Lista de ativos atualizáveis para adicionar como exclusões da audiência de implantação.</span><span class="sxs-lookup"><span data-stu-id="b4a2f-144">List of updatable assets to add as exclusions from the deployment audience.</span></span>|
|<span data-ttu-id="b4a2f-145">removeExclusions</span><span class="sxs-lookup"><span data-stu-id="b4a2f-145">removeExclusions</span></span>|<span data-ttu-id="b4a2f-146">[coleção microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="b4a2f-146">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="b4a2f-147">Lista de ativos atualizáveis para remover como exclusões da audiência de implantação.</span><span class="sxs-lookup"><span data-stu-id="b4a2f-147">List of updatable assets to remove as exclusions from the deployment audience.</span></span>|



## <a name="response"></a><span data-ttu-id="b4a2f-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4a2f-148">Response</span></span>

<span data-ttu-id="b4a2f-149">Se tiver êxito, esta ação retornará um código de resposta `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="b4a2f-149">If successful, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="b4a2f-150">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b4a2f-150">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b4a2f-151">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b4a2f-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b4a2f-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b4a2f-152">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b4a2f-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="b4a2f-153">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b4a2f-154">C#</span><span class="sxs-lookup"><span data-stu-id="b4a2f-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/deploymentaudience-updateaudience-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b4a2f-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b4a2f-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/deploymentaudience-updateaudience-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b4a2f-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b4a2f-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/deploymentaudience-updateaudience-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b4a2f-157">Java</span><span class="sxs-lookup"><span data-stu-id="b4a2f-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/deploymentaudience-updateaudience-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="b4a2f-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4a2f-158">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

