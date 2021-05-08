---
title: Listar recursos updatableAssetGroup
description: Obter uma lista de objetos updatableAssetGroup e suas propriedades.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: d0529c59c00e84e122e5be3e5658c963535fd6d9
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52239250"
---
# <a name="list-updatableassetgroup-resources"></a><span data-ttu-id="f91d8-103">Listar recursos updatableAssetGroup</span><span class="sxs-lookup"><span data-stu-id="f91d8-103">List updatableAssetGroup resources</span></span>
<span data-ttu-id="f91d8-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="f91d8-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f91d8-105">Obter uma lista de [objetos updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="f91d8-105">Get a list of [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) objects and their properties.</span></span>

<span data-ttu-id="f91d8-106">Essa operação filtra o tipo de recurso totalmente `microsoft.graph.windowsUpdates.updatableAssetGroup` qualificado, , que herda de [updatableAsset](../resources/windowsupdates-updatableasset.md).</span><span class="sxs-lookup"><span data-stu-id="f91d8-106">This operation filters on the fully qualified resource type, `microsoft.graph.windowsUpdates.updatableAssetGroup`, which inherits from [updatableAsset](../resources/windowsupdates-updatableasset.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f91d8-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f91d8-107">Permissions</span></span>
<span data-ttu-id="f91d8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f91d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f91d8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f91d8-110">Permission type</span></span>|<span data-ttu-id="f91d8-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f91d8-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f91d8-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f91d8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f91d8-113">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f91d8-113">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="f91d8-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f91d8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f91d8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f91d8-115">Not supported.</span></span>|
|<span data-ttu-id="f91d8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f91d8-116">Application</span></span>|<span data-ttu-id="f91d8-117">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f91d8-117">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f91d8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f91d8-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/windows/updates/updatableAssets/?$filter=isof('microsoft.graph.windowsUpdates.updatableAssetGroup')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f91d8-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f91d8-119">Optional query parameters</span></span>
<span data-ttu-id="f91d8-120">Este método dá suporte a alguns dos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$count` , , , , , e `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="f91d8-120">This method supports some of the [OData query parameters](/graph/query-parameters) to help customize the response, including `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f91d8-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f91d8-121">Request headers</span></span>
|<span data-ttu-id="f91d8-122">Nome</span><span class="sxs-lookup"><span data-stu-id="f91d8-122">Name</span></span>|<span data-ttu-id="f91d8-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f91d8-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f91d8-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f91d8-124">Authorization</span></span>|<span data-ttu-id="f91d8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f91d8-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f91d8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f91d8-127">Request body</span></span>
<span data-ttu-id="f91d8-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f91d8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f91d8-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f91d8-129">Response</span></span>

<span data-ttu-id="f91d8-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de objetos [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f91d8-130">If successful, this method returns a `200 OK` response code and a collection of [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f91d8-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f91d8-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f91d8-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f91d8-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f91d8-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f91d8-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_updatableassetgroup"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/?$filter=isof('microsoft.graph.windowsUpdates.updatableAssetGroup')
```
# <a name="c"></a>[<span data-ttu-id="f91d8-134">C#</span><span class="sxs-lookup"><span data-stu-id="f91d8-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-updatableassetgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f91d8-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f91d8-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-updatableassetgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f91d8-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f91d8-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-updatableassetgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f91d8-137">Java</span><span class="sxs-lookup"><span data-stu-id="f91d8-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-updatableassetgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="f91d8-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="f91d8-138">Response</span></span>

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

