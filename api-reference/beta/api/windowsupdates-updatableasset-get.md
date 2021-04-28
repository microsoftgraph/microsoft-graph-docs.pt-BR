---
title: Obter updatableAsset
description: Leia as propriedades e as relações de um objeto updatableAsset.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: ac33b00cc44c11339a75215cbbb20effc1e82a7f
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067269"
---
# <a name="get-updatableasset"></a><span data-ttu-id="1b5a0-103">Obter updatableAsset</span><span class="sxs-lookup"><span data-stu-id="1b5a0-103">Get updatableAsset</span></span>
<span data-ttu-id="1b5a0-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="1b5a0-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b5a0-105">Leia as propriedades e as relações de um [objeto updatableAsset.](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="1b5a0-105">Read the properties and relationships of an [updatableAsset](../resources/windowsupdates-updatableasset.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1b5a0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1b5a0-106">Permissions</span></span>
<span data-ttu-id="1b5a0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b5a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b5a0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1b5a0-109">Permission type</span></span>|<span data-ttu-id="1b5a0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1b5a0-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1b5a0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1b5a0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1b5a0-112">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b5a0-112">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="1b5a0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1b5a0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1b5a0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1b5a0-114">Not supported.</span></span>|
|<span data-ttu-id="1b5a0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1b5a0-115">Application</span></span>|<span data-ttu-id="1b5a0-116">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b5a0-116">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1b5a0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1b5a0-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/windows/updates/updatableAssets/{updatableAssetId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1b5a0-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1b5a0-118">Optional query parameters</span></span>
<span data-ttu-id="1b5a0-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1b5a0-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="1b5a0-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1b5a0-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

<span data-ttu-id="1b5a0-121">Para usar um parâmetro de consulta em uma propriedade que não seja herdada de [updatableAsset](../resources/windowsupdates-updatableasset.md), inclua o tipo de recurso completo para a propriedade.</span><span class="sxs-lookup"><span data-stu-id="1b5a0-121">To use a query parameter on a property that is not inherited from [updatableAsset](../resources/windowsupdates-updatableasset.md), include the full resource type for the property.</span></span> <span data-ttu-id="1b5a0-122">Por exemplo, para aplicar `$select` na propriedade **errors** do [azureADDevice,](../resources/windowsupdates-azureaddevice.md)use `$select=microsoft.graph.windowsUpdates.azureADDevice/errors` .</span><span class="sxs-lookup"><span data-stu-id="1b5a0-122">For example, to apply `$select` on the **errors** property of [azureADDevice](../resources/windowsupdates-azureaddevice.md), use `$select=microsoft.graph.windowsUpdates.azureADDevice/errors`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1b5a0-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1b5a0-123">Request headers</span></span>
|<span data-ttu-id="1b5a0-124">Nome</span><span class="sxs-lookup"><span data-stu-id="1b5a0-124">Name</span></span>|<span data-ttu-id="1b5a0-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b5a0-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1b5a0-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="1b5a0-126">Authorization</span></span>|<span data-ttu-id="1b5a0-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1b5a0-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b5a0-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1b5a0-129">Request body</span></span>
<span data-ttu-id="1b5a0-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1b5a0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1b5a0-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b5a0-131">Response</span></span>

<span data-ttu-id="1b5a0-132">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto updatableAsset](../resources/windowsupdates-updatableasset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1b5a0-132">If successful, this method returns a `200 OK` response code and an [updatableAsset](../resources/windowsupdates-updatableasset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1b5a0-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1b5a0-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1b5a0-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1b5a0-134">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_updatableasset"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/{updatableAssetId}
```


### <a name="response"></a><span data-ttu-id="1b5a0-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b5a0-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsUpdates.updatableAsset"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsUpdates.updatableAsset",
    "id": "f5ba7065-7065-f5ba-6570-baf56570baf5"
  }
}
```

