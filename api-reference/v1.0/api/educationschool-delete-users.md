---
title: Remover educationUser de uma educationSchool
description: Exclua um usuário de uma escola.
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 4249ae683cab4dc2c9d42699f67dfbd5ca9c3ece
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27865545"
---
# <a name="remove-educationuser-from-an-educationschool"></a><span data-ttu-id="ec56c-103">Remover educationUser de uma educationSchool</span><span class="sxs-lookup"><span data-stu-id="ec56c-103">Remove educationUser from an educationSchool</span></span>

<span data-ttu-id="ec56c-104">Exclua um usuário de uma escola.</span><span class="sxs-lookup"><span data-stu-id="ec56c-104">Delete a user from a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="ec56c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ec56c-105">Permissions</span></span>
<span data-ttu-id="ec56c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec56c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec56c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ec56c-108">Permission type</span></span>      | <span data-ttu-id="ec56c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ec56c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec56c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ec56c-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="ec56c-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ec56c-111">Not supported.</span></span>  |
|<span data-ttu-id="ec56c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ec56c-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="ec56c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ec56c-113">Not supported.</span></span>  |
|<span data-ttu-id="ec56c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ec56c-114">Application</span></span> | <span data-ttu-id="ec56c-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec56c-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="ec56c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ec56c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}/users/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="ec56c-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ec56c-117">Request headers</span></span>
| <span data-ttu-id="ec56c-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ec56c-118">Header</span></span>       | <span data-ttu-id="ec56c-119">Valor</span><span class="sxs-lookup"><span data-stu-id="ec56c-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ec56c-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="ec56c-120">Authorization</span></span>  | <span data-ttu-id="ec56c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ec56c-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ec56c-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ec56c-123">Request body</span></span>
<span data-ttu-id="ec56c-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ec56c-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="ec56c-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec56c-125">Response</span></span>
<span data-ttu-id="ec56c-126">Se bem-sucedido, esse método retornará um código de resposta `204 No Content` e um corpo de resposta vazio.</span><span class="sxs-lookup"><span data-stu-id="ec56c-126">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec56c-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ec56c-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ec56c-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ec56c-128">Request</span></span>
<span data-ttu-id="ec56c-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ec56c-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/schools/{school-id}/users/{user-id}
```

##### <a name="response"></a><span data-ttu-id="ec56c-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec56c-130">Response</span></span>
<span data-ttu-id="ec56c-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ec56c-131">The following is an example of the response.</span></span> 
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
