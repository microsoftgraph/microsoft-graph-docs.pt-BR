---
title: 'deploymentAudience: updateAudience'
description: Atualize os membros e as coleções de exclusões de uma deploymentAudience.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: a0567070f4042896835b735fa69b5cd1dddeb1a3
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067273"
---
# <a name="deploymentaudience-updateaudience"></a><span data-ttu-id="884e2-103">deploymentAudience: updateAudience</span><span class="sxs-lookup"><span data-stu-id="884e2-103">deploymentAudience: updateAudience</span></span>
<span data-ttu-id="884e2-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="884e2-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="884e2-105">Atualizar os membros e coleções de exclusões de [uma deploymentAudience](../resources/windowsupdates-deploymentaudience.md).</span><span class="sxs-lookup"><span data-stu-id="884e2-105">Update the members and exclusions collections of a [deploymentAudience](../resources/windowsupdates-deploymentaudience.md).</span></span>

<span data-ttu-id="884e2-106">Adicionar um [azureADDevice](../resources/windowsupdates-azureaddevice.md) aos membros ou coleções de exclusões de um público de implantação cria automaticamente um objeto de dispositivo do Azure AD, se ainda não existir.</span><span class="sxs-lookup"><span data-stu-id="884e2-106">Adding an [azureADDevice](../resources/windowsupdates-azureaddevice.md) to the members or exclusions collections of a deployment audience automatically creates an Azure AD device object, if it does not already exist.</span></span>

<span data-ttu-id="884e2-107">Se o mesmo [updatableAsset](../resources/windowsupdates-updatableasset.md)  for incluído  nas exclusões e coleções de membros de uma **deploymentAudience,** a implantação não se aplicará a esse ativo.</span><span class="sxs-lookup"><span data-stu-id="884e2-107">If the same [updatableAsset](../resources/windowsupdates-updatableasset.md) gets included in the **exclusions** and **members** collections of a **deploymentAudience**, deployment will not apply to that asset.</span></span>

<span data-ttu-id="884e2-108">Se todos **os objetos updateableAsset** são do mesmo tipo, você também pode usar o método [updateAudienceById](windowsupdates-deploymentaudience-updateaudiencebyid.md) para atualizar **a deploymentAudience**.</span><span class="sxs-lookup"><span data-stu-id="884e2-108">If all **updatableAsset** objects are the same type, you can also use the method [updateAudienceById](windowsupdates-deploymentaudience-updateaudiencebyid.md) to update the **deploymentAudience**.</span></span>

## <a name="permissions"></a><span data-ttu-id="884e2-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="884e2-109">Permissions</span></span>
<span data-ttu-id="884e2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="884e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="884e2-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="884e2-112">Permission type</span></span>|<span data-ttu-id="884e2-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="884e2-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="884e2-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="884e2-114">Delegated (work or school account)</span></span>|<span data-ttu-id="884e2-115">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="884e2-115">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="884e2-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="884e2-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="884e2-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="884e2-117">Not supported.</span></span>|
|<span data-ttu-id="884e2-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="884e2-118">Application</span></span>|<span data-ttu-id="884e2-119">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="884e2-119">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="884e2-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="884e2-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/windows/updates/deployments/{deploymentId}/audience/updateAudience
```

## <a name="request-headers"></a><span data-ttu-id="884e2-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="884e2-121">Request headers</span></span>
|<span data-ttu-id="884e2-122">Nome</span><span class="sxs-lookup"><span data-stu-id="884e2-122">Name</span></span>|<span data-ttu-id="884e2-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="884e2-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="884e2-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="884e2-124">Authorization</span></span>|<span data-ttu-id="884e2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="884e2-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="884e2-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="884e2-127">Content-Type</span></span>|<span data-ttu-id="884e2-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="884e2-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="884e2-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="884e2-130">Request body</span></span>
<span data-ttu-id="884e2-131">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="884e2-131">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="884e2-132">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="884e2-132">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="884e2-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="884e2-133">Parameter</span></span>|<span data-ttu-id="884e2-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="884e2-134">Type</span></span>|<span data-ttu-id="884e2-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="884e2-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="884e2-136">addMembers</span><span class="sxs-lookup"><span data-stu-id="884e2-136">addMembers</span></span>|<span data-ttu-id="884e2-137">[coleção microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="884e2-137">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="884e2-138">Lista de [recursos updatableAsset](../resources/windowsupdates-updatableasset.md) a adicionar como membros da audiência de implantação.</span><span class="sxs-lookup"><span data-stu-id="884e2-138">List of [updatableAsset](../resources/windowsupdates-updatableasset.md) resources to add as members of the deployment audience.</span></span>|
|<span data-ttu-id="884e2-139">removeMembers</span><span class="sxs-lookup"><span data-stu-id="884e2-139">removeMembers</span></span>|<span data-ttu-id="884e2-140">[coleção microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="884e2-140">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="884e2-141">Lista de ativos atualizáveis para remover como membros da audiência de implantação.</span><span class="sxs-lookup"><span data-stu-id="884e2-141">List of updatable assets to remove as members of the deployment audience.</span></span>|
|<span data-ttu-id="884e2-142">addExclusions</span><span class="sxs-lookup"><span data-stu-id="884e2-142">addExclusions</span></span>|<span data-ttu-id="884e2-143">[coleção microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="884e2-143">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="884e2-144">Lista de ativos atualizáveis para adicionar como exclusões da audiência de implantação.</span><span class="sxs-lookup"><span data-stu-id="884e2-144">List of updatable assets to add as exclusions from the deployment audience.</span></span>|
|<span data-ttu-id="884e2-145">removeExclusions</span><span class="sxs-lookup"><span data-stu-id="884e2-145">removeExclusions</span></span>|<span data-ttu-id="884e2-146">[coleção microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="884e2-146">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="884e2-147">Lista de ativos atualizáveis para remover como exclusões da audiência de implantação.</span><span class="sxs-lookup"><span data-stu-id="884e2-147">List of updatable assets to remove as exclusions from the deployment audience.</span></span>|



## <a name="response"></a><span data-ttu-id="884e2-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="884e2-148">Response</span></span>

<span data-ttu-id="884e2-149">Se tiver êxito, esta ação retornará um código de resposta `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="884e2-149">If successful, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="884e2-150">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="884e2-150">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="884e2-151">Exemplos</span><span class="sxs-lookup"><span data-stu-id="884e2-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="884e2-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="884e2-152">Request</span></span>

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


### <a name="response"></a><span data-ttu-id="884e2-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="884e2-153">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

