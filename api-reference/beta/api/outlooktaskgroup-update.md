---
title: Atualizar outlooktaskgroup
description: Atualize as propriedades graváveis de um grupo de tarefa do Outlook.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: ecea8487e0fedfdf3658d5f04c0ae8d96dcd5d93
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940411"
---
# <a name="update-outlooktaskgroup"></a><span data-ttu-id="55466-103">Atualizar outlooktaskgroup</span><span class="sxs-lookup"><span data-stu-id="55466-103">Update outlooktaskgroup</span></span>

> <span data-ttu-id="55466-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="55466-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="55466-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="55466-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="55466-106">Atualize as propriedades graváveis de um grupo de tarefa do Outlook.</span><span class="sxs-lookup"><span data-stu-id="55466-106">Update the writable properties of an Outlook task group.</span></span>

<span data-ttu-id="55466-107">Observe que você não pode modificar o nome do grupo de tarefas padrão, "Minhas tarefas".</span><span class="sxs-lookup"><span data-stu-id="55466-107">Note that you cannot modify the name of the default task group, "My Tasks".</span></span>
## <a name="permissions"></a><span data-ttu-id="55466-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="55466-108">Permissions</span></span>
<span data-ttu-id="55466-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55466-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55466-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="55466-111">Permission type</span></span>      | <span data-ttu-id="55466-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="55466-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="55466-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="55466-113">Delegated (work or school account)</span></span> | <span data-ttu-id="55466-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="55466-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="55466-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="55466-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55466-116">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="55466-116">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="55466-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="55466-117">Application</span></span> | <span data-ttu-id="55466-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55466-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="55466-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="55466-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id|userPrincipalName}/outlook/taskGroups/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="55466-120">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="55466-120">Optional request headers</span></span>
| <span data-ttu-id="55466-121">Nome</span><span class="sxs-lookup"><span data-stu-id="55466-121">Name</span></span>       | <span data-ttu-id="55466-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="55466-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="55466-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="55466-123">Authorization</span></span>  | <span data-ttu-id="55466-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="55466-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="55466-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="55466-126">Request body</span></span>
<span data-ttu-id="55466-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="55466-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="55466-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="55466-130">Property</span></span>     | <span data-ttu-id="55466-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="55466-131">Type</span></span>   |<span data-ttu-id="55466-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="55466-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="55466-133">name</span><span class="sxs-lookup"><span data-stu-id="55466-133">name</span></span>|<span data-ttu-id="55466-134">String</span><span class="sxs-lookup"><span data-stu-id="55466-134">String</span></span>|<span data-ttu-id="55466-135">O nome do grupo de tarefas.</span><span class="sxs-lookup"><span data-stu-id="55466-135">The name of the task group.</span></span>|

## <a name="response"></a><span data-ttu-id="55466-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="55466-136">Response</span></span>

<span data-ttu-id="55466-137">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto atualizado [outlookTaskGroup](../resources/outlooktaskgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="55466-137">If successful, this method returns a `200 OK` response code and updated [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="55466-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="55466-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="55466-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55466-139">Request</span></span>
<span data-ttu-id="55466-140">O exemplo a seguir altera o nome de um grupo de tarefas para "Tarefas Pessoais".</span><span class="sxs-lookup"><span data-stu-id="55466-140">The following example changes the name of a task group to "Personal Tasks".</span></span> 
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
##### <a name="response"></a><span data-ttu-id="55466-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="55466-141">Response</span></span>
<span data-ttu-id="55466-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="55466-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
