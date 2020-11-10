---
title: Anexar educationRubric a educationAssignment
description: Anexar um objeto educationRubric existente a um educationAssignment.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 3d96ca954dbfb40c5c3db1f8404144337bcc0f34
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48966494"
---
# <a name="create-educationrubric"></a><span data-ttu-id="b933f-103">Criar educationRubric</span><span class="sxs-lookup"><span data-stu-id="b933f-103">Create educationRubric</span></span>

<span data-ttu-id="b933f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b933f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b933f-105">Anexar um objeto [educationRubric](../resources/educationrubric.md) existente a um [educationAssignment](../resources/educationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b933f-105">Attach an existing [educationRubric](../resources/educationrubric.md) object to an [educationAssignment](../resources/educationassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b933f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b933f-106">Permissions</span></span>

<span data-ttu-id="b933f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b933f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b933f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b933f-109">Permission type</span></span>                        | <span data-ttu-id="b933f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b933f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b933f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b933f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b933f-112">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b933f-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="b933f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b933f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b933f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b933f-114">Not supported.</span></span> |
| <span data-ttu-id="b933f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b933f-115">Application</span></span>                            | <span data-ttu-id="b933f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b933f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b933f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b933f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /education/classes/{id}/assignments/{id}/rubric/$ref
```

## <a name="request-headers"></a><span data-ttu-id="b933f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b933f-118">Request headers</span></span>

| <span data-ttu-id="b933f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b933f-119">Name</span></span>          | <span data-ttu-id="b933f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b933f-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b933f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b933f-121">Authorization</span></span> | <span data-ttu-id="b933f-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="b933f-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="b933f-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b933f-123">Request body</span></span>

<span data-ttu-id="b933f-124">No corpo da solicitação, forneça a ID de OData de um objeto [educationRubric](../resources/educationrubric.md) existente.</span><span class="sxs-lookup"><span data-stu-id="b933f-124">In the request body, supply the OData ID of an existing [educationRubric](../resources/educationrubric.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b933f-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="b933f-125">Response</span></span>

<span data-ttu-id="b933f-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b933f-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b933f-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b933f-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b933f-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b933f-129">Request</span></span>

<span data-ttu-id="b933f-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b933f-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b933f-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="b933f-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationrubric_from_educationassignment"
}-->

```http
PUT https://graph.microsoft.com/beta/education/classes/{id}/assignments/{id}/rubric/$ref
Content-type: application/json

{
  "@odata.id": "https://graph.microsoft.com/v1.0/education/me/rubrics/{id}"
}
```
# <a name="c"></a>[<span data-ttu-id="b933f-132">C#</span><span class="sxs-lookup"><span data-stu-id="b933f-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationrubric-from-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b933f-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b933f-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationrubric-from-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b933f-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b933f-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationrubric-from-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b933f-135">Java</span><span class="sxs-lookup"><span data-stu-id="b933f-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationrubric-from-educationassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b933f-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="b933f-136">Response</span></span>

<span data-ttu-id="b933f-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b933f-137">The following is an example of the response.</span></span>

> <span data-ttu-id="b933f-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b933f-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationRubric"
} -->

```http
HTTP/1.1 204 No Content
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationRubric",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


