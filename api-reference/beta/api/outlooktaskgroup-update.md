---
title: Atualizar outlooktaskgroup
description: Atualizar as propriedades graváveis de um grupo de tarefas do Outlook.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 30a5ca98bf60c8d90ea8691cd229287570445d90
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36349698"
---
# <a name="update-outlooktaskgroup"></a><span data-ttu-id="f092e-103">Atualizar outlooktaskgroup</span><span class="sxs-lookup"><span data-stu-id="f092e-103">Update outlooktaskgroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f092e-104">Atualizar as propriedades graváveis de um grupo de tarefas do Outlook.</span><span class="sxs-lookup"><span data-stu-id="f092e-104">Update the writable properties of an Outlook task group.</span></span>

<span data-ttu-id="f092e-105">Observe que você não pode modificar o nome do grupo de tarefas padrão, "minhas tarefas".</span><span class="sxs-lookup"><span data-stu-id="f092e-105">Note that you cannot modify the name of the default task group, "My Tasks".</span></span>
## <a name="permissions"></a><span data-ttu-id="f092e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f092e-106">Permissions</span></span>
<span data-ttu-id="f092e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f092e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f092e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f092e-109">Permission type</span></span>      | <span data-ttu-id="f092e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f092e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f092e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f092e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f092e-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f092e-112">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="f092e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f092e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f092e-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f092e-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="f092e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f092e-115">Application</span></span> | <span data-ttu-id="f092e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f092e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f092e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f092e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/outlook/taskGroups/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskGroups/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="f092e-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="f092e-118">Optional request headers</span></span>
| <span data-ttu-id="f092e-119">Name</span><span class="sxs-lookup"><span data-stu-id="f092e-119">Name</span></span>       | <span data-ttu-id="f092e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f092e-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f092e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f092e-121">Authorization</span></span>  | <span data-ttu-id="f092e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f092e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f092e-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f092e-124">Request body</span></span>
<span data-ttu-id="f092e-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="f092e-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f092e-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f092e-128">Property</span></span>     | <span data-ttu-id="f092e-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="f092e-129">Type</span></span>   |<span data-ttu-id="f092e-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="f092e-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f092e-131">name</span><span class="sxs-lookup"><span data-stu-id="f092e-131">name</span></span>|<span data-ttu-id="f092e-132">String</span><span class="sxs-lookup"><span data-stu-id="f092e-132">String</span></span>|<span data-ttu-id="f092e-133">O nome do grupo de tarefas.</span><span class="sxs-lookup"><span data-stu-id="f092e-133">The name of the task group.</span></span>|

## <a name="response"></a><span data-ttu-id="f092e-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f092e-134">Response</span></span>

<span data-ttu-id="f092e-135">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [outlookTaskGroup](../resources/outlooktaskgroup.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f092e-135">If successful, this method returns a `200 OK` response code and updated [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f092e-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f092e-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f092e-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f092e-137">Request</span></span>
<span data-ttu-id="f092e-138">O exemplo a seguir altera o nome de um grupo de tarefas para "Tarefas Pessoais".</span><span class="sxs-lookup"><span data-stu-id="f092e-138">The following example changes the name of a task group to "Personal Tasks".</span></span> 

# <a name="httptabhttp"></a>[<span data-ttu-id="f092e-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="f092e-139">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="f092e-140">C#</span><span class="sxs-lookup"><span data-stu-id="f092e-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-outlooktaskgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f092e-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f092e-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-outlooktaskgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f092e-142">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="f092e-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-outlooktaskgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f092e-143">Java</span><span class="sxs-lookup"><span data-stu-id="f092e-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-outlooktaskgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f092e-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="f092e-144">Response</span></span>
<span data-ttu-id="f092e-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f092e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
