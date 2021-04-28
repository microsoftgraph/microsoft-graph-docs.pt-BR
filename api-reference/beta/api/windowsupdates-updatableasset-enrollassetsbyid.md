---
title: 'updatableAsset: enrollAssetsById'
description: Registrar recursos updatableAsset do mesmo tipo no gerenciamento de atualizações pelo serviço de implantação.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: b7a481b214069edc14c188e4de544602924bd7b6
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067270"
---
# <a name="updatableasset-enrollassetsbyid"></a><span data-ttu-id="d562a-103">updatableAsset: enrollAssetsById</span><span class="sxs-lookup"><span data-stu-id="d562a-103">updatableAsset: enrollAssetsById</span></span>
<span data-ttu-id="d562a-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="d562a-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d562a-105">Registrar [recursos updatableAsset](../resources/windowsupdates-updatableasset.md) do mesmo tipo no gerenciamento de atualizações pelo serviço de implantação.</span><span class="sxs-lookup"><span data-stu-id="d562a-105">Enroll [updatableAsset](../resources/windowsupdates-updatableasset.md) resources of the same type in update management by the deployment service.</span></span>

<span data-ttu-id="d562a-106">Você também pode usar o método [enrollAssets](windowsupdates-updatableasset-enrollassets.md) para registrar ativos.</span><span class="sxs-lookup"><span data-stu-id="d562a-106">You can also use the method [enrollAssets](windowsupdates-updatableasset-enrollassets.md) to enroll assets.</span></span>

## <a name="permissions"></a><span data-ttu-id="d562a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d562a-107">Permissions</span></span>
<span data-ttu-id="d562a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d562a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d562a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d562a-110">Permission type</span></span>|<span data-ttu-id="d562a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d562a-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d562a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d562a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d562a-113">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d562a-113">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="d562a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d562a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d562a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d562a-115">Not supported.</span></span>|
|<span data-ttu-id="d562a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d562a-116">Application</span></span>|<span data-ttu-id="d562a-117">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d562a-117">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d562a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d562a-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/windows/updates/updatableAssets/enrollAssetsById
```

## <a name="request-headers"></a><span data-ttu-id="d562a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d562a-119">Request headers</span></span>
|<span data-ttu-id="d562a-120">Nome</span><span class="sxs-lookup"><span data-stu-id="d562a-120">Name</span></span>|<span data-ttu-id="d562a-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d562a-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d562a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d562a-122">Authorization</span></span>|<span data-ttu-id="d562a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d562a-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d562a-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d562a-125">Content-Type</span></span>|<span data-ttu-id="d562a-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d562a-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d562a-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d562a-128">Request body</span></span>
<span data-ttu-id="d562a-129">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="d562a-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d562a-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="d562a-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d562a-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d562a-131">Parameter</span></span>|<span data-ttu-id="d562a-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="d562a-132">Type</span></span>|<span data-ttu-id="d562a-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="d562a-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d562a-134">updateCategory</span><span class="sxs-lookup"><span data-stu-id="d562a-134">updateCategory</span></span>|<span data-ttu-id="d562a-135">microsoft.graph.windowsUpdates.updateCategory</span><span class="sxs-lookup"><span data-stu-id="d562a-135">microsoft.graph.windowsUpdates.updateCategory</span></span>|<span data-ttu-id="d562a-136">A categoria de atualizações para o serviço gerenciar.</span><span class="sxs-lookup"><span data-stu-id="d562a-136">The category of updates for the service to manage.</span></span> <span data-ttu-id="d562a-137">Oferece suporte a um subconjunto dos valores **para updateCategory**.</span><span class="sxs-lookup"><span data-stu-id="d562a-137">Supports a subset of the values for **updateCategory**.</span></span> <span data-ttu-id="d562a-138">Os valores possíveis são: `feature` .</span><span class="sxs-lookup"><span data-stu-id="d562a-138">Possible values are: `feature`.</span></span>|
|<span data-ttu-id="d562a-139">memberEntityType</span><span class="sxs-lookup"><span data-stu-id="d562a-139">memberEntityType</span></span>|<span data-ttu-id="d562a-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d562a-140">String</span></span>|<span data-ttu-id="d562a-141">O tipo completo dos **recursos updatableAsset.**</span><span class="sxs-lookup"><span data-stu-id="d562a-141">The full type of the **updatableAsset** resources.</span></span> <span data-ttu-id="d562a-142">Os valores possíveis são: `#microsoft.graph.windowsUpdates.azureADDevice` .</span><span class="sxs-lookup"><span data-stu-id="d562a-142">Possible values are: `#microsoft.graph.windowsUpdates.azureADDevice`.</span></span>|
|<span data-ttu-id="d562a-143">ids</span><span class="sxs-lookup"><span data-stu-id="d562a-143">ids</span></span>|<span data-ttu-id="d562a-144">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d562a-144">String collection</span></span>|<span data-ttu-id="d562a-145">Lista de identificadores correspondentes aos **recursos updatableAsset** para se inscrever no gerenciamento de atualizações pelo serviço para **a atualização determinadaCategory**.</span><span class="sxs-lookup"><span data-stu-id="d562a-145">List of identifiers corresponding to the **updatableAsset** resources to enroll in update management by the service for the given **updateCategory**.</span></span>|

## <a name="response"></a><span data-ttu-id="d562a-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="d562a-146">Response</span></span>

<span data-ttu-id="d562a-147">Se tiver êxito, esta ação retornará um código de resposta `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="d562a-147">If successful, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="d562a-148">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d562a-148">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d562a-149">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d562a-149">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d562a-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d562a-150">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "updatableasset_enrollassetsbyid"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/enrollAssetsById
Content-Type: application/json

{
  "updateCategory": "feature",
  "memberEntityType": "#microsoft.graph.windowsUpdates.azureADDevice",
  "ids": [
    "String",
    "String",
    "String"
  ]
}
```


### <a name="response"></a><span data-ttu-id="d562a-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="d562a-151">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

