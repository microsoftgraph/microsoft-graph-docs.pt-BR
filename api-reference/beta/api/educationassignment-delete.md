---
title: Excluir educationAssignment
description: Excluir uma atribuição existente. Somente os professores de uma aula podem excluir atribuições.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 0cae6bc0d5d6e799d780e9120f2935759ff5843e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33325176"
---
# <a name="delete-educationassignment"></a><span data-ttu-id="d8a0a-104">Excluir educationAssignment</span><span class="sxs-lookup"><span data-stu-id="d8a0a-104">Delete educationAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8a0a-105">Excluir uma atribuição existente.</span><span class="sxs-lookup"><span data-stu-id="d8a0a-105">Delete an existing assignment.</span></span> <span data-ttu-id="d8a0a-106">Somente os professores de uma aula podem excluir atribuições.</span><span class="sxs-lookup"><span data-stu-id="d8a0a-106">Only teachers within a class can delete assignments.</span></span>

## <a name="permissions"></a><span data-ttu-id="d8a0a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d8a0a-107">Permissions</span></span>
<span data-ttu-id="d8a0a-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8a0a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8a0a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d8a0a-110">Permission type</span></span>      | <span data-ttu-id="d8a0a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d8a0a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d8a0a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d8a0a-112">Delegated (work or school account)</span></span>| <span data-ttu-id="d8a0a-113">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8a0a-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="d8a0a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d8a0a-114">Delegated (personal Microsoft account)</span></span> |   <span data-ttu-id="d8a0a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8a0a-115">Not Supported.</span></span> |
|<span data-ttu-id="d8a0a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d8a0a-116">Application</span></span> | <span data-ttu-id="d8a0a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8a0a-117">Not Supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="d8a0a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d8a0a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/<id>/assignments/<id>
```
## <a name="request-headers"></a><span data-ttu-id="d8a0a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d8a0a-119">Request headers</span></span>
| <span data-ttu-id="d8a0a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d8a0a-120">Header</span></span>       | <span data-ttu-id="d8a0a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d8a0a-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d8a0a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d8a0a-122">Authorization</span></span>  | <span data-ttu-id="d8a0a-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d8a0a-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d8a0a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d8a0a-125">Request body</span></span>
<span data-ttu-id="d8a0a-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d8a0a-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="d8a0a-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8a0a-127">Response</span></span>
<span data-ttu-id="d8a0a-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d8a0a-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8a0a-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d8a0a-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="d8a0a-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d8a0a-131">Request</span></span>
<span data-ttu-id="d8a0a-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d8a0a-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_educationassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/classes/11014/assignments/19002
```
### <a name="response"></a><span data-ttu-id="d8a0a-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8a0a-133">Response</span></span>
<span data-ttu-id="d8a0a-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d8a0a-134">The following is an example of the response.</span></span> 


<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
