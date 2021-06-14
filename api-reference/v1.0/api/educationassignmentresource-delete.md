---
title: Excluir educationAssignmentResource
description: Exclua um recurso específico anexado a uma atribuição.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: f6e86992537e366d5f0972f323729796f197e2b5
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912218"
---
# <a name="delete-educationassignmentresource"></a><span data-ttu-id="18b01-103">Excluir educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="18b01-103">Delete educationAssignmentResource</span></span>

<span data-ttu-id="18b01-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18b01-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="18b01-105">Exclua um recurso específico anexado a uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="18b01-105">Delete a specific resource attached to an assignment.</span></span>

<span data-ttu-id="18b01-106">Em geral, somente os professores da classe podem remover um recurso.</span><span class="sxs-lookup"><span data-stu-id="18b01-106">In general, only teachers in the class can remove a resource.</span></span> <span data-ttu-id="18b01-107">No entanto, os professores não podem remover recursos marcados como "distributeToStudents", depois que a atribuição tiver sido publicada para os alunos.</span><span class="sxs-lookup"><span data-stu-id="18b01-107">However, teachers cannot remove resources marked as "distributeToStudents", after the assignment has been published to students.</span></span>

## <a name="permissions"></a><span data-ttu-id="18b01-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="18b01-108">Permissions</span></span>
<span data-ttu-id="18b01-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18b01-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18b01-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="18b01-111">Permission type</span></span>      | <span data-ttu-id="18b01-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="18b01-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18b01-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="18b01-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="18b01-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18b01-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="18b01-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="18b01-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="18b01-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="18b01-116">Not supported.</span></span>  |
|<span data-ttu-id="18b01-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="18b01-117">Application</span></span> | <span data-ttu-id="18b01-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="18b01-118">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="18b01-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="18b01-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/resources/8b01c1d0-aafc-4f8c-bd73-89faa3df1c1c

```
## <a name="request-headers"></a><span data-ttu-id="18b01-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="18b01-120">Request headers</span></span>
| <span data-ttu-id="18b01-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="18b01-121">Header</span></span>       | <span data-ttu-id="18b01-122">Valor</span><span class="sxs-lookup"><span data-stu-id="18b01-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="18b01-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="18b01-123">Authorization</span></span>  | <span data-ttu-id="18b01-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="18b01-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="18b01-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="18b01-126">Request body</span></span>
<span data-ttu-id="18b01-127">Não fornece um corpo de solicitação para este método.</span><span class="sxs-lookup"><span data-stu-id="18b01-127">Don't supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="18b01-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="18b01-128">Response</span></span>
<span data-ttu-id="18b01-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="18b01-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18b01-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="18b01-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="18b01-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="18b01-132">Request</span></span>
<span data-ttu-id="18b01-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="18b01-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_educationassignmentresource"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/resources/22002
```

### <a name="response"></a><span data-ttu-id="18b01-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="18b01-134">Response</span></span>
<span data-ttu-id="18b01-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="18b01-135">The following is an example of the response.</span></span> 


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
  "suppressions": [
  ]
}
-->


