---
title: Criar outlookTaskGroup
description: Crie um grupo de tarefas do Outlook na caixa de correio do usuário.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 91f2aad901b67cbb419c8cf590f55f7b4a4a904b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913650"
---
# <a name="create-outlooktaskgroup"></a><span data-ttu-id="8b9dd-103">Criar outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="8b9dd-103">Create outlookTaskGroup</span></span>

> <span data-ttu-id="8b9dd-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8b9dd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8b9dd-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8b9dd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8b9dd-106">Crie um grupo de tarefas do Outlook na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="8b9dd-106">Create an Outlook task group in the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="8b9dd-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="8b9dd-107">Permissions</span></span>
<span data-ttu-id="8b9dd-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b9dd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b9dd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8b9dd-110">Permission type</span></span>      | <span data-ttu-id="8b9dd-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8b9dd-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8b9dd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8b9dd-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8b9dd-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b9dd-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="8b9dd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8b9dd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b9dd-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b9dd-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="8b9dd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8b9dd-116">Application</span></span> | <span data-ttu-id="8b9dd-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8b9dd-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b9dd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8b9dd-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/outlook/taskGroups

```
## <a name="request-headers"></a><span data-ttu-id="8b9dd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8b9dd-119">Request headers</span></span>
| <span data-ttu-id="8b9dd-120">Nome</span><span class="sxs-lookup"><span data-stu-id="8b9dd-120">Name</span></span>       | <span data-ttu-id="8b9dd-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b9dd-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8b9dd-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8b9dd-122">Authorization</span></span>  | <span data-ttu-id="8b9dd-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8b9dd-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8b9dd-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8b9dd-125">Request body</span></span>
<span data-ttu-id="8b9dd-126">No corpo da solicitação, fornece uma representação JSON do objeto [outlookTaskGroup](../resources/outlooktaskgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="8b9dd-126">In the request body, supply a JSON representation of [outlookTaskGroup](../resources/outlooktaskgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8b9dd-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b9dd-127">Response</span></span>

<span data-ttu-id="8b9dd-128">Se tiver êxito, este método retornará `201 Created` objeto response de código e [outlookTaskGroup](../resources/outlooktaskgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8b9dd-128">If successful, this method returns `201 Created` response code and [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b9dd-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8b9dd-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8b9dd-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8b9dd-130">Request</span></span>
<span data-ttu-id="8b9dd-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8b9dd-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_outlooktaskgroup_from_outlookuser"
}-->
```http
POST https://graph.microsoft.com/beta/me/outlook/taskGroups
Content-type: application/json
Content-length: 40

{
  "name": "Leisure tasks"
}
```
<span data-ttu-id="8b9dd-132">No corpo da solicitação, fornece uma representação JSON do objeto [outlookTaskGroup](../resources/outlooktaskgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="8b9dd-132">In the request body, supply a JSON representation of [outlookTaskGroup](../resources/outlooktaskgroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="8b9dd-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b9dd-133">Response</span></span>
<span data-ttu-id="8b9dd-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8b9dd-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskGroup"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 138

{
  "id": "AAMkADIyAAAhrbe-AAA=",
  "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAIbAGjg==",
  "isDefaultGroup": false,
  "name": "Leisure tasks",
  "groupKey": "63d640cf-946f-4734-9c29-60dda7b76acb"

}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create outlookTaskGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
