---
title: Criar updatableAssetGroup
description: Crie um novo objeto updatableAssetGroup.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 9e3abe53f8e18236cb83fa9105d3890bc21dcce9
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067253"
---
# <a name="create-updatableassetgroup"></a><span data-ttu-id="e4bb8-103">Criar updatableAssetGroup</span><span class="sxs-lookup"><span data-stu-id="e4bb8-103">Create updatableAssetGroup</span></span>
<span data-ttu-id="e4bb8-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="e4bb8-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4bb8-105">Crie um novo [objeto updatableAssetGroup.](../resources/windowsupdates-updatableassetgroup.md)</span><span class="sxs-lookup"><span data-stu-id="e4bb8-105">Create a new [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) object.</span></span>

<span data-ttu-id="e4bb8-106">O **recurso updatableAssetGroup** herda de [updatableAsset](../resources/windowsupdates-updatableasset.md).</span><span class="sxs-lookup"><span data-stu-id="e4bb8-106">The **updatableAssetGroup** resource inherits from [updatableAsset](../resources/windowsupdates-updatableasset.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e4bb8-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="e4bb8-107">Permissions</span></span>
<span data-ttu-id="e4bb8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4bb8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4bb8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e4bb8-110">Permission type</span></span>|<span data-ttu-id="e4bb8-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e4bb8-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4bb8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e4bb8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e4bb8-113">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4bb8-113">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="e4bb8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e4bb8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4bb8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4bb8-115">Not supported.</span></span>|
|<span data-ttu-id="e4bb8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e4bb8-116">Application</span></span>|<span data-ttu-id="e4bb8-117">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4bb8-117">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4bb8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e4bb8-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/windows/updates/updatableAssets
```

## <a name="request-headers"></a><span data-ttu-id="e4bb8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e4bb8-119">Request headers</span></span>
|<span data-ttu-id="e4bb8-120">Nome</span><span class="sxs-lookup"><span data-stu-id="e4bb8-120">Name</span></span>|<span data-ttu-id="e4bb8-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4bb8-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e4bb8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e4bb8-122">Authorization</span></span>|<span data-ttu-id="e4bb8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e4bb8-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e4bb8-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e4bb8-125">Content-Type</span></span>|<span data-ttu-id="e4bb8-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e4bb8-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4bb8-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e4bb8-128">Request body</span></span>
<span data-ttu-id="e4bb8-129">No corpo da solicitação, fornece uma representação JSON do [objeto updatableAssetGroup.](../resources/windowsupdates-updatableassetgroup.md)</span><span class="sxs-lookup"><span data-stu-id="e4bb8-129">In the request body, supply a JSON representation of the [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) object.</span></span>

<span data-ttu-id="e4bb8-130">Nenhuma propriedade é necessária.</span><span class="sxs-lookup"><span data-stu-id="e4bb8-130">No properties are required.</span></span>


## <a name="response"></a><span data-ttu-id="e4bb8-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4bb8-131">Response</span></span>

<span data-ttu-id="e4bb8-132">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e4bb8-132">If successful, this method returns a `201 Created` response code and an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e4bb8-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e4bb8-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e4bb8-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e4bb8-134">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_updatableassetgroup_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets
Content-Type: application/json
Content-length: 76

{
  "@odata.type": "#microsoft.graph.windowsUpdates.updatableAssetGroup"
}
```


### <a name="response"></a><span data-ttu-id="e4bb8-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4bb8-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsUpdates.updatableAssetGroup"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.windowsUpdates.updatableAssetGroup",
  "id": "5c55730b-730b-5c55-0b73-555c0b73555c"
}
```

