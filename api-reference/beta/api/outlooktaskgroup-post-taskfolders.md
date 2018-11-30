---
title: Criar outlookTaskFolder
description: Crie uma pasta de tarefas do Outlook em um outlookTaskGroup especificado.
ms.openlocfilehash: 38fbc4766a520e5d671b37b98442096ceb481fd3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27032930"
---
# <a name="create-outlooktaskfolder"></a><span data-ttu-id="4ba9a-103">Criar outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="4ba9a-103">Create outlookTaskFolder</span></span>

> <span data-ttu-id="4ba9a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4ba9a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4ba9a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4ba9a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4ba9a-106">Crie uma pasta de tarefas do Outlook em um [outlookTaskGroup](../resources/outlooktaskgroup.md)de especificado.</span><span class="sxs-lookup"><span data-stu-id="4ba9a-106">Create an Outlook task folder under a specified [outlookTaskGroup](../resources/outlooktaskgroup.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="4ba9a-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="4ba9a-107">Permissions</span></span>
<span data-ttu-id="4ba9a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ba9a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ba9a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4ba9a-110">Permission type</span></span>      | <span data-ttu-id="4ba9a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4ba9a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ba9a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4ba9a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4ba9a-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4ba9a-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="4ba9a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4ba9a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ba9a-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4ba9a-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="4ba9a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4ba9a-116">Application</span></span> | <span data-ttu-id="4ba9a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4ba9a-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4ba9a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4ba9a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders

```
## <a name="request-headers"></a><span data-ttu-id="4ba9a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4ba9a-119">Request headers</span></span>
| <span data-ttu-id="4ba9a-120">Nome</span><span class="sxs-lookup"><span data-stu-id="4ba9a-120">Name</span></span>       | <span data-ttu-id="4ba9a-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ba9a-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4ba9a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4ba9a-122">Authorization</span></span>  | <span data-ttu-id="4ba9a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4ba9a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4ba9a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4ba9a-125">Request body</span></span>
<span data-ttu-id="4ba9a-126">No corpo da solicitação, fornece uma representação JSON do objeto [outlookTaskFolder](../resources/outlooktaskfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="4ba9a-126">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="4ba9a-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ba9a-127">Response</span></span>

<span data-ttu-id="4ba9a-128">Se tiver êxito, este método retornará `201 Created` objeto response de código e [outlookTaskFolder](../resources/outlooktaskfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4ba9a-128">If successful, this method returns `201 Created` response code and [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ba9a-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4ba9a-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4ba9a-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4ba9a-130">Request</span></span>
<span data-ttu-id="4ba9a-131">O exemplo a seguir cria uma pasta de tarefas chamada `Cooking` do grupo de tarefa especificada.</span><span class="sxs-lookup"><span data-stu-id="4ba9a-131">The following example creates a task folder called `Cooking` in the specified task group.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_outlooktaskfolder_from_outlooktaskgroup"
}-->
```http
POST https://graph.microsoft.com/beta/me/taskgroups('AAMkADIyAAAhrbe-AAA')/taskfolders 

Content-type: application/json
Content-length: 131

{
  "name": "Cooking"
}
```
<span data-ttu-id="4ba9a-132">No corpo da solicitação, fornece uma representação JSON do objeto [outlookTaskFolder](../resources/outlooktaskfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="4ba9a-132">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="4ba9a-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ba9a-133">Response</span></span>
<span data-ttu-id="4ba9a-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4ba9a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskFolder"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 151

{
  "id": "AAMkADIyAAAhrbPXAAA=",
  "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAIbAOlA==",
  "isDefaultFolder": false,
  "name": "Cooking",
  "parentGroupKey": "63d640cf-946f-4734-9c29-60dda7b76acb"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create outlookTaskFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->