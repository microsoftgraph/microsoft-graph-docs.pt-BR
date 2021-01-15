---
title: Atualizar linkedResource
description: Atualizar as propriedades de um objeto linkedResource.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: b41e4d3948ccca6f58c1ab701367f4432b489551
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873805"
---
# <a name="update-linkedresource"></a><span data-ttu-id="66714-103">Atualizar linkedResource</span><span class="sxs-lookup"><span data-stu-id="66714-103">Update linkedResource</span></span>
<span data-ttu-id="66714-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66714-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="66714-105">Atualizar as propriedades de um [objeto linkedResource.](../resources/linkedresource.md)</span><span class="sxs-lookup"><span data-stu-id="66714-105">Update the properties of a [linkedResource](../resources/linkedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="66714-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="66714-106">Permissions</span></span>
<span data-ttu-id="66714-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66714-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66714-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="66714-109">Permission type</span></span>|<span data-ttu-id="66714-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="66714-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66714-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="66714-111">Delegated (work or school account)</span></span>|<span data-ttu-id="66714-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66714-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="66714-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="66714-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66714-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66714-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="66714-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="66714-115">Application</span></span>|<span data-ttu-id="66714-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="66714-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="66714-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="66714-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources/{linkedResourcesId}
PATCH /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources/{linkedResourcesId}
```

## <a name="request-headers"></a><span data-ttu-id="66714-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="66714-118">Request headers</span></span>
|<span data-ttu-id="66714-119">Nome</span><span class="sxs-lookup"><span data-stu-id="66714-119">Name</span></span>|<span data-ttu-id="66714-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="66714-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="66714-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="66714-121">Authorization</span></span>|<span data-ttu-id="66714-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="66714-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="66714-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="66714-124">Content-Type</span></span>|<span data-ttu-id="66714-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="66714-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="66714-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="66714-127">Request body</span></span>
<span data-ttu-id="66714-128">No corpo da solicitação, fornece uma representação JSON do [objeto linkedResource.](../resources/linkedresource.md)</span><span class="sxs-lookup"><span data-stu-id="66714-128">In the request body, supply a JSON representation of the [linkedResource](../resources/linkedresource.md) object.</span></span>

<span data-ttu-id="66714-129">A tabela a seguir mostra as propriedades que são necessárias ao atualizar [o linkedResource](../resources/linkedresource.md).</span><span class="sxs-lookup"><span data-stu-id="66714-129">The following table shows the properties that are required when you update the [linkedResource](../resources/linkedresource.md).</span></span>

|<span data-ttu-id="66714-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="66714-130">Property</span></span>|<span data-ttu-id="66714-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="66714-131">Type</span></span>|<span data-ttu-id="66714-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="66714-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66714-133">id</span><span class="sxs-lookup"><span data-stu-id="66714-133">id</span></span>|<span data-ttu-id="66714-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="66714-134">String</span></span>|<span data-ttu-id="66714-135">ID gerada pelo servidor para a entidade vinculada Herdada da [entidade](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="66714-135">Server generated Id for the linked entity Inherited from [entity](../resources/entity.md)</span></span>|

## <a name="response"></a><span data-ttu-id="66714-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="66714-136">Response</span></span>

<span data-ttu-id="66714-137">Se bem-sucedido, este método retorna um código `200 OK` de resposta e um objeto [linkedResource](../resources/linkedresource.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="66714-137">If successful, this method returns a `200 OK` response code and an updated [linkedResource](../resources/linkedresource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="66714-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="66714-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="66714-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="66714-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="66714-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="66714-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["dfsdc-f9dfdfs-dcsda9", "e2dc-f9cce2-dce29", "f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9"],
  "name": "update_linkedresource"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources/f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9
Content-Type: application/json
Content-length: 166

{
  "@odata.type": "#microsoft.graph.linkedResource",
  "webUrl": "http://microsoft.com",
  "applicationName": "Microsoft",
  "displayName": "Microsoft"
}
```
# <a name="c"></a>[<span data-ttu-id="66714-141">C#</span><span class="sxs-lookup"><span data-stu-id="66714-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-linkedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="66714-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="66714-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-linkedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="66714-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="66714-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-linkedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="66714-144">Java</span><span class="sxs-lookup"><span data-stu-id="66714-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-linkedresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="66714-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="66714-145">Response</span></span>
<span data-ttu-id="66714-146">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="66714-146">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.linkedResource"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.linkedResource",
  "id": "f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9",
  "webUrl": "http://microsoft.com",
  "applicationName": "Microsoft",
  "displayName": "Microsoft",
  "externalId": "dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9"
}
```


