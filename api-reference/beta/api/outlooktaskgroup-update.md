---
title: Atualizar outlooktaskgroup
description: Atualizar as propriedades graváveis de um grupo de tarefas do Outlook.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: b628f0cf610afef88a198db721ee5395a34d1e08
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32539607"
---
# <a name="update-outlooktaskgroup"></a><span data-ttu-id="35fd1-103">Atualizar outlooktaskgroup</span><span class="sxs-lookup"><span data-stu-id="35fd1-103">Update outlooktaskgroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35fd1-104">Atualizar as propriedades graváveis de um grupo de tarefas do Outlook.</span><span class="sxs-lookup"><span data-stu-id="35fd1-104">Update the writable properties of an Outlook task group.</span></span>

<span data-ttu-id="35fd1-105">Observe que você não pode modificar o nome do grupo de tarefas padrão, "minhas tarefas".</span><span class="sxs-lookup"><span data-stu-id="35fd1-105">Note that you cannot modify the name of the default task group, "My Tasks".</span></span>
## <a name="permissions"></a><span data-ttu-id="35fd1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="35fd1-106">Permissions</span></span>
<span data-ttu-id="35fd1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35fd1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35fd1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="35fd1-109">Permission type</span></span>      | <span data-ttu-id="35fd1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="35fd1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="35fd1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="35fd1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="35fd1-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="35fd1-112">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="35fd1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="35fd1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="35fd1-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="35fd1-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="35fd1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="35fd1-115">Application</span></span> | <span data-ttu-id="35fd1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="35fd1-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="35fd1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="35fd1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/outlook/taskGroups/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskGroups/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="35fd1-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="35fd1-118">Optional request headers</span></span>
| <span data-ttu-id="35fd1-119">Name</span><span class="sxs-lookup"><span data-stu-id="35fd1-119">Name</span></span>       | <span data-ttu-id="35fd1-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="35fd1-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="35fd1-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="35fd1-121">Authorization</span></span>  | <span data-ttu-id="35fd1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="35fd1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="35fd1-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="35fd1-124">Request body</span></span>
<span data-ttu-id="35fd1-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="35fd1-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="35fd1-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="35fd1-128">Property</span></span>     | <span data-ttu-id="35fd1-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="35fd1-129">Type</span></span>   |<span data-ttu-id="35fd1-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="35fd1-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="35fd1-131">name</span><span class="sxs-lookup"><span data-stu-id="35fd1-131">name</span></span>|<span data-ttu-id="35fd1-132">String</span><span class="sxs-lookup"><span data-stu-id="35fd1-132">String</span></span>|<span data-ttu-id="35fd1-133">O nome do grupo de tarefas.</span><span class="sxs-lookup"><span data-stu-id="35fd1-133">The name of the task group.</span></span>|

## <a name="response"></a><span data-ttu-id="35fd1-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="35fd1-134">Response</span></span>

<span data-ttu-id="35fd1-135">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [outlookTaskGroup](../resources/outlooktaskgroup.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="35fd1-135">If successful, this method returns a `200 OK` response code and updated [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="35fd1-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="35fd1-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="35fd1-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="35fd1-137">Request</span></span>
<span data-ttu-id="35fd1-138">O exemplo a seguir altera o nome de um grupo de tarefas para "Tarefas Pessoais".</span><span class="sxs-lookup"><span data-stu-id="35fd1-138">The following example changes the name of a task group to "Personal Tasks".</span></span> 
<!-- {
  "blockType": "request",
  "name": "update_outlooktaskgroup"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/outlook/taskgroups('AAMkADIyAAAhrbe-AAA=')

Content-type: application/json
Content-length: 28

{
  "name": "Personal Tasks",
}
```
##### <a name="response"></a><span data-ttu-id="35fd1-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="35fd1-139">Response</span></span>
<span data-ttu-id="35fd1-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="35fd1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/outlooktaskgroup-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
