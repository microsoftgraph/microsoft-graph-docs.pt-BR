---
title: Criar linkedResource
description: Criar um novo objeto linkedResource.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 56ad2b1f83475cc6b5af748c129f0cd84cdc07b0
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/30/2020
ms.locfileid: "48313685"
---
# <a name="create-linkedresource"></a><span data-ttu-id="78087-103">Criar linkedResource</span><span class="sxs-lookup"><span data-stu-id="78087-103">Create linkedResource</span></span>
<span data-ttu-id="78087-104">Namespace: Microsoft. Graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="78087-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="78087-105">Criar um novo objeto **linkedResource** .</span><span class="sxs-lookup"><span data-stu-id="78087-105">Create a new **linkedResource** object.</span></span>

<span data-ttu-id="78087-106">Você também pode criar um objeto **linkedResource** ao [criar um todoTask](/graph/api/todotasklist-post-tasks?view=graph-rest-beta&preserve-view=true&tabs=http#examples).</span><span class="sxs-lookup"><span data-stu-id="78087-106">You can also create a **linkedResource** object while [creating a todoTask](/graph/api/todotasklist-post-tasks?view=graph-rest-beta&preserve-view=true&tabs=http#examples).</span></span>

## <a name="permissions"></a><span data-ttu-id="78087-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="78087-107">Permissions</span></span>
<span data-ttu-id="78087-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78087-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78087-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="78087-110">Permission type</span></span>|<span data-ttu-id="78087-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="78087-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="78087-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="78087-112">Delegated (work or school account)</span></span>|<span data-ttu-id="78087-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="78087-113">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="78087-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="78087-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="78087-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="78087-115">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="78087-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="78087-116">Application</span></span>|<span data-ttu-id="78087-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="78087-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="78087-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="78087-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
POST /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
```

## <a name="request-headers"></a><span data-ttu-id="78087-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="78087-119">Request headers</span></span>
|<span data-ttu-id="78087-120">Nome</span><span class="sxs-lookup"><span data-stu-id="78087-120">Name</span></span>|<span data-ttu-id="78087-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="78087-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="78087-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="78087-122">Authorization</span></span>|<span data-ttu-id="78087-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="78087-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="78087-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="78087-125">Content-Type</span></span>|<span data-ttu-id="78087-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="78087-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="78087-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="78087-128">Request body</span></span>
<span data-ttu-id="78087-129">No corpo da solicitação, forneça uma representação JSON do objeto [linkedResource](../resources/linkedresource.md) .</span><span class="sxs-lookup"><span data-stu-id="78087-129">In the request body, supply a JSON representation of the [linkedResource](../resources/linkedresource.md) object.</span></span>

<span data-ttu-id="78087-130">A tabela a seguir mostra as propriedades que são necessárias ao criar [linkedResource](../resources/linkedresource.md).</span><span class="sxs-lookup"><span data-stu-id="78087-130">The following table shows the properties that are required when you create the [linkedResource](../resources/linkedresource.md).</span></span>

|<span data-ttu-id="78087-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="78087-131">Property</span></span>|<span data-ttu-id="78087-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="78087-132">Type</span></span>|<span data-ttu-id="78087-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="78087-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78087-134">id</span><span class="sxs-lookup"><span data-stu-id="78087-134">id</span></span>|<span data-ttu-id="78087-135">String</span><span class="sxs-lookup"><span data-stu-id="78087-135">String</span></span>|<span data-ttu-id="78087-136">ID gerada pelo servidor para a entidade vinculada herdada da [entidade](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="78087-136">Server generated Id for the linked entity Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="78087-137">webUrl</span><span class="sxs-lookup"><span data-stu-id="78087-137">webUrl</span></span>|<span data-ttu-id="78087-138">String</span><span class="sxs-lookup"><span data-stu-id="78087-138">String</span></span>|<span data-ttu-id="78087-139">Deeplink para a entidade vinculada</span><span class="sxs-lookup"><span data-stu-id="78087-139">Deeplink to the linked entity</span></span> |
|<span data-ttu-id="78087-140">applicationName</span><span class="sxs-lookup"><span data-stu-id="78087-140">applicationName</span></span>|<span data-ttu-id="78087-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="78087-141">String</span></span>|<span data-ttu-id="78087-142">Campo que indica o nome do aplicativo da fonte que está enviando a entidade vinculada</span><span class="sxs-lookup"><span data-stu-id="78087-142">Field indicating app name of the source that is sending the linked entity</span></span> |
|<span data-ttu-id="78087-143">displayName</span><span class="sxs-lookup"><span data-stu-id="78087-143">displayName</span></span>|<span data-ttu-id="78087-144">String</span><span class="sxs-lookup"><span data-stu-id="78087-144">String</span></span>|<span data-ttu-id="78087-145">Campo indicando o título da entidade vinculada.</span><span class="sxs-lookup"><span data-stu-id="78087-145">Field indicating title of the linked entity.</span></span> |
|<span data-ttu-id="78087-146">externalId</span><span class="sxs-lookup"><span data-stu-id="78087-146">externalId</span></span>|<span data-ttu-id="78087-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="78087-147">String</span></span>|<span data-ttu-id="78087-148">ID do objeto associado a essa tarefa no sistema de terceiros/parceiros</span><span class="sxs-lookup"><span data-stu-id="78087-148">Id of the object that is associated with this task on the third-party/partner system</span></span> |



## <a name="response"></a><span data-ttu-id="78087-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="78087-149">Response</span></span>

<span data-ttu-id="78087-150">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [linkedResource](../resources/linkedresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="78087-150">If successful, this method returns a `201 Created` response code and a [linkedResource](../resources/linkedresource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="78087-151">Exemplos</span><span class="sxs-lookup"><span data-stu-id="78087-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="78087-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="78087-152">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="78087-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="78087-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["dfsdc-f9dfdfs-dcsda9", "e2dc-f9cce2-dce29"],
  "name": "create_linkedresource_from_linkedresources"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources
Content-Type: application/json
Content-length: 166

{
  "webUrl": "https://microsoft.com",
  "applicationName": "Microsoft",
  "displayName": "Microsoft",
  "externalId": "dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9"
}
```
# <a name="javascript"></a>[<span data-ttu-id="78087-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="78087-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-linkedresource-from-linkedresources-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="78087-155">C#</span><span class="sxs-lookup"><span data-stu-id="78087-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-linkedresource-from-linkedresources-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="78087-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="78087-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-linkedresource-from-linkedresources-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="78087-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="78087-157">Response</span></span>
<span data-ttu-id="78087-158">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="78087-158">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.linkedResource"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.linkedResource",
  "id": "f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9",
  "webUrl": "http:://microsoft.com",
  "applicationName": "Microsoft",
  "displayName": "Microsoft",
  "externalId": "dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9"
}
```



