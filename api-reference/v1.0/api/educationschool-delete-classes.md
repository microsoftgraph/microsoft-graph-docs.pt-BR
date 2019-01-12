---
title: Remover educationClass
description: Exclua uma classe de uma escola.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 3cf61d77171e7dc3161aa3b3cc48d663de784649
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950946"
---
# <a name="remove-educationclass"></a><span data-ttu-id="f3e69-103">Remover educationClass</span><span class="sxs-lookup"><span data-stu-id="f3e69-103">Remove educationClass</span></span>

<span data-ttu-id="f3e69-104">Exclua uma classe de uma escola.</span><span class="sxs-lookup"><span data-stu-id="f3e69-104">Delete a class from a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="f3e69-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f3e69-105">Permissions</span></span>
<span data-ttu-id="f3e69-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3e69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3e69-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f3e69-108">Permission type</span></span>      | <span data-ttu-id="f3e69-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f3e69-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f3e69-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f3e69-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="f3e69-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f3e69-111">Not supported.</span></span>  |
|<span data-ttu-id="f3e69-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f3e69-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f3e69-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f3e69-113">Not supported.</span></span>  |
|<span data-ttu-id="f3e69-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f3e69-114">Application</span></span> | <span data-ttu-id="f3e69-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3e69-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f3e69-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f3e69-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}/classes/{classId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="f3e69-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f3e69-117">Request headers</span></span>
| <span data-ttu-id="f3e69-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f3e69-118">Header</span></span>       | <span data-ttu-id="f3e69-119">Valor</span><span class="sxs-lookup"><span data-stu-id="f3e69-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f3e69-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="f3e69-120">Authorization</span></span>  | <span data-ttu-id="f3e69-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f3e69-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f3e69-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f3e69-123">Request body</span></span>
<span data-ttu-id="f3e69-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f3e69-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="f3e69-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3e69-125">Response</span></span>
<span data-ttu-id="f3e69-126">Se bem-sucedido, esse método retornará um código de resposta `204 No Content` e um corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f3e69-126">If successful, this method returns a `204 No Content` response code and a response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3e69-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f3e69-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f3e69-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f3e69-128">Request</span></span>
<span data-ttu-id="f3e69-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f3e69-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/schools/{school-id}/classes/{class-id}
```

##### <a name="response"></a><span data-ttu-id="f3e69-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3e69-130">Response</span></span>
<span data-ttu-id="f3e69-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f3e69-131">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
