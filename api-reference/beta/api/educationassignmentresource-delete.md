---
title: Excluir educationAssignmentResource
description: .
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 239d971961d69f4c3d4e3442faea18ead00b507c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324693"
---
# <a name="delete-educationassignmentresource"></a><span data-ttu-id="5ca00-103">Excluir educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="5ca00-103">Delete educationAssignmentResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ca00-104">Excluir um recurso de uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="5ca00-104">Delete a resource from an assignment.</span></span> <span data-ttu-id="5ca00-105">Somente os professores da turma podem remover um recurso.</span><span class="sxs-lookup"><span data-stu-id="5ca00-105">Only teachers in the class can remove a resource.</span></span> <span data-ttu-id="5ca00-106">Após uma atribuição ter sido publicada para estudantes, os professores não poderão remover recursos marcados como "distributeToStudents".</span><span class="sxs-lookup"><span data-stu-id="5ca00-106">After an assignment has been published to students, teachers cannot remove resources that are marked as "distributeToStudents".</span></span>

## <a name="permissions"></a><span data-ttu-id="5ca00-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="5ca00-107">Permissions</span></span>
<span data-ttu-id="5ca00-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ca00-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ca00-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5ca00-110">Permission type</span></span>      | <span data-ttu-id="5ca00-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5ca00-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ca00-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5ca00-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="5ca00-113">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5ca00-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="5ca00-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5ca00-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="5ca00-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ca00-115">Not supported.</span></span>  |
|<span data-ttu-id="5ca00-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ca00-116">Application</span></span> | <span data-ttu-id="5ca00-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ca00-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="5ca00-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5ca00-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /educationClasses/assignments/{id}/resources/{id}

```
## <a name="request-headers"></a><span data-ttu-id="5ca00-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5ca00-119">Request headers</span></span>
| <span data-ttu-id="5ca00-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5ca00-120">Header</span></span>       | <span data-ttu-id="5ca00-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5ca00-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5ca00-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5ca00-122">Authorization</span></span>  | <span data-ttu-id="5ca00-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ca00-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5ca00-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5ca00-125">Request body</span></span>
<span data-ttu-id="5ca00-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5ca00-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="5ca00-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ca00-127">Response</span></span>
<span data-ttu-id="5ca00-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ca00-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ca00-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5ca00-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5ca00-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ca00-131">Request</span></span>
<span data-ttu-id="5ca00-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ca00-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationassignmentresource"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/resources/22002
```
##### <a name="response"></a><span data-ttu-id="5ca00-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ca00-133">Response</span></span>
<span data-ttu-id="5ca00-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5ca00-134">The following is an example of the response.</span></span> 


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
  "description": "Delete educationAssignmentResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
