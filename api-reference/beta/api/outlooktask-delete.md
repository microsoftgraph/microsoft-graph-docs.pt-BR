---
title: Excluir outlookTask
description: Exclua a tarefa especificada do Outlook na caixa de correio do usuário.
ms.openlocfilehash: 00c2c4d1e5b706b34b531380e32083be55c98776
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040644"
---
# <a name="delete-outlooktask"></a><span data-ttu-id="bc773-103">Excluir outlookTask</span><span class="sxs-lookup"><span data-stu-id="bc773-103">Delete outlookTask</span></span>

> <span data-ttu-id="bc773-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bc773-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bc773-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bc773-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bc773-106">Exclua a tarefa especificada do Outlook na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="bc773-106">Delete the specified Outlook task in the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="bc773-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="bc773-107">Permissions</span></span>
<span data-ttu-id="bc773-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc773-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc773-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bc773-110">Permission type</span></span>      | <span data-ttu-id="bc773-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bc773-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc773-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bc773-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bc773-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc773-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="bc773-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bc773-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc773-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc773-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="bc773-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bc773-116">Application</span></span> | <span data-ttu-id="bc773-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc773-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc773-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bc773-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id|userPrincipalName}/outlook/tasks/{id}
DELETE /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks/{id}
DELETE /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}

```
## <a name="request-headers"></a><span data-ttu-id="bc773-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bc773-119">Request headers</span></span>
| <span data-ttu-id="bc773-120">Nome</span><span class="sxs-lookup"><span data-stu-id="bc773-120">Name</span></span>       | <span data-ttu-id="bc773-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc773-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="bc773-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="bc773-122">Authorization</span></span>  | <span data-ttu-id="bc773-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bc773-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bc773-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bc773-125">Request body</span></span>
<span data-ttu-id="bc773-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bc773-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bc773-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc773-127">Response</span></span>

<span data-ttu-id="bc773-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bc773-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc773-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bc773-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bc773-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bc773-131">Request</span></span>
<span data-ttu-id="bc773-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bc773-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_outlooktask"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/outlook/tasks('AAMkADIyAAAhrb_QAAA=')
```
##### <a name="response"></a><span data-ttu-id="bc773-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc773-133">Response</span></span>
<span data-ttu-id="bc773-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bc773-134">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete outlookTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->