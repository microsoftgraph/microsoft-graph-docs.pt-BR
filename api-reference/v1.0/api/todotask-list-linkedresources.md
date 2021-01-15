---
title: Listar linkedResources
description: Obter o linkedResources da propriedade de navegação linkedResources.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 827c0f0065239a89dc1fb4197eb59ddf1b26d18a
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49874407"
---
# <a name="list-linkedresources"></a><span data-ttu-id="6cb4f-103">Listar linkedResources</span><span class="sxs-lookup"><span data-stu-id="6cb4f-103">List linkedResources</span></span>
<span data-ttu-id="6cb4f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6cb4f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6cb4f-105">Obter informações de um ou mais itens em um aplicativo parceiro, com base no qual uma tarefa [especificada](../resources/todotask.md) foi criada.</span><span class="sxs-lookup"><span data-stu-id="6cb4f-105">Get information of one or more items in a partner application, based on which a specified [task](../resources/todotask.md) was created.</span></span> <span data-ttu-id="6cb4f-106">As informações são representadas em um [objeto linkedResource](../resources/linkedresource.md) para cada item.</span><span class="sxs-lookup"><span data-stu-id="6cb4f-106">The information is represented in a [linkedResource](../resources/linkedresource.md) object for each item.</span></span> <span data-ttu-id="6cb4f-107">Ele inclui uma ID externa para o item no aplicativo parceiro e, se aplicável, um link profundo para esse item no aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6cb4f-107">It includes an external ID for the item in the partner application, and if applicable, a deep link to that item in the application.</span></span>

## <a name="permissions"></a><span data-ttu-id="6cb4f-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="6cb4f-108">Permissions</span></span>
<span data-ttu-id="6cb4f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6cb4f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6cb4f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6cb4f-111">Permission type</span></span>|<span data-ttu-id="6cb4f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6cb4f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6cb4f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6cb4f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6cb4f-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6cb4f-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="6cb4f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6cb4f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6cb4f-116">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6cb4f-116">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="6cb4f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6cb4f-117">Application</span></span>|<span data-ttu-id="6cb4f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6cb4f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6cb4f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6cb4f-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
GET /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6cb4f-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6cb4f-120">Optional query parameters</span></span>
<span data-ttu-id="6cb4f-121">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6cb4f-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="6cb4f-122">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="6cb4f-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6cb4f-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6cb4f-123">Request headers</span></span>
|<span data-ttu-id="6cb4f-124">Nome</span><span class="sxs-lookup"><span data-stu-id="6cb4f-124">Name</span></span>|<span data-ttu-id="6cb4f-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="6cb4f-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6cb4f-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="6cb4f-126">Authorization</span></span>|<span data-ttu-id="6cb4f-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6cb4f-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6cb4f-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6cb4f-129">Request body</span></span>
<span data-ttu-id="6cb4f-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6cb4f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6cb4f-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="6cb4f-131">Response</span></span>

<span data-ttu-id="6cb4f-132">Se bem-sucedido, este método retorna um código de resposta e uma `200 OK` coleção de [objetos linkedResource](../resources/linkedresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6cb4f-132">If successful, this method returns a `200 OK` response code and a collection of [linkedResource](../resources/linkedresource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6cb4f-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6cb4f-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6cb4f-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6cb4f-134">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="6cb4f-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="6cb4f-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["dfsdc-f9dfdfs-dcsda9", "e2dc-f9cce2-dce29"],
  "name": "get_linkedresource"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources
```
# <a name="c"></a>[<span data-ttu-id="6cb4f-136">C#</span><span class="sxs-lookup"><span data-stu-id="6cb4f-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-linkedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6cb4f-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6cb4f-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-linkedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6cb4f-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6cb4f-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-linkedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6cb4f-139">Java</span><span class="sxs-lookup"><span data-stu-id="6cb4f-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-linkedresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="6cb4f-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="6cb4f-140">Response</span></span>
<span data-ttu-id="6cb4f-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6cb4f-141">**Note:** The response object shown here might be shortened for readability.</span></span>
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



