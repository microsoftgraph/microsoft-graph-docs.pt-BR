---
title: Obter implantação
description: Leia as propriedades e as relações de um objeto de implantação.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: e0741f449da2677696ccb30488cc0fc41ebe39c9
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241335"
---
# <a name="get-deployment"></a><span data-ttu-id="e8dca-103">Obter implantação</span><span class="sxs-lookup"><span data-stu-id="e8dca-103">Get deployment</span></span>
<span data-ttu-id="e8dca-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="e8dca-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8dca-105">Leia as propriedades e as relações de um [objeto de](../resources/windowsupdates-deployment.md) implantação.</span><span class="sxs-lookup"><span data-stu-id="e8dca-105">Read the properties and relationships of a [deployment](../resources/windowsupdates-deployment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8dca-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e8dca-106">Permissions</span></span>
<span data-ttu-id="e8dca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8dca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8dca-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8dca-109">Permission type</span></span>|<span data-ttu-id="e8dca-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e8dca-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8dca-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8dca-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e8dca-112">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8dca-112">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="e8dca-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8dca-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8dca-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8dca-114">Not supported.</span></span>|
|<span data-ttu-id="e8dca-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8dca-115">Application</span></span>|<span data-ttu-id="e8dca-116">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8dca-116">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8dca-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8dca-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/windows/updates/deployments/{deploymentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e8dca-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e8dca-118">Optional query parameters</span></span>
<span data-ttu-id="e8dca-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e8dca-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="e8dca-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="e8dca-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e8dca-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e8dca-121">Request headers</span></span>
|<span data-ttu-id="e8dca-122">Nome</span><span class="sxs-lookup"><span data-stu-id="e8dca-122">Name</span></span>|<span data-ttu-id="e8dca-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8dca-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e8dca-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e8dca-124">Authorization</span></span>|<span data-ttu-id="e8dca-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8dca-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8dca-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8dca-127">Request body</span></span>
<span data-ttu-id="e8dca-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e8dca-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8dca-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8dca-129">Response</span></span>

<span data-ttu-id="e8dca-130">Se tiver êxito, este método retornará um código de resposta e um `200 OK` objeto [de](../resources/windowsupdates-deployment.md) implantação no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e8dca-130">If successful, this method returns a `200 OK` response code and a [deployment](../resources/windowsupdates-deployment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e8dca-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e8dca-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e8dca-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8dca-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e8dca-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="e8dca-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_deployment"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/windows/updates/deployments/b5171742-1742-b517-4217-17b5421717b5
```
# <a name="c"></a>[<span data-ttu-id="e8dca-134">C#</span><span class="sxs-lookup"><span data-stu-id="e8dca-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-deployment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e8dca-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e8dca-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-deployment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e8dca-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e8dca-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-deployment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e8dca-137">Java</span><span class="sxs-lookup"><span data-stu-id="e8dca-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-deployment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="e8dca-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8dca-138">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsUpdates.deployment"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
    "id": "b5171742-1742-b517-4217-17b5421717b5",
    "state": {
      "@odata.type": "microsoft.graph.windowsUpdates.deploymentState"
    },
    "content": {
      "@odata.type": "microsoft.graph.windowsUpdates.deployableContent"
    },
    "settings": {
      "@odata.type": "microsoft.graph.windowsUpdates.deploymentSettings"
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
  }
}
```

