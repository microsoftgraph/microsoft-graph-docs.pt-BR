---
title: Atualizar outlooktaskgroup
description: Atualizar as propriedades graváveis de um grupo de tarefas do Outlook.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 75e41f92b28d4ca8ab2114e0fc7fd346ad49d16f
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35267785"
---
# <a name="update-outlooktaskgroup"></a><span data-ttu-id="d56bf-103">Atualizar outlooktaskgroup</span><span class="sxs-lookup"><span data-stu-id="d56bf-103">Update outlooktaskgroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d56bf-104">Atualizar as propriedades graváveis de um grupo de tarefas do Outlook.</span><span class="sxs-lookup"><span data-stu-id="d56bf-104">Update the writable properties of an Outlook task group.</span></span>

<span data-ttu-id="d56bf-105">Observe que você não pode modificar o nome do grupo de tarefas padrão, "minhas tarefas".</span><span class="sxs-lookup"><span data-stu-id="d56bf-105">Note that you cannot modify the name of the default task group, "My Tasks".</span></span>
## <a name="permissions"></a><span data-ttu-id="d56bf-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d56bf-106">Permissions</span></span>
<span data-ttu-id="d56bf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d56bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d56bf-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d56bf-109">Permission type</span></span>      | <span data-ttu-id="d56bf-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d56bf-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d56bf-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d56bf-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d56bf-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d56bf-112">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="d56bf-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d56bf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d56bf-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d56bf-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="d56bf-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d56bf-115">Application</span></span> | <span data-ttu-id="d56bf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d56bf-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d56bf-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d56bf-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/outlook/taskGroups/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskGroups/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="d56bf-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="d56bf-118">Optional request headers</span></span>
| <span data-ttu-id="d56bf-119">Name</span><span class="sxs-lookup"><span data-stu-id="d56bf-119">Name</span></span>       | <span data-ttu-id="d56bf-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d56bf-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="d56bf-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d56bf-121">Authorization</span></span>  | <span data-ttu-id="d56bf-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d56bf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d56bf-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d56bf-124">Request body</span></span>
<span data-ttu-id="d56bf-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="d56bf-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d56bf-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d56bf-128">Property</span></span>     | <span data-ttu-id="d56bf-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="d56bf-129">Type</span></span>   |<span data-ttu-id="d56bf-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="d56bf-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d56bf-131">name</span><span class="sxs-lookup"><span data-stu-id="d56bf-131">name</span></span>|<span data-ttu-id="d56bf-132">String</span><span class="sxs-lookup"><span data-stu-id="d56bf-132">String</span></span>|<span data-ttu-id="d56bf-133">O nome do grupo de tarefas.</span><span class="sxs-lookup"><span data-stu-id="d56bf-133">The name of the task group.</span></span>|

## <a name="response"></a><span data-ttu-id="d56bf-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d56bf-134">Response</span></span>

<span data-ttu-id="d56bf-135">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [outlookTaskGroup](../resources/outlooktaskgroup.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d56bf-135">If successful, this method returns a `200 OK` response code and updated [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d56bf-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d56bf-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d56bf-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d56bf-137">Request</span></span>
<span data-ttu-id="d56bf-138">O exemplo a seguir altera o nome de um grupo de tarefas para "Tarefas Pessoais".</span><span class="sxs-lookup"><span data-stu-id="d56bf-138">The following example changes the name of a task group to "Personal Tasks".</span></span> 
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
##### <a name="response"></a><span data-ttu-id="d56bf-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="d56bf-139">Response</span></span>
<span data-ttu-id="d56bf-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d56bf-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="d56bf-143">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="d56bf-143">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d56bf-144">C#</span><span class="sxs-lookup"><span data-stu-id="d56bf-144">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_outlooktaskgroup-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d56bf-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="d56bf-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_outlooktaskgroup-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d56bf-146">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d56bf-146">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_outlooktaskgroup-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/outlooktaskgroup-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/outlooktaskgroup-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/outlooktaskgroup-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
