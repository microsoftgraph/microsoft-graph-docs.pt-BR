---
title: 'updatableAsset: enrollAssets'
description: Registrar recursos updatableAsset no gerenciamento de atualizações pelo serviço de implantação.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 2b488eaaa70ba0b04a440aabcde0d759ad6e8d36
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067272"
---
# <a name="updatableasset-enrollassets"></a><span data-ttu-id="46883-103">updatableAsset: enrollAssets</span><span class="sxs-lookup"><span data-stu-id="46883-103">updatableAsset: enrollAssets</span></span>
<span data-ttu-id="46883-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="46883-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46883-105">Registrar [recursos updatableAsset](../resources/windowsupdates-updatableasset.md) no gerenciamento de atualizações pelo serviço de implantação.</span><span class="sxs-lookup"><span data-stu-id="46883-105">Enroll [updatableAsset](../resources/windowsupdates-updatableasset.md) resources in update management by the deployment service.</span></span>

<span data-ttu-id="46883-106">Você pode registrar um [recurso do azureADDevice](../resources/windowsupdates-azureaddevice.md) no gerenciamento de atualizações, mas pode não registrar um [UpdateableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) no gerenciamento de atualizações.</span><span class="sxs-lookup"><span data-stu-id="46883-106">You can enroll an [azureADDevice](../resources/windowsupdates-azureaddevice.md) resource in update management, but may not enroll an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) in update management.</span></span>

<span data-ttu-id="46883-107">Registrar um dispositivo do Azure AD no gerenciamento de atualizações cria automaticamente um **objeto azureADDevice** se ele ainda não existir.</span><span class="sxs-lookup"><span data-stu-id="46883-107">Enrolling an Azure AD device in update management automatically creates an **azureADDevice** object if it does not already exist.</span></span>

<span data-ttu-id="46883-108">Você também pode usar o método [enrollAssetsById para](windowsupdates-updatableasset-enrollassetsbyid.md) registrar ativos.</span><span class="sxs-lookup"><span data-stu-id="46883-108">You can also use the method [enrollAssetsById](windowsupdates-updatableasset-enrollassetsbyid.md) to enroll assets.</span></span>

## <a name="permissions"></a><span data-ttu-id="46883-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="46883-109">Permissions</span></span>
<span data-ttu-id="46883-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46883-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46883-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="46883-112">Permission type</span></span>|<span data-ttu-id="46883-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="46883-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46883-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="46883-114">Delegated (work or school account)</span></span>|<span data-ttu-id="46883-115">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46883-115">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="46883-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="46883-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46883-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46883-117">Not supported.</span></span>|
|<span data-ttu-id="46883-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="46883-118">Application</span></span>|<span data-ttu-id="46883-119">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46883-119">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="46883-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="46883-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/windows/updates/updatableAssets/enrollAssets
```

## <a name="request-headers"></a><span data-ttu-id="46883-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="46883-121">Request headers</span></span>
|<span data-ttu-id="46883-122">Nome</span><span class="sxs-lookup"><span data-stu-id="46883-122">Name</span></span>|<span data-ttu-id="46883-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="46883-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="46883-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="46883-124">Authorization</span></span>|<span data-ttu-id="46883-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46883-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="46883-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="46883-127">Content-Type</span></span>|<span data-ttu-id="46883-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46883-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="46883-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="46883-130">Request body</span></span>
<span data-ttu-id="46883-131">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="46883-131">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="46883-132">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="46883-132">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="46883-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="46883-133">Parameter</span></span>|<span data-ttu-id="46883-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="46883-134">Type</span></span>|<span data-ttu-id="46883-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="46883-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46883-136">updateCategory</span><span class="sxs-lookup"><span data-stu-id="46883-136">updateCategory</span></span>|<span data-ttu-id="46883-137">microsoft.graph.windowsUpdates.updateCategory</span><span class="sxs-lookup"><span data-stu-id="46883-137">microsoft.graph.windowsUpdates.updateCategory</span></span>|<span data-ttu-id="46883-138">A categoria de atualizações para o serviço gerenciar.</span><span class="sxs-lookup"><span data-stu-id="46883-138">The category of updates for the service to manage.</span></span> <span data-ttu-id="46883-139">Oferece suporte a um subconjunto dos valores **para updateCategory**.</span><span class="sxs-lookup"><span data-stu-id="46883-139">Supports a subset of the values for **updateCategory**.</span></span> <span data-ttu-id="46883-140">Os valores possíveis são: `feature` .</span><span class="sxs-lookup"><span data-stu-id="46883-140">Possible values are: `feature`.</span></span>|
|<span data-ttu-id="46883-141">assets</span><span class="sxs-lookup"><span data-stu-id="46883-141">assets</span></span>|<span data-ttu-id="46883-142">[coleção microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="46883-142">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="46883-143">Lista de **recursos updatableAsset** para se inscrever no gerenciamento de atualizações pelo serviço para a **atualização determinadaCategory**.</span><span class="sxs-lookup"><span data-stu-id="46883-143">List of **updatableAsset** resources to enroll in update management by the service for the given **updateCategory**.</span></span>|

## <a name="response"></a><span data-ttu-id="46883-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="46883-144">Response</span></span>

<span data-ttu-id="46883-145">Se tiver êxito, esta ação retornará um código de resposta `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="46883-145">If successful, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="46883-146">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="46883-146">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="46883-147">Exemplos</span><span class="sxs-lookup"><span data-stu-id="46883-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="46883-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="46883-148">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "updatableasset_enrollassets"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/enrollAssets
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


### <a name="response"></a><span data-ttu-id="46883-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="46883-149">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

