---
title: Atualizar outlooktaskgroup
description: Atualize as propriedades writable de um grupo de Outlook tarefa.
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 37bf87e8d52ac320d29fd7be1f6cdd3dae7165ea
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049202"
---
# <a name="update-outlooktaskgroup-deprecated"></a><span data-ttu-id="b2c08-103">Atualizar outlooktaskgroup (preterido)</span><span class="sxs-lookup"><span data-stu-id="b2c08-103">Update outlooktaskgroup (deprecated)</span></span>

<span data-ttu-id="b2c08-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2c08-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="b2c08-105">Atualize as propriedades writable de um grupo de Outlook tarefa.</span><span class="sxs-lookup"><span data-stu-id="b2c08-105">Update the writable properties of an Outlook task group.</span></span>

<span data-ttu-id="b2c08-106">Observe que você não pode modificar o nome do grupo de tarefas padrão, "Minhas Tarefas".</span><span class="sxs-lookup"><span data-stu-id="b2c08-106">Note that you cannot modify the name of the default task group, "My Tasks".</span></span>
## <a name="permissions"></a><span data-ttu-id="b2c08-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="b2c08-107">Permissions</span></span>
<span data-ttu-id="b2c08-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2c08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2c08-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b2c08-110">Permission type</span></span>      | <span data-ttu-id="b2c08-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b2c08-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b2c08-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b2c08-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b2c08-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b2c08-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="b2c08-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b2c08-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b2c08-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b2c08-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="b2c08-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b2c08-116">Application</span></span> | <span data-ttu-id="b2c08-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2c08-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b2c08-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b2c08-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/outlook/taskGroups/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskGroups/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="b2c08-119">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="b2c08-119">Optional request headers</span></span>
| <span data-ttu-id="b2c08-120">Nome</span><span class="sxs-lookup"><span data-stu-id="b2c08-120">Name</span></span>       | <span data-ttu-id="b2c08-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2c08-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="b2c08-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b2c08-122">Authorization</span></span>  | <span data-ttu-id="b2c08-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b2c08-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b2c08-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b2c08-125">Request body</span></span>
<span data-ttu-id="b2c08-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="b2c08-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b2c08-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b2c08-129">Property</span></span>     | <span data-ttu-id="b2c08-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b2c08-130">Type</span></span>   |<span data-ttu-id="b2c08-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2c08-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b2c08-132">nome</span><span class="sxs-lookup"><span data-stu-id="b2c08-132">name</span></span>|<span data-ttu-id="b2c08-133">String</span><span class="sxs-lookup"><span data-stu-id="b2c08-133">String</span></span>|<span data-ttu-id="b2c08-134">O nome do grupo de tarefas.</span><span class="sxs-lookup"><span data-stu-id="b2c08-134">The name of the task group.</span></span>|

## <a name="response"></a><span data-ttu-id="b2c08-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2c08-135">Response</span></span>

<span data-ttu-id="b2c08-136">Se tiver êxito, este método retornará um código `200 OK` de resposta e o objeto [outlookTaskGroup](../resources/outlooktaskgroup.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b2c08-136">If successful, this method returns a `200 OK` response code and updated [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b2c08-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b2c08-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b2c08-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b2c08-138">Request</span></span>
<span data-ttu-id="b2c08-139">O exemplo a seguir altera o nome de um grupo de tarefas para "Tarefas Pessoais".</span><span class="sxs-lookup"><span data-stu-id="b2c08-139">The following example changes the name of a task group to "Personal Tasks".</span></span> 

# <a name="http"></a>[<span data-ttu-id="b2c08-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="b2c08-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_outlooktaskgroup"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/outlook/taskgroups/AAMkADIyAAAhrbe-AAA=
Content-type: application/json
Content-length: 28

{
  "name": "Personal Tasks",
}
```
# <a name="c"></a>[<span data-ttu-id="b2c08-141">C#</span><span class="sxs-lookup"><span data-stu-id="b2c08-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-outlooktaskgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b2c08-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b2c08-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-outlooktaskgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b2c08-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b2c08-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-outlooktaskgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b2c08-144">Java</span><span class="sxs-lookup"><span data-stu-id="b2c08-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-outlooktaskgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b2c08-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2c08-145">Response</span></span>
<span data-ttu-id="b2c08-146">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b2c08-146">Here is an example of the response.</span></span> <span data-ttu-id="b2c08-147">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b2c08-147">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskGroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 138

{
  "id": "AAMkADIyAAAhrbe-AAA=",
  "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAIbAGjw==",
  "isDefaultGroup": false,
  "name": "Personal Tasks",
  "groupKey": "63d640cf-946f-4734-9c29-60dda7b76acb"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update outlooktaskgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


