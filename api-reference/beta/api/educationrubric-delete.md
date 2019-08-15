---
title: Excluir educationRubric
description: Excluir um objeto educationRubric.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: aae747b530e5109fbf56048b34be4b6a418f019c
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36416209"
---
# <a name="delete-educationrubric"></a><span data-ttu-id="11dec-103">Excluir educationRubric</span><span class="sxs-lookup"><span data-stu-id="11dec-103">Delete educationRubric</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11dec-104">Excluir um objeto [educationRubric](../resources/educationrubric.md) .</span><span class="sxs-lookup"><span data-stu-id="11dec-104">Delete an [educationRubric](../resources/educationrubric.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="11dec-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="11dec-105">Permissions</span></span>

<span data-ttu-id="11dec-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11dec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="11dec-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="11dec-108">Permission type</span></span>                        | <span data-ttu-id="11dec-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="11dec-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="11dec-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="11dec-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="11dec-111">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="11dec-111">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="11dec-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="11dec-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11dec-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11dec-113">Not supported.</span></span> |
| <span data-ttu-id="11dec-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="11dec-114">Application</span></span>                            | <span data-ttu-id="11dec-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11dec-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="11dec-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="11dec-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/me/rubrics/{id}
```

## <a name="request-headers"></a><span data-ttu-id="11dec-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="11dec-117">Request headers</span></span>

| <span data-ttu-id="11dec-118">Nome</span><span class="sxs-lookup"><span data-stu-id="11dec-118">Name</span></span>          | <span data-ttu-id="11dec-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="11dec-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="11dec-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="11dec-120">Authorization</span></span> | <span data-ttu-id="11dec-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="11dec-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="11dec-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="11dec-122">Request body</span></span>

<span data-ttu-id="11dec-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="11dec-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="11dec-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="11dec-124">Response</span></span>

<span data-ttu-id="11dec-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="11dec-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="11dec-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="11dec-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="11dec-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="11dec-128">Request</span></span>

<span data-ttu-id="11dec-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="11dec-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationrubric"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/me/rubrics/{id}
```

### <a name="response"></a><span data-ttu-id="11dec-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="11dec-130">Response</span></span>

<span data-ttu-id="11dec-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="11dec-131">The following is an example of the response.</span></span>

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
