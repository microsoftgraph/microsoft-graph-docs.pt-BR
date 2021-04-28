---
title: Listar recursos updatableAssetGroup
description: Obter uma lista de objetos updatableAssetGroup e suas propriedades.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 4ae3141880a0ded7677184ecdb55d3dd6e554a5f
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067284"
---
# <a name="list-updatableassetgroup-resources"></a><span data-ttu-id="c3c8e-103">Listar recursos updatableAssetGroup</span><span class="sxs-lookup"><span data-stu-id="c3c8e-103">List updatableAssetGroup resources</span></span>
<span data-ttu-id="c3c8e-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="c3c8e-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3c8e-105">Obter uma lista de [objetos updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="c3c8e-105">Get a list of [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) objects and their properties.</span></span>

<span data-ttu-id="c3c8e-106">Essa operação filtra o tipo de recurso totalmente `microsoft.graph.windowsUpdates.updatableAssetGroup` qualificado, , que herda de [updatableAsset](../resources/windowsupdates-updatableasset.md).</span><span class="sxs-lookup"><span data-stu-id="c3c8e-106">This operation filters on the fully qualified resource type, `microsoft.graph.windowsUpdates.updatableAssetGroup`, which inherits from [updatableAsset](../resources/windowsupdates-updatableasset.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c3c8e-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="c3c8e-107">Permissions</span></span>
<span data-ttu-id="c3c8e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3c8e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3c8e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c3c8e-110">Permission type</span></span>|<span data-ttu-id="c3c8e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c3c8e-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3c8e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c3c8e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c3c8e-113">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3c8e-113">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="c3c8e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c3c8e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3c8e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c3c8e-115">Not supported.</span></span>|
|<span data-ttu-id="c3c8e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c3c8e-116">Application</span></span>|<span data-ttu-id="c3c8e-117">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3c8e-117">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3c8e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c3c8e-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/windows/updates/updatableAssets/?$filter=isof('microsoft.graph.windowsUpdates.updatableAssetGroup')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c3c8e-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c3c8e-119">Optional query parameters</span></span>
<span data-ttu-id="c3c8e-120">Este método dá suporte a alguns dos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$count` , , , , , e `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="c3c8e-120">This method supports some of the [OData query parameters](/graph/query-parameters) to help customize the response, including `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c3c8e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c3c8e-121">Request headers</span></span>
|<span data-ttu-id="c3c8e-122">Nome</span><span class="sxs-lookup"><span data-stu-id="c3c8e-122">Name</span></span>|<span data-ttu-id="c3c8e-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3c8e-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c3c8e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="c3c8e-124">Authorization</span></span>|<span data-ttu-id="c3c8e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c3c8e-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3c8e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c3c8e-127">Request body</span></span>
<span data-ttu-id="c3c8e-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c3c8e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c3c8e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3c8e-129">Response</span></span>

<span data-ttu-id="c3c8e-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de objetos [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c3c8e-130">If successful, this method returns a `200 OK` response code and a collection of [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c3c8e-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c3c8e-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c3c8e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c3c8e-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_updatableassetgroup"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/?$filter=isof('microsoft.graph.windowsUpdates.updatableAssetGroup')
```


### <a name="response"></a><span data-ttu-id="c3c8e-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3c8e-133">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.windowsUpdates.updatableAssetGroup)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.updatableAssetGroup",
      "id": "5c55730b-730b-5c55-0b73-555c0b73555c"
    },
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.updatableAssetGroup",
      "id": "deb43c16-77ff-465d-aa79-366a107a6c7a"
    },
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.updatableAssetGroup",
      "id": "312643e6-b805-419f-bdf7-1a104dd6c8b9"
    }
  ]
}
```

