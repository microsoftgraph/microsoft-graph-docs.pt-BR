---
title: Obter updatableAssetGroup
description: Leia as propriedades e as relações de um objeto updatableAssetGroup.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 96019f9fac94e79e51963ce98a878799b58d918e
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52238934"
---
# <a name="get-updatableassetgroup"></a><span data-ttu-id="114c5-103">Obter updatableAssetGroup</span><span class="sxs-lookup"><span data-stu-id="114c5-103">Get updatableAssetGroup</span></span>
<span data-ttu-id="114c5-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="114c5-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="114c5-105">Leia as propriedades e as relações de um [objeto updatableAssetGroup.](../resources/windowsupdates-updatableassetgroup.md)</span><span class="sxs-lookup"><span data-stu-id="114c5-105">Read the properties and relationships of an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="114c5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="114c5-106">Permissions</span></span>
<span data-ttu-id="114c5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="114c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="114c5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="114c5-109">Permission type</span></span>|<span data-ttu-id="114c5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="114c5-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="114c5-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="114c5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="114c5-112">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="114c5-112">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="114c5-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="114c5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="114c5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="114c5-114">Not supported.</span></span>|
|<span data-ttu-id="114c5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="114c5-115">Application</span></span>|<span data-ttu-id="114c5-116">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="114c5-116">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="114c5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="114c5-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/windows/updates/updatableAssets/{updatableAssetGroupId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="114c5-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="114c5-118">Optional query parameters</span></span>
<span data-ttu-id="114c5-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="114c5-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="114c5-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="114c5-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="114c5-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="114c5-121">Request headers</span></span>
|<span data-ttu-id="114c5-122">Nome</span><span class="sxs-lookup"><span data-stu-id="114c5-122">Name</span></span>|<span data-ttu-id="114c5-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="114c5-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="114c5-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="114c5-124">Authorization</span></span>|<span data-ttu-id="114c5-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="114c5-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="114c5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="114c5-127">Request body</span></span>
<span data-ttu-id="114c5-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="114c5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="114c5-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="114c5-129">Response</span></span>

<span data-ttu-id="114c5-130">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="114c5-130">If successful, this method returns a `200 OK` response code and an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="114c5-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="114c5-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="114c5-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="114c5-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="114c5-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="114c5-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_updatableassetgroup"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/5c55730b-730b-5c55-0b73-555c0b73555c
```
# <a name="c"></a>[<span data-ttu-id="114c5-134">C#</span><span class="sxs-lookup"><span data-stu-id="114c5-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-updatableassetgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="114c5-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="114c5-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-updatableassetgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="114c5-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="114c5-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-updatableassetgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="114c5-137">Java</span><span class="sxs-lookup"><span data-stu-id="114c5-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-updatableassetgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="114c5-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="114c5-138">Response</span></span>

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

