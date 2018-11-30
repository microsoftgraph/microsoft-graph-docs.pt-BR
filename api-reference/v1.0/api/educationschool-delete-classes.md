---
title: Remover educationClass
description: Exclua uma classe de uma escola.
ms.openlocfilehash: 5103265bbb0c0f74def65c9adba9cc28dc41785b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006548"
---
# <a name="remove-educationclass"></a><span data-ttu-id="568fa-103">Remover educationClass</span><span class="sxs-lookup"><span data-stu-id="568fa-103">Remove educationClass</span></span>

<span data-ttu-id="568fa-104">Exclua uma classe de uma escola.</span><span class="sxs-lookup"><span data-stu-id="568fa-104">Delete a class from a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="568fa-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="568fa-105">Permissions</span></span>
<span data-ttu-id="568fa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="568fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="568fa-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="568fa-108">Permission type</span></span>      | <span data-ttu-id="568fa-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="568fa-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="568fa-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="568fa-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="568fa-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="568fa-111">Not supported.</span></span>  |
|<span data-ttu-id="568fa-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="568fa-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="568fa-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="568fa-113">Not supported.</span></span>  |
|<span data-ttu-id="568fa-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="568fa-114">Application</span></span> | <span data-ttu-id="568fa-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="568fa-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="568fa-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="568fa-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}/classes/{classId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="568fa-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="568fa-117">Request headers</span></span>
| <span data-ttu-id="568fa-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="568fa-118">Header</span></span>       | <span data-ttu-id="568fa-119">Valor</span><span class="sxs-lookup"><span data-stu-id="568fa-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="568fa-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="568fa-120">Authorization</span></span>  | <span data-ttu-id="568fa-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="568fa-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="568fa-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="568fa-123">Request body</span></span>
<span data-ttu-id="568fa-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="568fa-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="568fa-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="568fa-125">Response</span></span>
<span data-ttu-id="568fa-126">Se bem-sucedido, esse método retornará um código de resposta `204 No Content` e um corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="568fa-126">If successful, this method returns a `204 No Content` response code and a response body.</span></span>

## <a name="example"></a><span data-ttu-id="568fa-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="568fa-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="568fa-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="568fa-128">Request</span></span>
<span data-ttu-id="568fa-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="568fa-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/schools/{school-id}/classes/{class-id}
```

##### <a name="response"></a><span data-ttu-id="568fa-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="568fa-130">Response</span></span>
<span data-ttu-id="568fa-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="568fa-131">The following is an example of the response.</span></span> 

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