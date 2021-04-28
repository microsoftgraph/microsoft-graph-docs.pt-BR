---
title: 'updatableAsset: unenrollAssets'
description: Desembrre os recursos updatableAsset do gerenciamento de atualizações pelo serviço de implantação.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 3e714d403fdc6423053bd958201abd3e95352f0f
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067265"
---
# <a name="updatableasset-unenrollassets"></a><span data-ttu-id="56757-103">updatableAsset: unenrollAssets</span><span class="sxs-lookup"><span data-stu-id="56757-103">updatableAsset: unenrollAssets</span></span>
<span data-ttu-id="56757-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="56757-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56757-105">Desembrre [os recursos updatableAsset](../resources/windowsupdates-updatableasset.md) do gerenciamento de atualizações pelo serviço de implantação.</span><span class="sxs-lookup"><span data-stu-id="56757-105">Unenroll [updatableAsset](../resources/windowsupdates-updatableasset.md) resources from update management by the deployment service.</span></span>

<span data-ttu-id="56757-106">Você também pode usar o [método unenrollAssetsById](windowsupdates-updatableasset-unenrollassetsbyid.md) para desemrollar ativos.</span><span class="sxs-lookup"><span data-stu-id="56757-106">You can also use the method [unenrollAssetsById](windowsupdates-updatableasset-unenrollassetsbyid.md) to unenroll assets.</span></span>

## <a name="permissions"></a><span data-ttu-id="56757-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="56757-107">Permissions</span></span>
<span data-ttu-id="56757-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56757-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56757-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="56757-110">Permission type</span></span>|<span data-ttu-id="56757-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="56757-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56757-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="56757-112">Delegated (work or school account)</span></span>|<span data-ttu-id="56757-113">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56757-113">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="56757-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="56757-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56757-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="56757-115">Not supported.</span></span>|
|<span data-ttu-id="56757-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="56757-116">Application</span></span>|<span data-ttu-id="56757-117">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56757-117">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="56757-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="56757-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /updatableAssetGroup/members/unenrollAssets
```

## <a name="request-headers"></a><span data-ttu-id="56757-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="56757-119">Request headers</span></span>
|<span data-ttu-id="56757-120">Nome</span><span class="sxs-lookup"><span data-stu-id="56757-120">Name</span></span>|<span data-ttu-id="56757-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="56757-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="56757-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="56757-122">Authorization</span></span>|<span data-ttu-id="56757-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56757-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="56757-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="56757-125">Content-Type</span></span>|<span data-ttu-id="56757-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56757-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="56757-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="56757-128">Request body</span></span>
<span data-ttu-id="56757-129">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="56757-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="56757-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="56757-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="56757-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="56757-131">Parameter</span></span>|<span data-ttu-id="56757-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="56757-132">Type</span></span>|<span data-ttu-id="56757-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="56757-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56757-134">updateCategory</span><span class="sxs-lookup"><span data-stu-id="56757-134">updateCategory</span></span>|<span data-ttu-id="56757-135">microsoft.graph.windowsUpdates.updateCategory</span><span class="sxs-lookup"><span data-stu-id="56757-135">microsoft.graph.windowsUpdates.updateCategory</span></span>|<span data-ttu-id="56757-136">A categoria de atualizações para o serviço parar de gerenciar.</span><span class="sxs-lookup"><span data-stu-id="56757-136">The category of updates for the service to stop managing.</span></span> <span data-ttu-id="56757-137">Oferece suporte a um subconjunto dos valores **para updateCategory**.</span><span class="sxs-lookup"><span data-stu-id="56757-137">Supports a subset of the values for **updateCategory**.</span></span> <span data-ttu-id="56757-138">Os valores possíveis são: `feature` .</span><span class="sxs-lookup"><span data-stu-id="56757-138">Possible values are: `feature`.</span></span>|
|<span data-ttu-id="56757-139">assets</span><span class="sxs-lookup"><span data-stu-id="56757-139">assets</span></span>|<span data-ttu-id="56757-140">[coleção microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="56757-140">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="56757-141">Lista de **recursos updatableAsset** para desembragem do gerenciamento de atualizações pelo serviço para a **atualização determinadaCategory**.</span><span class="sxs-lookup"><span data-stu-id="56757-141">List of **updatableAsset** resources to unenroll from update management by the service for the given **updateCategory**.</span></span>|



## <a name="response"></a><span data-ttu-id="56757-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="56757-142">Response</span></span>

<span data-ttu-id="56757-143">Se tiver êxito, esta ação retornará um código de resposta `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="56757-143">If successful, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="56757-144">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="56757-144">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="56757-145">Exemplos</span><span class="sxs-lookup"><span data-stu-id="56757-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="56757-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="56757-146">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "updatableasset_unenrollassets"
}
-->
``` http
POST https://graph.microsoft.com/beta/updatableAssetGroup/members/unenrollAssets
Content-Type: application/json

{
  "updateCategory": "String",
  "assets": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "String (identifier)"
    }
  ]
}
```


### <a name="response"></a><span data-ttu-id="56757-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="56757-147">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

