---
title: Listar linkedResources
description: Obtenha o linkedResources da propriedade de navegação linkedResources.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: c3d780e05c71112ddabd1d5d6a64b22d6f771d40
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873255"
---
# <a name="list-linkedresources"></a><span data-ttu-id="458b9-103">Listar linkedResources</span><span class="sxs-lookup"><span data-stu-id="458b9-103">List linkedResources</span></span>
<span data-ttu-id="458b9-104">Namespace: Microsoft. Graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="458b9-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="458b9-105">Obtenha o linkedResources da propriedade de navegação linkedResources.</span><span class="sxs-lookup"><span data-stu-id="458b9-105">Get the linkedResources from the linkedResources navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="458b9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="458b9-106">Permissions</span></span>
<span data-ttu-id="458b9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="458b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="458b9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="458b9-109">Permission type</span></span>|<span data-ttu-id="458b9-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="458b9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="458b9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="458b9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="458b9-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="458b9-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="458b9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="458b9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="458b9-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="458b9-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="458b9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="458b9-115">Application</span></span>|<span data-ttu-id="458b9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="458b9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="458b9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="458b9-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
GET /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="458b9-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="458b9-118">Optional query parameters</span></span>
<span data-ttu-id="458b9-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="458b9-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="458b9-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="458b9-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="458b9-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="458b9-121">Request headers</span></span>
|<span data-ttu-id="458b9-122">Nome</span><span class="sxs-lookup"><span data-stu-id="458b9-122">Name</span></span>|<span data-ttu-id="458b9-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="458b9-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="458b9-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="458b9-124">Authorization</span></span>|<span data-ttu-id="458b9-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="458b9-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="458b9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="458b9-127">Request body</span></span>
<span data-ttu-id="458b9-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="458b9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="458b9-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="458b9-129">Response</span></span>

<span data-ttu-id="458b9-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [linkedResource](../resources/linkedresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="458b9-130">If successful, this method returns a `200 OK` response code and a collection of [linkedResource](../resources/linkedresource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="458b9-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="458b9-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="458b9-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="458b9-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="458b9-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="458b9-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["dfsdc-f9dfdfs-dcsda9", "e2dc-f9cce2-dce29"],
  "name": "get_linkedresource"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources
```
# <a name="c"></a>[<span data-ttu-id="458b9-134">C#</span><span class="sxs-lookup"><span data-stu-id="458b9-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-linkedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="458b9-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="458b9-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-linkedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="458b9-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="458b9-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-linkedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="458b9-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="458b9-137">Response</span></span>
<span data-ttu-id="458b9-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="458b9-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.linkedResource)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.linkedResource",
      "id": "f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9",
      "webUrl": "http:://microsoft.com",
      "applicationName": "Microsoft",
      "displayName": "Microsoft",
      "externalId": "dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9"
    }
  ]
}
```

