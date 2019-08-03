---
title: Remover o educationRubric do educationAssignment
description: Remover um educationRubric de um educationAssignment
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: a6334e24c01db8f32f643f552b1a64cb2c86967d
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173220"
---
# <a name="remove-educationrubric-from-educationassignment"></a><span data-ttu-id="2ccad-103">Remover o educationRubric do educationAssignment</span><span class="sxs-lookup"><span data-stu-id="2ccad-103">Remove educationRubric from educationAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ccad-104">Remover um [educationRubric](../resources/educationrubric.md) de um [educationAssignment](../resources/educationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2ccad-104">Remove an [educationRubric](../resources/educationrubric.md) from an [educationAssignment](../resources/educationassignment.md).</span></span>  <span data-ttu-id="2ccad-105">Isso não exclui o próprio amostra rubric.</span><span class="sxs-lookup"><span data-stu-id="2ccad-105">This does not delete the rubric itself.</span></span>

## <a name="permissions"></a><span data-ttu-id="2ccad-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2ccad-106">Permissions</span></span>

<span data-ttu-id="2ccad-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ccad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2ccad-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2ccad-109">Permission type</span></span>                        | <span data-ttu-id="2ccad-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2ccad-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2ccad-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2ccad-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2ccad-112">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2ccad-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="2ccad-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2ccad-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ccad-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ccad-114">Not supported.</span></span> |
| <span data-ttu-id="2ccad-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2ccad-115">Application</span></span>                            | <span data-ttu-id="2ccad-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ccad-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2ccad-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2ccad-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/{id}/assignments/{id}/rubric/$ref
```

## <a name="request-headers"></a><span data-ttu-id="2ccad-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2ccad-118">Request headers</span></span>

| <span data-ttu-id="2ccad-119">Nome</span><span class="sxs-lookup"><span data-stu-id="2ccad-119">Name</span></span>          | <span data-ttu-id="2ccad-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ccad-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="2ccad-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="2ccad-121">Authorization</span></span> | <span data-ttu-id="2ccad-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="2ccad-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="2ccad-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2ccad-123">Request body</span></span>

<span data-ttu-id="2ccad-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2ccad-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ccad-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ccad-125">Response</span></span>

<span data-ttu-id="2ccad-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2ccad-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2ccad-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2ccad-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2ccad-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2ccad-129">Request</span></span>

<span data-ttu-id="2ccad-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2ccad-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationrubric_from_educationassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/me/assignments/{id}/rubric/$ref
```

### <a name="response"></a><span data-ttu-id="2ccad-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ccad-131">Response</span></span>

<span data-ttu-id="2ccad-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2ccad-132">The following is an example of the response.</span></span>

> <span data-ttu-id="2ccad-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2ccad-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete educationRubric",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
