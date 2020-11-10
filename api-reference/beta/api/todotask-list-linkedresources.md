---
title: Listar linkedResources
description: Obtenha o linkedResources da propriedade de navegação linkedResources.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 8dff0b6872a0094703c4f46f53cee8bc48fee180
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48974362"
---
# <a name="list-linkedresources"></a><span data-ttu-id="2665a-103">Listar linkedResources</span><span class="sxs-lookup"><span data-stu-id="2665a-103">List linkedResources</span></span>
<span data-ttu-id="2665a-104">Namespace: Microsoft. Graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="2665a-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="2665a-105">Obter informações de um ou mais itens em um aplicativo parceiro, com base no qual uma [tarefa](../resources/todotask.md) especificada foi criada.</span><span class="sxs-lookup"><span data-stu-id="2665a-105">Get information of one or more items in a partner application, based on which a specified [task](../resources/todotask.md) was created.</span></span> <span data-ttu-id="2665a-106">As informações são representadas em um objeto [linkedResource](../resources/linkedresource.md) para cada item.</span><span class="sxs-lookup"><span data-stu-id="2665a-106">The information is represented in a [linkedResource](../resources/linkedresource.md) object for each item.</span></span> <span data-ttu-id="2665a-107">Ele inclui uma ID externa para o item no aplicativo parceiro e, se aplicável, um link profundo para esse item no aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2665a-107">It includes an external ID for the item in the partner application, and if applicable, a deep link to that item in the application.</span></span>

## <a name="permissions"></a><span data-ttu-id="2665a-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="2665a-108">Permissions</span></span>
<span data-ttu-id="2665a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2665a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2665a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2665a-111">Permission type</span></span>|<span data-ttu-id="2665a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2665a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2665a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2665a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2665a-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2665a-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="2665a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2665a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2665a-116">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2665a-116">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="2665a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2665a-117">Application</span></span>|<span data-ttu-id="2665a-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2665a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2665a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2665a-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
GET /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2665a-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2665a-120">Optional query parameters</span></span>
<span data-ttu-id="2665a-121">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2665a-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="2665a-122">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="2665a-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="2665a-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2665a-123">Request headers</span></span>
|<span data-ttu-id="2665a-124">Nome</span><span class="sxs-lookup"><span data-stu-id="2665a-124">Name</span></span>|<span data-ttu-id="2665a-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="2665a-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2665a-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="2665a-126">Authorization</span></span>|<span data-ttu-id="2665a-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2665a-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2665a-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2665a-129">Request body</span></span>
<span data-ttu-id="2665a-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2665a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2665a-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="2665a-131">Response</span></span>

<span data-ttu-id="2665a-132">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [linkedResource](../resources/linkedresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2665a-132">If successful, this method returns a `200 OK` response code and a collection of [linkedResource](../resources/linkedresource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2665a-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2665a-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2665a-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2665a-134">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="2665a-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="2665a-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["dfsdc-f9dfdfs-dcsda9", "e2dc-f9cce2-dce29"],
  "name": "get_linkedresource"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources
```
# <a name="c"></a>[<span data-ttu-id="2665a-136">C#</span><span class="sxs-lookup"><span data-stu-id="2665a-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-linkedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2665a-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2665a-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-linkedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2665a-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2665a-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-linkedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2665a-139">Java</span><span class="sxs-lookup"><span data-stu-id="2665a-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-linkedresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="2665a-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="2665a-140">Response</span></span>
<span data-ttu-id="2665a-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2665a-141">**Note:** The response object shown here might be shortened for readability.</span></span>
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



