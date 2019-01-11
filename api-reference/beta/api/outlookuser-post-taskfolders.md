---
title: Criar outlookTaskFolder
description: Crie uma pasta de tarefa no grupo de tarefa padrão (`My Tasks`) da caixa de correio do usuário.
localization_priority: Normal
ms.openlocfilehash: d863786028f29419d6e20d8be7c18d6b37250e25
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832562"
---
# <a name="create-outlooktaskfolder"></a><span data-ttu-id="ebcee-103">Criar outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="ebcee-103">Create outlookTaskFolder</span></span>

> <span data-ttu-id="ebcee-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ebcee-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ebcee-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ebcee-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ebcee-106">Crie uma pasta de tarefa no grupo de tarefa padrão (`My Tasks`) da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="ebcee-106">Create a task folder in the default task group (`My Tasks`) of the user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="ebcee-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="ebcee-107">Permissions</span></span>
<span data-ttu-id="ebcee-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ebcee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebcee-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ebcee-110">Permission type</span></span>      | <span data-ttu-id="ebcee-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ebcee-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ebcee-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ebcee-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ebcee-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ebcee-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="ebcee-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ebcee-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ebcee-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ebcee-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="ebcee-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ebcee-116">Application</span></span> | <span data-ttu-id="ebcee-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ebcee-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ebcee-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ebcee-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/outlook/taskFolders

```
## <a name="request-headers"></a><span data-ttu-id="ebcee-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ebcee-119">Request headers</span></span>
| <span data-ttu-id="ebcee-120">Nome</span><span class="sxs-lookup"><span data-stu-id="ebcee-120">Name</span></span>       | <span data-ttu-id="ebcee-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="ebcee-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ebcee-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ebcee-122">Authorization</span></span>  | <span data-ttu-id="ebcee-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ebcee-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ebcee-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ebcee-125">Request body</span></span>
<span data-ttu-id="ebcee-126">No corpo da solicitação, fornece uma representação JSON do objeto [outlookTaskFolder](../resources/outlooktaskfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="ebcee-126">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ebcee-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="ebcee-127">Response</span></span>

<span data-ttu-id="ebcee-128">Se tiver êxito, este método retornará `201 Created` objeto response de código e [outlookTaskFolder](../resources/outlooktaskfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ebcee-128">If successful, this method returns `201 Created` response code and [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ebcee-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ebcee-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ebcee-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ebcee-130">Request</span></span>
<span data-ttu-id="ebcee-131">O exemplo a seguir cria uma pasta de tarefas chamada dos alunos no grupo de tarefa padrão (`My Tasks`) da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="ebcee-131">The following example creates a task folder called Volunteer in the default task group (`My Tasks`) of the user's mailbox.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_outlooktaskfolder_from_outlookuser"
}-->
```http
POST https://graph.microsoft.com/beta/me/outlook/taskfolders 
Content-type: application/json
Content-length: 60

{
  "name": "Volunteer"
}
```
<span data-ttu-id="ebcee-132">No corpo da solicitação, fornece uma representação JSON do objeto [outlookTaskFolder](../resources/outlooktaskfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="ebcee-132">In the request body, supply a JSON representation of [outlookTaskFolder](../resources/outlooktaskfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="ebcee-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="ebcee-133">Response</span></span>
<span data-ttu-id="ebcee-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ebcee-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "id": "AAMkADIyAAAhrbPWAAA=",
  "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAIbAGig==",
  "isDefaultFolder": false,
  "name": "Volunteer",
  "parentGroupKey": "0006f0b7-0000-0000-c000-000000000046"
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
