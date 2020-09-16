---
title: Criar linkedResources
description: Criar um novo objeto linkedResources.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: d55a63848d26bccb8bee5f6931d42bc85f95c2ef
ms.sourcegitcommit: 7e1993d64cc6d3145ae0ca984fefe74772b6052b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/16/2020
ms.locfileid: "47843097"
---
# <a name="create-linkedresources"></a><span data-ttu-id="7355e-103">Criar linkedResources</span><span class="sxs-lookup"><span data-stu-id="7355e-103">Create linkedResources</span></span>
<span data-ttu-id="7355e-104">Namespace: Microsoft. Graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="7355e-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="7355e-105">Criar um novo objeto linkedResources.</span><span class="sxs-lookup"><span data-stu-id="7355e-105">Create a new linkedResources object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7355e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7355e-106">Permissions</span></span>
<span data-ttu-id="7355e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7355e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7355e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7355e-109">Permission type</span></span>|<span data-ttu-id="7355e-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7355e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7355e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7355e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7355e-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7355e-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="7355e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7355e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7355e-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7355e-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="7355e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7355e-115">Application</span></span>|<span data-ttu-id="7355e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7355e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7355e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7355e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
POST /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
```

## <a name="request-headers"></a><span data-ttu-id="7355e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7355e-118">Request headers</span></span>
|<span data-ttu-id="7355e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="7355e-119">Name</span></span>|<span data-ttu-id="7355e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="7355e-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7355e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7355e-121">Authorization</span></span>|<span data-ttu-id="7355e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7355e-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="7355e-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7355e-124">Content-Type</span></span>|<span data-ttu-id="7355e-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7355e-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7355e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7355e-127">Request body</span></span>
<span data-ttu-id="7355e-128">No corpo da solicitação, forneça uma representação JSON do objeto [linkedResource](../resources/linkedresource.md) .</span><span class="sxs-lookup"><span data-stu-id="7355e-128">In the request body, supply a JSON representation of the [linkedResource](../resources/linkedresource.md) object.</span></span>

<span data-ttu-id="7355e-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [linkedResource](../resources/linkedresource.md).</span><span class="sxs-lookup"><span data-stu-id="7355e-129">The following table shows the properties that are required when you create the [linkedResource](../resources/linkedresource.md).</span></span>

|<span data-ttu-id="7355e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7355e-130">Property</span></span>|<span data-ttu-id="7355e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7355e-131">Type</span></span>|<span data-ttu-id="7355e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7355e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7355e-133">id</span><span class="sxs-lookup"><span data-stu-id="7355e-133">id</span></span>|<span data-ttu-id="7355e-134">String</span><span class="sxs-lookup"><span data-stu-id="7355e-134">String</span></span>|<span data-ttu-id="7355e-135">ID gerada pelo servidor para a entidade vinculada herdada da [entidade](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="7355e-135">Server generated Id for the linked entity Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="7355e-136">webUrl</span><span class="sxs-lookup"><span data-stu-id="7355e-136">webUrl</span></span>|<span data-ttu-id="7355e-137">String</span><span class="sxs-lookup"><span data-stu-id="7355e-137">String</span></span>|<span data-ttu-id="7355e-138">Deeplink para a entidade vinculada</span><span class="sxs-lookup"><span data-stu-id="7355e-138">Deeplink to the linked entity</span></span> |
|<span data-ttu-id="7355e-139">applicationName</span><span class="sxs-lookup"><span data-stu-id="7355e-139">applicationName</span></span>|<span data-ttu-id="7355e-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7355e-140">String</span></span>|<span data-ttu-id="7355e-141">Campo que indica o nome do aplicativo da fonte que está enviando a entidade vinculada</span><span class="sxs-lookup"><span data-stu-id="7355e-141">Field indicating app name of the source that is sending the linked entity</span></span> |
|<span data-ttu-id="7355e-142">displayName</span><span class="sxs-lookup"><span data-stu-id="7355e-142">displayName</span></span>|<span data-ttu-id="7355e-143">String</span><span class="sxs-lookup"><span data-stu-id="7355e-143">String</span></span>|<span data-ttu-id="7355e-144">Campo indicando o título da entidade vinculada.</span><span class="sxs-lookup"><span data-stu-id="7355e-144">Field indicating title of the linked entity.</span></span> |
|<span data-ttu-id="7355e-145">externalId</span><span class="sxs-lookup"><span data-stu-id="7355e-145">externalId</span></span>|<span data-ttu-id="7355e-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7355e-146">String</span></span>|<span data-ttu-id="7355e-147">ID do objeto associado a essa tarefa no sistema de terceiros/parceiros</span><span class="sxs-lookup"><span data-stu-id="7355e-147">Id of the object that is associated with this task on the third-party/partner system</span></span> |



## <a name="response"></a><span data-ttu-id="7355e-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="7355e-148">Response</span></span>

<span data-ttu-id="7355e-149">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [linkedResource](../resources/linkedresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7355e-149">If successful, this method returns a `201 Created` response code and a [linkedResource](../resources/linkedresource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7355e-150">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7355e-150">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7355e-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7355e-151">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7355e-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="7355e-152">HTTP</span></span>](#tab/http)
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
  "@odata.type": "#microsoft.graph.linkedResource",
  "webUrl": "http:://microsoft.com",
  "applicationName": "Microsoft",
  "displayName": "Microsoft",
  "externalId": "dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9"
}
```
# <a name="javascript"></a>[<span data-ttu-id="7355e-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7355e-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-linkedresource-from-linkedresources-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="7355e-154">C#</span><span class="sxs-lookup"><span data-stu-id="7355e-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-linkedresource-from-linkedresources-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7355e-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7355e-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-linkedresource-from-linkedresources-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="7355e-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="7355e-156">Response</span></span>
<span data-ttu-id="7355e-157">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7355e-157">**Note:** The response object shown here might be shortened for readability.</span></span>
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

