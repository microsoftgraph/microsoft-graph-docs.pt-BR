---
title: Criar linkedResource
description: Criar um novo objeto linkedResource.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 899f2b39c0a73a774c6c8df6da4aa80eb3f06fc7
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872923"
---
# <a name="create-linkedresource"></a><span data-ttu-id="052c5-103">Criar linkedResource</span><span class="sxs-lookup"><span data-stu-id="052c5-103">Create linkedResource</span></span>
<span data-ttu-id="052c5-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="052c5-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="052c5-105">Crie um [objeto linkedResource](../resources/linkedresource.md) para associar uma tarefa [especificada](../resources/todotask.md) a um item em um aplicativo parceiro.</span><span class="sxs-lookup"><span data-stu-id="052c5-105">Create a [linkedResource](../resources/linkedresource.md) object to associate a specified [task](../resources/todotask.md) with an item in a partner application.</span></span> <span data-ttu-id="052c5-106">Por exemplo, você pode associar uma tarefa a um item de email no Outlook que gerou a tarefa e pode criar um objeto **linkedResource** para controlar sua associação.</span><span class="sxs-lookup"><span data-stu-id="052c5-106">For example, you can associate a task with an email item in Outlook that spurred the task, and you can create a **linkedResource** object to track its association.</span></span>

<span data-ttu-id="052c5-107">Você também pode criar um **objeto linkedResource** ao [criar um todoTask](/graph/api/todotasklist-post-tasks?view=graph-rest-beta&preserve-view=true&tabs=http#examples).</span><span class="sxs-lookup"><span data-stu-id="052c5-107">You can also create a **linkedResource** object while [creating a todoTask](/graph/api/todotasklist-post-tasks?view=graph-rest-beta&preserve-view=true&tabs=http#examples).</span></span>

## <a name="permissions"></a><span data-ttu-id="052c5-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="052c5-108">Permissions</span></span>
<span data-ttu-id="052c5-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="052c5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="052c5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="052c5-111">Permission type</span></span>|<span data-ttu-id="052c5-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="052c5-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="052c5-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="052c5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="052c5-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="052c5-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="052c5-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="052c5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="052c5-116">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="052c5-116">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="052c5-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="052c5-117">Application</span></span>|<span data-ttu-id="052c5-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="052c5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="052c5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="052c5-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
POST /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
```

## <a name="request-headers"></a><span data-ttu-id="052c5-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="052c5-120">Request headers</span></span>
|<span data-ttu-id="052c5-121">Nome</span><span class="sxs-lookup"><span data-stu-id="052c5-121">Name</span></span>|<span data-ttu-id="052c5-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="052c5-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="052c5-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="052c5-123">Authorization</span></span>|<span data-ttu-id="052c5-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="052c5-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="052c5-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="052c5-126">Content-Type</span></span>|<span data-ttu-id="052c5-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="052c5-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="052c5-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="052c5-129">Request body</span></span>
<span data-ttu-id="052c5-130">No corpo da solicitação, fornece uma representação JSON do [objeto linkedResource.](../resources/linkedresource.md)</span><span class="sxs-lookup"><span data-stu-id="052c5-130">In the request body, supply a JSON representation of the [linkedResource](../resources/linkedresource.md) object.</span></span>

<span data-ttu-id="052c5-131">A tabela a seguir mostra as propriedades que são necessárias ao criar [linkedResource](../resources/linkedresource.md).</span><span class="sxs-lookup"><span data-stu-id="052c5-131">The following table shows the properties that are required when you create the [linkedResource](../resources/linkedresource.md).</span></span>

|<span data-ttu-id="052c5-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="052c5-132">Property</span></span>|<span data-ttu-id="052c5-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="052c5-133">Type</span></span>|<span data-ttu-id="052c5-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="052c5-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="052c5-135">id</span><span class="sxs-lookup"><span data-stu-id="052c5-135">id</span></span>|<span data-ttu-id="052c5-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="052c5-136">String</span></span>|<span data-ttu-id="052c5-137">ID gerada pelo servidor para a entidade vinculada Herdada da [entidade](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="052c5-137">Server generated Id for the linked entity Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="052c5-138">webUrl</span><span class="sxs-lookup"><span data-stu-id="052c5-138">webUrl</span></span>|<span data-ttu-id="052c5-139">String</span><span class="sxs-lookup"><span data-stu-id="052c5-139">String</span></span>|<span data-ttu-id="052c5-140">Deeplink para a entidade vinculada</span><span class="sxs-lookup"><span data-stu-id="052c5-140">Deeplink to the linked entity</span></span> |
|<span data-ttu-id="052c5-141">applicationName</span><span class="sxs-lookup"><span data-stu-id="052c5-141">applicationName</span></span>|<span data-ttu-id="052c5-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="052c5-142">String</span></span>|<span data-ttu-id="052c5-143">Campo indicando o nome do aplicativo da fonte que está enviando a entidade vinculada</span><span class="sxs-lookup"><span data-stu-id="052c5-143">Field indicating app name of the source that is sending the linked entity</span></span> |
|<span data-ttu-id="052c5-144">displayName</span><span class="sxs-lookup"><span data-stu-id="052c5-144">displayName</span></span>|<span data-ttu-id="052c5-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="052c5-145">String</span></span>|<span data-ttu-id="052c5-146">Campo que indica o título da entidade vinculada.</span><span class="sxs-lookup"><span data-stu-id="052c5-146">Field indicating title of the linked entity.</span></span> |
|<span data-ttu-id="052c5-147">externalId</span><span class="sxs-lookup"><span data-stu-id="052c5-147">externalId</span></span>|<span data-ttu-id="052c5-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="052c5-148">String</span></span>|<span data-ttu-id="052c5-149">ID do objeto que está associado a essa tarefa no sistema de terceiros/parceiro</span><span class="sxs-lookup"><span data-stu-id="052c5-149">Id of the object that is associated with this task on the third-party/partner system</span></span> |



## <a name="response"></a><span data-ttu-id="052c5-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="052c5-150">Response</span></span>

<span data-ttu-id="052c5-151">Se bem-sucedido, este método retorna um código de resposta e um objeto `201 Created` [linkedResource](../resources/linkedresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="052c5-151">If successful, this method returns a `201 Created` response code and a [linkedResource](../resources/linkedresource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="052c5-152">Exemplos</span><span class="sxs-lookup"><span data-stu-id="052c5-152">Examples</span></span>

### <a name="request"></a><span data-ttu-id="052c5-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="052c5-153">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="052c5-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="052c5-154">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="052c5-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="052c5-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-linkedresource-from-linkedresources-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="052c5-156">C#</span><span class="sxs-lookup"><span data-stu-id="052c5-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-linkedresource-from-linkedresources-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="052c5-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="052c5-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-linkedresource-from-linkedresources-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="052c5-158">Java</span><span class="sxs-lookup"><span data-stu-id="052c5-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-linkedresource-from-linkedresources-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="052c5-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="052c5-159">Response</span></span>
<span data-ttu-id="052c5-160">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="052c5-160">**Note:** The response object shown here might be shortened for readability.</span></span>
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



