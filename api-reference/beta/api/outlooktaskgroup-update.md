---
title: Atualizar outlooktaskgroup
description: Atualize as propriedades graváveis de um grupo de tarefa do Outlook.
author: angelgolfer-ms
ms.openlocfilehash: 40d146f90bf512ec9afa8790d7f02d4039dd53cc
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334899"
---
# <a name="update-outlooktaskgroup"></a><span data-ttu-id="bfd4c-103">Atualizar outlooktaskgroup</span><span class="sxs-lookup"><span data-stu-id="bfd4c-103">Update outlooktaskgroup</span></span>

> <span data-ttu-id="bfd4c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bfd4c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bfd4c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bfd4c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bfd4c-106">Atualize as propriedades graváveis de um grupo de tarefa do Outlook.</span><span class="sxs-lookup"><span data-stu-id="bfd4c-106">Update the writable properties of an Outlook task group.</span></span>

<span data-ttu-id="bfd4c-107">Observe que você não pode modificar o nome do grupo de tarefas padrão, "Minhas tarefas".</span><span class="sxs-lookup"><span data-stu-id="bfd4c-107">Note that you cannot modify the name of the default task group, "My Tasks".</span></span>
## <a name="permissions"></a><span data-ttu-id="bfd4c-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="bfd4c-108">Permissions</span></span>
<span data-ttu-id="bfd4c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bfd4c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bfd4c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bfd4c-111">Permission type</span></span>      | <span data-ttu-id="bfd4c-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bfd4c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bfd4c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bfd4c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="bfd4c-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bfd4c-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="bfd4c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bfd4c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bfd4c-116">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bfd4c-116">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="bfd4c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bfd4c-117">Application</span></span> | <span data-ttu-id="bfd4c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bfd4c-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bfd4c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bfd4c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id|userPrincipalName}/outlook/taskGroups/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="bfd4c-120">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="bfd4c-120">Optional request headers</span></span>
| <span data-ttu-id="bfd4c-121">Nome</span><span class="sxs-lookup"><span data-stu-id="bfd4c-121">Name</span></span>       | <span data-ttu-id="bfd4c-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="bfd4c-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="bfd4c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bfd4c-123">Authorization</span></span>  | <span data-ttu-id="bfd4c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bfd4c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bfd4c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bfd4c-126">Request body</span></span>
<span data-ttu-id="bfd4c-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="bfd4c-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="bfd4c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bfd4c-130">Property</span></span>     | <span data-ttu-id="bfd4c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="bfd4c-131">Type</span></span>   |<span data-ttu-id="bfd4c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="bfd4c-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bfd4c-133">name</span><span class="sxs-lookup"><span data-stu-id="bfd4c-133">name</span></span>|<span data-ttu-id="bfd4c-134">String</span><span class="sxs-lookup"><span data-stu-id="bfd4c-134">String</span></span>|<span data-ttu-id="bfd4c-135">O nome do grupo de tarefas.</span><span class="sxs-lookup"><span data-stu-id="bfd4c-135">The name of the task group.</span></span>|

## <a name="response"></a><span data-ttu-id="bfd4c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="bfd4c-136">Response</span></span>

<span data-ttu-id="bfd4c-137">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto atualizado [outlookTaskGroup](../resources/outlooktaskgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bfd4c-137">If successful, this method returns a `200 OK` response code and updated [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bfd4c-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bfd4c-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bfd4c-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bfd4c-139">Request</span></span>
<span data-ttu-id="bfd4c-140">O exemplo a seguir altera o nome de um grupo de tarefas para "Tarefas Pessoais".</span><span class="sxs-lookup"><span data-stu-id="bfd4c-140">The following example changes the name of a task group to "Personal Tasks".</span></span> 
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
##### <a name="response"></a><span data-ttu-id="bfd4c-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="bfd4c-141">Response</span></span>
<span data-ttu-id="bfd4c-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bfd4c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update outlooktaskgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->