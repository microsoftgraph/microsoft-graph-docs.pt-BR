---
title: Remover educationUser de uma educationSchool
description: Exclua um usuário de uma escola.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 930ae9ca24b379abd728bd01ebd6ce8f72291757
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987640"
---
# <a name="remove-educationuser-from-an-educationschool"></a><span data-ttu-id="5eb48-103">Remover educationUser de uma educationSchool</span><span class="sxs-lookup"><span data-stu-id="5eb48-103">Remove educationUser from an educationSchool</span></span>

<span data-ttu-id="5eb48-104">Exclua um usuário de uma escola.</span><span class="sxs-lookup"><span data-stu-id="5eb48-104">Delete a user from a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="5eb48-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5eb48-105">Permissions</span></span>
<span data-ttu-id="5eb48-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5eb48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5eb48-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5eb48-108">Permission type</span></span>      | <span data-ttu-id="5eb48-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5eb48-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5eb48-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5eb48-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="5eb48-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5eb48-111">Not supported.</span></span>  |
|<span data-ttu-id="5eb48-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5eb48-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="5eb48-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5eb48-113">Not supported.</span></span>  |
|<span data-ttu-id="5eb48-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5eb48-114">Application</span></span> | <span data-ttu-id="5eb48-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5eb48-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="5eb48-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5eb48-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}/users/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="5eb48-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5eb48-117">Request headers</span></span>
| <span data-ttu-id="5eb48-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5eb48-118">Header</span></span>       | <span data-ttu-id="5eb48-119">Valor</span><span class="sxs-lookup"><span data-stu-id="5eb48-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5eb48-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="5eb48-120">Authorization</span></span>  | <span data-ttu-id="5eb48-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5eb48-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5eb48-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5eb48-123">Request body</span></span>
<span data-ttu-id="5eb48-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5eb48-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="5eb48-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="5eb48-125">Response</span></span>
<span data-ttu-id="5eb48-126">Se bem-sucedido, esse método retornará um código de resposta `204 No Content` e um corpo de resposta vazio.</span><span class="sxs-lookup"><span data-stu-id="5eb48-126">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="5eb48-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5eb48-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5eb48-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5eb48-128">Request</span></span>
<span data-ttu-id="5eb48-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5eb48-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/schools/{school-id}/users/{user-id}
```

##### <a name="response"></a><span data-ttu-id="5eb48-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="5eb48-130">Response</span></span>
<span data-ttu-id="5eb48-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5eb48-131">The following is an example of the response.</span></span> 
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
