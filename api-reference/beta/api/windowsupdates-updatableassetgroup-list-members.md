---
title: Listar membros do grupo de ativos atualizáveis
description: Listar os membros de um recurso updatableAssetGroup. Os membros são do tipo azureADDevice.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 747bf224d4dfbddf0d7845e3ca6f4d23e48912d1
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52266663"
---
# <a name="list-updatable-asset-group-members"></a><span data-ttu-id="47edd-104">Listar membros do grupo de ativos atualizáveis</span><span class="sxs-lookup"><span data-stu-id="47edd-104">List updatable asset group members</span></span>
<span data-ttu-id="47edd-105">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="47edd-105">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="47edd-106">Listar os membros de [um recurso updatableAssetGroup.](../resources/windowsupdates-updatableassetgroup.md)</span><span class="sxs-lookup"><span data-stu-id="47edd-106">List the members of an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) resource.</span></span> <span data-ttu-id="47edd-107">Os membros são do tipo [azureADDevice.](../resources/windowsupdates-azureaddevice.md)</span><span class="sxs-lookup"><span data-stu-id="47edd-107">Members are of the [azureADDevice](../resources/windowsupdates-azureaddevice.md) type.</span></span>

<span data-ttu-id="47edd-108">Esta operação faz referência à **propriedade de navegação members** de um recurso **updatableAssetGroup.**</span><span class="sxs-lookup"><span data-stu-id="47edd-108">This operation references the **members** navigation property of an **updatableAssetGroup** resource.</span></span> <span data-ttu-id="47edd-109">Para fazer referência a uma propriedade de um tipo derivado de [updatableAsset](../resources/windowsupdates-updatableasset.md), inclua o tipo de recurso derivado completo na URL de consulta, ou seja, `.../microsoft.graph.windowsUpdates.updatableAssetGroup/members` .</span><span class="sxs-lookup"><span data-stu-id="47edd-109">To reference a property of a type derived from [updatableAsset](../resources/windowsupdates-updatableasset.md), include the full derived resource type in the query URL, i.e., `.../microsoft.graph.windowsUpdates.updatableAssetGroup/members`.</span></span>

## <a name="permissions"></a><span data-ttu-id="47edd-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="47edd-110">Permissions</span></span>
<span data-ttu-id="47edd-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47edd-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47edd-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="47edd-113">Permission type</span></span>|<span data-ttu-id="47edd-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="47edd-114">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47edd-115">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="47edd-115">Delegated (work or school account)</span></span>|<span data-ttu-id="47edd-116">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47edd-116">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="47edd-117">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="47edd-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47edd-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47edd-118">Not supported.</span></span>|
|<span data-ttu-id="47edd-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="47edd-119">Application</span></span>|<span data-ttu-id="47edd-120">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47edd-120">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="47edd-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="47edd-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/windows/updates/updatableAssets/{updatableAssetGroupId}/microsoft.graph.windowsUpdates.updatableAssetGroup/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="47edd-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="47edd-122">Optional query parameters</span></span>
<span data-ttu-id="47edd-123">Este método dá suporte a alguns dos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$count` , , , , , e `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="47edd-123">This method supports some of the [OData query parameters](/graph/query-parameters) to help customize the response, including `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

<span data-ttu-id="47edd-124">Para usar um parâmetro de consulta em uma propriedade que não seja herdada de [updatableAsset](../resources/windowsupdates-updatableasset.md), inclua o tipo de recurso completo para a propriedade.</span><span class="sxs-lookup"><span data-stu-id="47edd-124">To use a query parameter on a property that is not inherited from [updatableAsset](../resources/windowsupdates-updatableasset.md), include the full resource type for the property.</span></span> <span data-ttu-id="47edd-125">Por exemplo, para aplicar `$select` na propriedade **errors** do [azureADDevice,](../resources/windowsupdates-azureaddevice.md)use `$select=microsoft.graph.windowsUpdates.azureADDevice/errors` .</span><span class="sxs-lookup"><span data-stu-id="47edd-125">For example, to apply `$select` on the **errors** property of [azureADDevice](../resources/windowsupdates-azureaddevice.md), use `$select=microsoft.graph.windowsUpdates.azureADDevice/errors`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="47edd-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="47edd-126">Request headers</span></span>
|<span data-ttu-id="47edd-127">Nome</span><span class="sxs-lookup"><span data-stu-id="47edd-127">Name</span></span>|<span data-ttu-id="47edd-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="47edd-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="47edd-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="47edd-129">Authorization</span></span>|<span data-ttu-id="47edd-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="47edd-p106">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="47edd-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="47edd-132">Request body</span></span>
<span data-ttu-id="47edd-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="47edd-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47edd-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="47edd-134">Response</span></span>

<span data-ttu-id="47edd-135">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de objetos [updatableAsset](../resources/windowsupdates-updatableasset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="47edd-135">If successful, this method returns a `200 OK` response code and a collection of [updatableAsset](../resources/windowsupdates-updatableasset.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="47edd-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="47edd-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="47edd-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="47edd-137">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="47edd-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="47edd-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_updatableasset"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/{updatableAssetGroupId}/microsoft.graph.windowsUpdates.updatableAssetGroup/members
```
# <a name="c"></a>[<span data-ttu-id="47edd-139">C#</span><span class="sxs-lookup"><span data-stu-id="47edd-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-updatableasset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="47edd-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="47edd-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-updatableasset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="47edd-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="47edd-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-updatableasset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="47edd-142">Java</span><span class="sxs-lookup"><span data-stu-id="47edd-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-updatableasset-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="47edd-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="47edd-143">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.windowsUpdates.updatableAsset)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "f5ba7065-7065-f5ba-6570-baf56570baf5"
    },
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "6d49dfaf-9c24-42f7-9628-c136e35774c8"
    },
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "1f61492e-4e34-4dee-904a-0d38299e76b2"
    },
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "bfe3c2d1-4cef-4952-8c5e-30d56ccf0cdc"
    }
  ]
}
```

