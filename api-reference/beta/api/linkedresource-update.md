---
title: Atualizar linkedResource
description: Atualiza as propriedades de um objeto linkedResource.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 0e80010f88dd52b9dbd44430ae251dcecab8e33c
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/07/2020
ms.locfileid: "48373857"
---
# <a name="update-linkedresource"></a><span data-ttu-id="2ffad-103">Atualizar linkedResource</span><span class="sxs-lookup"><span data-stu-id="2ffad-103">Update linkedResource</span></span>
<span data-ttu-id="2ffad-104">Namespace: Microsoft. Graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="2ffad-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="2ffad-105">Atualiza as propriedades de um objeto [linkedResource](../resources/linkedresource.md) .</span><span class="sxs-lookup"><span data-stu-id="2ffad-105">Update the properties of a [linkedResource](../resources/linkedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2ffad-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2ffad-106">Permissions</span></span>
<span data-ttu-id="2ffad-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ffad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ffad-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2ffad-109">Permission type</span></span>|<span data-ttu-id="2ffad-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2ffad-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ffad-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2ffad-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2ffad-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2ffad-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="2ffad-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2ffad-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ffad-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2ffad-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="2ffad-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2ffad-115">Application</span></span>|<span data-ttu-id="2ffad-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2ffad-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ffad-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2ffad-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources/{linkedResourcesId}
PATCH /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources/{linkedResourcesId}
```

## <a name="request-headers"></a><span data-ttu-id="2ffad-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2ffad-118">Request headers</span></span>
|<span data-ttu-id="2ffad-119">Nome</span><span class="sxs-lookup"><span data-stu-id="2ffad-119">Name</span></span>|<span data-ttu-id="2ffad-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ffad-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2ffad-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="2ffad-121">Authorization</span></span>|<span data-ttu-id="2ffad-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2ffad-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="2ffad-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2ffad-124">Content-Type</span></span>|<span data-ttu-id="2ffad-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2ffad-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ffad-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2ffad-127">Request body</span></span>
<span data-ttu-id="2ffad-128">No corpo da solicitação, forneça uma representação JSON do objeto [linkedResource](../resources/linkedresource.md) .</span><span class="sxs-lookup"><span data-stu-id="2ffad-128">In the request body, supply a JSON representation of the [linkedResource](../resources/linkedresource.md) object.</span></span>

<span data-ttu-id="2ffad-129">A tabela a seguir mostra as propriedades que são necessárias ao atualizar o [linkedResource](../resources/linkedresource.md).</span><span class="sxs-lookup"><span data-stu-id="2ffad-129">The following table shows the properties that are required when you update the [linkedResource](../resources/linkedresource.md).</span></span>

|<span data-ttu-id="2ffad-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2ffad-130">Property</span></span>|<span data-ttu-id="2ffad-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ffad-131">Type</span></span>|<span data-ttu-id="2ffad-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ffad-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ffad-133">id</span><span class="sxs-lookup"><span data-stu-id="2ffad-133">id</span></span>|<span data-ttu-id="2ffad-134">String</span><span class="sxs-lookup"><span data-stu-id="2ffad-134">String</span></span>|<span data-ttu-id="2ffad-135">ID gerada pelo servidor para a entidade vinculada herdada da [entidade](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="2ffad-135">Server generated Id for the linked entity Inherited from [entity](../resources/entity.md)</span></span>|

## <a name="response"></a><span data-ttu-id="2ffad-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ffad-136">Response</span></span>

<span data-ttu-id="2ffad-137">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [linkedResource](../resources/linkedresource.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2ffad-137">If successful, this method returns a `200 OK` response code and an updated [linkedResource](../resources/linkedresource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2ffad-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2ffad-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2ffad-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2ffad-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="2ffad-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ffad-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["dfsdc-f9dfdfs-dcsda9", "e2dc-f9cce2-dce29", "f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9"],
  "name": "update_linkedresource"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources/f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9
Content-Type: application/json
Content-length: 166

{
  "@odata.type": "#microsoft.graph.linkedResource",
  "webUrl": "http://microsoft.com",
  "applicationName": "Microsoft",
  "displayName": "Microsoft"
}
```
# <a name="javascript"></a>[<span data-ttu-id="2ffad-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ffad-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-linkedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="2ffad-142">C#</span><span class="sxs-lookup"><span data-stu-id="2ffad-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-linkedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2ffad-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2ffad-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-linkedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2ffad-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ffad-144">Response</span></span>
<span data-ttu-id="2ffad-145">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2ffad-145">**Note:** The response object shown here might be shortened for readability.</span></span>
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


