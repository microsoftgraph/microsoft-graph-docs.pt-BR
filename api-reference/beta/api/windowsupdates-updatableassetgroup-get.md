---
title: Obter updatableAssetGroup
description: Leia as propriedades e as relações de um objeto updatableAssetGroup.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 6c31b6cb7080f053313513c60639a2d97fe1b0b9
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067890"
---
# <a name="get-updatableassetgroup"></a><span data-ttu-id="a5116-103">Obter updatableAssetGroup</span><span class="sxs-lookup"><span data-stu-id="a5116-103">Get updatableAssetGroup</span></span>
<span data-ttu-id="a5116-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="a5116-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5116-105">Leia as propriedades e as relações de um [objeto updatableAssetGroup.](../resources/windowsupdates-updatableassetgroup.md)</span><span class="sxs-lookup"><span data-stu-id="a5116-105">Read the properties and relationships of an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5116-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a5116-106">Permissions</span></span>
<span data-ttu-id="a5116-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5116-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5116-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a5116-109">Permission type</span></span>|<span data-ttu-id="a5116-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a5116-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a5116-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a5116-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a5116-112">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5116-112">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="a5116-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a5116-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5116-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a5116-114">Not supported.</span></span>|
|<span data-ttu-id="a5116-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a5116-115">Application</span></span>|<span data-ttu-id="a5116-116">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5116-116">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5116-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a5116-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/windows/updates/updatableAssets/{updatableAssetGroupId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a5116-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a5116-118">Optional query parameters</span></span>
<span data-ttu-id="a5116-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a5116-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="a5116-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a5116-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a5116-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a5116-121">Request headers</span></span>
|<span data-ttu-id="a5116-122">Nome</span><span class="sxs-lookup"><span data-stu-id="a5116-122">Name</span></span>|<span data-ttu-id="a5116-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5116-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a5116-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a5116-124">Authorization</span></span>|<span data-ttu-id="a5116-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a5116-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5116-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a5116-127">Request body</span></span>
<span data-ttu-id="a5116-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a5116-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a5116-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5116-129">Response</span></span>

<span data-ttu-id="a5116-130">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a5116-130">If successful, this method returns a `200 OK` response code and an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a5116-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a5116-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a5116-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a5116-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_updatableassetgroup"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/5c55730b-730b-5c55-0b73-555c0b73555c
```


### <a name="response"></a><span data-ttu-id="a5116-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5116-133">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsUpdates.updatableAssetGroup"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsUpdates.updatableAssetGroup",
    "id": "5c55730b-730b-5c55-0b73-555c0b73555c"
  }
}
```

