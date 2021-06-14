---
title: Excluir educationRubric de educationAssignment
description: Excluir um educationRubric de um educationAssignment
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 9ce6eb7090c75fab942fc9cd5e317b5526a6dd7b
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912220"
---
# <a name="delete-educationrubric-from-educationassignment"></a><span data-ttu-id="c8070-103">Excluir educationRubric de educationAssignment</span><span class="sxs-lookup"><span data-stu-id="c8070-103">Delete educationRubric from educationAssignment</span></span>

<span data-ttu-id="c8070-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8070-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c8070-105">Remover um [educationRubric](../resources/educationrubric.md) de [um educationAssignment](../resources/educationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c8070-105">Remove an [educationRubric](../resources/educationrubric.md) from an [educationAssignment](../resources/educationassignment.md).</span></span>
<span data-ttu-id="c8070-106">Este método não exclui a rubrica em si.</span><span class="sxs-lookup"><span data-stu-id="c8070-106">This method does not delete the rubric itself.</span></span>

## <a name="permissions"></a><span data-ttu-id="c8070-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="c8070-107">Permissions</span></span>

<span data-ttu-id="c8070-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8070-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c8070-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c8070-110">Permission type</span></span>                        | <span data-ttu-id="c8070-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c8070-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c8070-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c8070-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="c8070-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c8070-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="c8070-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c8070-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8070-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c8070-115">Not supported.</span></span> |
| <span data-ttu-id="c8070-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c8070-116">Application</span></span>                            | <span data-ttu-id="c8070-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c8070-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c8070-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c8070-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/rubric/$ref
```

## <a name="request-headers"></a><span data-ttu-id="c8070-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c8070-119">Request headers</span></span>

| <span data-ttu-id="c8070-120">Nome</span><span class="sxs-lookup"><span data-stu-id="c8070-120">Name</span></span>          | <span data-ttu-id="c8070-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8070-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="c8070-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c8070-122">Authorization</span></span> | <span data-ttu-id="c8070-123">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="c8070-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="c8070-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c8070-124">Request body</span></span>

<span data-ttu-id="c8070-125">Não fornece um corpo de solicitação para este método.</span><span class="sxs-lookup"><span data-stu-id="c8070-125">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8070-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8070-126">Response</span></span>

<span data-ttu-id="c8070-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c8070-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c8070-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c8070-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c8070-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c8070-130">Request</span></span>

<span data-ttu-id="c8070-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c8070-131">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_educationrubric_from_educationassignment"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/rubric/$ref
```

### <a name="response"></a><span data-ttu-id="c8070-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8070-132">Response</span></span>

<span data-ttu-id="c8070-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c8070-133">The following is an example of the response.</span></span>

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


