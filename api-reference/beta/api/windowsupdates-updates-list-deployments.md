---
title: Listar implantações
description: Obter uma lista de objetos de implantação e suas propriedades.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 4eda89bc8f9bbdd2ec65f6701347f79989cdebff
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52239149"
---
# <a name="list-deployments"></a><span data-ttu-id="94c74-103">Listar implantações</span><span class="sxs-lookup"><span data-stu-id="94c74-103">List deployments</span></span>
<span data-ttu-id="94c74-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="94c74-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94c74-105">Obter uma lista de [objetos de implantação](../resources/windowsupdates-deployment.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="94c74-105">Get a list of [deployment](../resources/windowsupdates-deployment.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="94c74-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="94c74-106">Permissions</span></span>
<span data-ttu-id="94c74-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94c74-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94c74-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="94c74-109">Permission type</span></span>|<span data-ttu-id="94c74-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="94c74-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="94c74-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="94c74-111">Delegated (work or school account)</span></span>|<span data-ttu-id="94c74-112">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94c74-112">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="94c74-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="94c74-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="94c74-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94c74-114">Not supported.</span></span>|
|<span data-ttu-id="94c74-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="94c74-115">Application</span></span>|<span data-ttu-id="94c74-116">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94c74-116">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="94c74-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="94c74-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/windows/updates/deployments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="94c74-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="94c74-118">Optional query parameters</span></span>
<span data-ttu-id="94c74-119">Este método dá suporte a alguns dos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$count` , , , , , e `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="94c74-119">This method supports some of the [OData query parameters](/graph/query-parameters) to help customize the response, including `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="94c74-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="94c74-120">Request headers</span></span>
|<span data-ttu-id="94c74-121">Nome</span><span class="sxs-lookup"><span data-stu-id="94c74-121">Name</span></span>|<span data-ttu-id="94c74-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="94c74-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="94c74-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="94c74-123">Authorization</span></span>|<span data-ttu-id="94c74-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94c74-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="94c74-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="94c74-126">Request body</span></span>
<span data-ttu-id="94c74-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="94c74-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94c74-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="94c74-128">Response</span></span>

<span data-ttu-id="94c74-129">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de objetos de [implantação](../resources/windowsupdates-deployment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94c74-129">If successful, this method returns a `200 OK` response code and a collection of [deployment](../resources/windowsupdates-deployment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="94c74-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="94c74-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="94c74-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="94c74-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="94c74-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="94c74-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_deployment"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/windows/updates/deployments
```
# <a name="c"></a>[<span data-ttu-id="94c74-133">C#</span><span class="sxs-lookup"><span data-stu-id="94c74-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-deployment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="94c74-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94c74-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-deployment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="94c74-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="94c74-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-deployment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="94c74-136">Java</span><span class="sxs-lookup"><span data-stu-id="94c74-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-deployment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="94c74-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="94c74-137">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.windowsUpdates.deployment)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
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
  ]
}
```

