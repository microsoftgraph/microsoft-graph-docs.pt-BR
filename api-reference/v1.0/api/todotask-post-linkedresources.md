---
title: Criar linkedResource
description: Criar um novo objeto linkedResource.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: f915765192cf039c2095bac7e64a573d9b43b595
ms.sourcegitcommit: d9457ac1b8c2e8ac4b9604dd9e116fd547d2bfbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/29/2020
ms.locfileid: "48797178"
---
# <a name="create-linkedresource"></a><span data-ttu-id="0970e-103">Criar linkedResource</span><span class="sxs-lookup"><span data-stu-id="0970e-103">Create linkedResource</span></span>
<span data-ttu-id="0970e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0970e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0970e-105">Crie um objeto [linkedResource](../resources/linkedresource.md) para associar uma [tarefa](../resources/todotask.md) especificada a um item em um aplicativo parceiro.</span><span class="sxs-lookup"><span data-stu-id="0970e-105">Create a [linkedResource](../resources/linkedresource.md) object to associate a specified [task](../resources/todotask.md) with an item in a partner application.</span></span> <span data-ttu-id="0970e-106">Por exemplo, você pode associar uma tarefa a um item de email no Outlook que spurred a tarefa e pode criar um objeto **linkedResource** para controlar sua associação.</span><span class="sxs-lookup"><span data-stu-id="0970e-106">For example, you can associate a task with an email item in Outlook that spurred the task, and you can create a **linkedResource** object to track its association.</span></span>

<span data-ttu-id="0970e-107">Você também pode criar um objeto **linkedResource** ao [criar uma tarefa](/graph/api/todotasklist-post-tasks?view=graph-rest-beta&preserve-view=true&tabs=http#examples).</span><span class="sxs-lookup"><span data-stu-id="0970e-107">You can also create a **linkedResource** object while [creating a task](/graph/api/todotasklist-post-tasks?view=graph-rest-beta&preserve-view=true&tabs=http#examples).</span></span>

## <a name="permissions"></a><span data-ttu-id="0970e-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="0970e-108">Permissions</span></span>
<span data-ttu-id="0970e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0970e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0970e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0970e-111">Permission type</span></span>|<span data-ttu-id="0970e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0970e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0970e-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0970e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0970e-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0970e-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="0970e-115">Delegada (conta Microsoft pessoal)</span><span class="sxs-lookup"><span data-stu-id="0970e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0970e-116">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0970e-116">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="0970e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0970e-117">Application</span></span>|<span data-ttu-id="0970e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0970e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0970e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0970e-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
POST /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources
```

## <a name="request-headers"></a><span data-ttu-id="0970e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0970e-120">Request headers</span></span>
|<span data-ttu-id="0970e-121">Nome</span><span class="sxs-lookup"><span data-stu-id="0970e-121">Name</span></span>|<span data-ttu-id="0970e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="0970e-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0970e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0970e-123">Authorization</span></span>|<span data-ttu-id="0970e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0970e-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="0970e-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0970e-126">Content-Type</span></span>|<span data-ttu-id="0970e-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0970e-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0970e-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0970e-129">Request body</span></span>
<span data-ttu-id="0970e-130">No corpo da solicitação, forneça uma representação JSON do objeto [linkedResource](../resources/linkedresource.md) .</span><span class="sxs-lookup"><span data-stu-id="0970e-130">In the request body, supply a JSON representation of the [linkedResource](../resources/linkedresource.md) object.</span></span>

<span data-ttu-id="0970e-131">A tabela a seguir mostra as propriedades que são necessárias ao criar [linkedResource](../resources/linkedresource.md).</span><span class="sxs-lookup"><span data-stu-id="0970e-131">The following table shows the properties that are required when you create the [linkedResource](../resources/linkedresource.md).</span></span>

|<span data-ttu-id="0970e-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0970e-132">Property</span></span>|<span data-ttu-id="0970e-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="0970e-133">Type</span></span>|<span data-ttu-id="0970e-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="0970e-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0970e-135">id</span><span class="sxs-lookup"><span data-stu-id="0970e-135">id</span></span>|<span data-ttu-id="0970e-136">String</span><span class="sxs-lookup"><span data-stu-id="0970e-136">String</span></span>|<span data-ttu-id="0970e-137">ID gerada pelo servidor para a entidade vinculada herdada da [entidade](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="0970e-137">Server generated Id for the linked entity Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="0970e-138">webUrl</span><span class="sxs-lookup"><span data-stu-id="0970e-138">webUrl</span></span>|<span data-ttu-id="0970e-139">String</span><span class="sxs-lookup"><span data-stu-id="0970e-139">String</span></span>|<span data-ttu-id="0970e-140">Deeplink para a entidade vinculada</span><span class="sxs-lookup"><span data-stu-id="0970e-140">Deeplink to the linked entity</span></span> |
|<span data-ttu-id="0970e-141">applicationName</span><span class="sxs-lookup"><span data-stu-id="0970e-141">applicationName</span></span>|<span data-ttu-id="0970e-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0970e-142">String</span></span>|<span data-ttu-id="0970e-143">Campo que indica o nome do aplicativo da fonte que está enviando a entidade vinculada</span><span class="sxs-lookup"><span data-stu-id="0970e-143">Field indicating app name of the source that is sending the linked entity</span></span> |
|<span data-ttu-id="0970e-144">displayName</span><span class="sxs-lookup"><span data-stu-id="0970e-144">displayName</span></span>|<span data-ttu-id="0970e-145">String</span><span class="sxs-lookup"><span data-stu-id="0970e-145">String</span></span>|<span data-ttu-id="0970e-146">Campo indicando o título da entidade vinculada.</span><span class="sxs-lookup"><span data-stu-id="0970e-146">Field indicating title of the linked entity.</span></span> |
|<span data-ttu-id="0970e-147">externalId</span><span class="sxs-lookup"><span data-stu-id="0970e-147">externalId</span></span>|<span data-ttu-id="0970e-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0970e-148">String</span></span>|<span data-ttu-id="0970e-149">ID do objeto associado a essa tarefa no sistema de terceiros/parceiros</span><span class="sxs-lookup"><span data-stu-id="0970e-149">Id of the object that is associated with this task on the third-party/partner system</span></span> |



## <a name="response"></a><span data-ttu-id="0970e-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="0970e-150">Response</span></span>

<span data-ttu-id="0970e-151">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [linkedResource](../resources/linkedresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0970e-151">If successful, this method returns a `201 Created` response code and a [linkedResource](../resources/linkedresource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0970e-152">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0970e-152">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0970e-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0970e-153">Request</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["dfsdc-f9dfdfs-dcsda9", "e2dc-f9cce2-dce29"],
  "name": "create_linkedresource_from_linkedresources"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources
Content-Type: application/json
Content-length: 166

{
  "webUrl": "https://microsoft.com",
  "applicationName": "Microsoft",
  "displayName": "Microsoft",
  "externalId": "dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9"
}
```


### <a name="response"></a><span data-ttu-id="0970e-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="0970e-154">Response</span></span>
<span data-ttu-id="0970e-155">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0970e-155">**Note:** The response object shown here might be shortened for readability.</span></span>
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



