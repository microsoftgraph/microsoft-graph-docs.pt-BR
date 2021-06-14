---
title: Excluir educationRubric
description: Exclua um objeto educationRubric.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 0b488c7c3307a7ac2388d36861eb4895fec44484
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912217"
---
# <a name="delete-educationrubric"></a><span data-ttu-id="d0f8c-103">Excluir educationRubric</span><span class="sxs-lookup"><span data-stu-id="d0f8c-103">Delete educationRubric</span></span>

<span data-ttu-id="d0f8c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0f8c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d0f8c-105">[Exclua um objeto educationRubric.](../resources/educationrubric.md)</span><span class="sxs-lookup"><span data-stu-id="d0f8c-105">Delete an [educationRubric](../resources/educationrubric.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d0f8c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d0f8c-106">Permissions</span></span>

<span data-ttu-id="d0f8c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0f8c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d0f8c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d0f8c-109">Permission type</span></span>                        | <span data-ttu-id="d0f8c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d0f8c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d0f8c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d0f8c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d0f8c-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d0f8c-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="d0f8c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d0f8c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0f8c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d0f8c-114">Not supported.</span></span> |
| <span data-ttu-id="d0f8c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d0f8c-115">Application</span></span>                            | <span data-ttu-id="d0f8c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d0f8c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d0f8c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d0f8c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/me/rubrics/ceb3863e-6912-4ea9-ac41-3c2bb7b6672d
```

## <a name="request-headers"></a><span data-ttu-id="d0f8c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d0f8c-118">Request headers</span></span>

| <span data-ttu-id="d0f8c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d0f8c-119">Name</span></span>          | <span data-ttu-id="d0f8c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0f8c-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="d0f8c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d0f8c-121">Authorization</span></span> | <span data-ttu-id="d0f8c-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="d0f8c-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="d0f8c-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d0f8c-123">Request body</span></span>

<span data-ttu-id="d0f8c-124">Não fornece um corpo de solicitação para este método.</span><span class="sxs-lookup"><span data-stu-id="d0f8c-124">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d0f8c-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0f8c-125">Response</span></span>

<span data-ttu-id="d0f8c-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d0f8c-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d0f8c-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d0f8c-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d0f8c-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d0f8c-129">Request</span></span>

<span data-ttu-id="d0f8c-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d0f8c-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_educationrubric"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/education/me/rubrics/ceb3863e-6912-4ea9-ac41-3c2bb7b6672d
```

### <a name="response"></a><span data-ttu-id="d0f8c-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0f8c-131">Response</span></span>

<span data-ttu-id="d0f8c-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d0f8c-132">The following is an example of the response.</span></span>

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


