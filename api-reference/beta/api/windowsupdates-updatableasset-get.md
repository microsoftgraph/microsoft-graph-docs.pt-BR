---
title: Obter updatableAsset
description: Leia as propriedades e as relações de um objeto updatableAsset.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: d89622adca8c28ebae52afa492eb233f0c1c0c72
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241196"
---
# <a name="get-updatableasset"></a><span data-ttu-id="e45ef-103">Obter updatableAsset</span><span class="sxs-lookup"><span data-stu-id="e45ef-103">Get updatableAsset</span></span>
<span data-ttu-id="e45ef-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="e45ef-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e45ef-105">Leia as propriedades e as relações de um [objeto updatableAsset.](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="e45ef-105">Read the properties and relationships of an [updatableAsset](../resources/windowsupdates-updatableasset.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e45ef-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e45ef-106">Permissions</span></span>
<span data-ttu-id="e45ef-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e45ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e45ef-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e45ef-109">Permission type</span></span>|<span data-ttu-id="e45ef-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e45ef-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e45ef-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e45ef-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e45ef-112">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e45ef-112">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="e45ef-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e45ef-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e45ef-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e45ef-114">Not supported.</span></span>|
|<span data-ttu-id="e45ef-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e45ef-115">Application</span></span>|<span data-ttu-id="e45ef-116">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e45ef-116">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e45ef-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e45ef-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/windows/updates/updatableAssets/{updatableAssetId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e45ef-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e45ef-118">Optional query parameters</span></span>
<span data-ttu-id="e45ef-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e45ef-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="e45ef-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="e45ef-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

<span data-ttu-id="e45ef-121">Para usar um parâmetro de consulta em uma propriedade que não seja herdada de [updatableAsset](../resources/windowsupdates-updatableasset.md), inclua o tipo de recurso completo para a propriedade.</span><span class="sxs-lookup"><span data-stu-id="e45ef-121">To use a query parameter on a property that is not inherited from [updatableAsset](../resources/windowsupdates-updatableasset.md), include the full resource type for the property.</span></span> <span data-ttu-id="e45ef-122">Por exemplo, para aplicar `$select` na propriedade **errors** do [azureADDevice,](../resources/windowsupdates-azureaddevice.md)use `$select=microsoft.graph.windowsUpdates.azureADDevice/errors` .</span><span class="sxs-lookup"><span data-stu-id="e45ef-122">For example, to apply `$select` on the **errors** property of [azureADDevice](../resources/windowsupdates-azureaddevice.md), use `$select=microsoft.graph.windowsUpdates.azureADDevice/errors`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e45ef-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e45ef-123">Request headers</span></span>
|<span data-ttu-id="e45ef-124">Nome</span><span class="sxs-lookup"><span data-stu-id="e45ef-124">Name</span></span>|<span data-ttu-id="e45ef-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="e45ef-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e45ef-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="e45ef-126">Authorization</span></span>|<span data-ttu-id="e45ef-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e45ef-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e45ef-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e45ef-129">Request body</span></span>
<span data-ttu-id="e45ef-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e45ef-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e45ef-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="e45ef-131">Response</span></span>

<span data-ttu-id="e45ef-132">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto updatableAsset](../resources/windowsupdates-updatableasset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e45ef-132">If successful, this method returns a `200 OK` response code and an [updatableAsset](../resources/windowsupdates-updatableasset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e45ef-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e45ef-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e45ef-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e45ef-134">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e45ef-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="e45ef-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_updatableasset"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/{updatableAssetId}
```
# <a name="c"></a>[<span data-ttu-id="e45ef-136">C#</span><span class="sxs-lookup"><span data-stu-id="e45ef-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-updatableasset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e45ef-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e45ef-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-updatableasset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e45ef-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e45ef-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-updatableasset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e45ef-139">Java</span><span class="sxs-lookup"><span data-stu-id="e45ef-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-updatableasset-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="e45ef-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="e45ef-140">Response</span></span>

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

