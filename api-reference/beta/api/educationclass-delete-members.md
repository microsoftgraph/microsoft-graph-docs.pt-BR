---
title: Remover um aluno
description: Remove um educationUser de uma educationClass
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: ee7661c2571a3aca43abd9410e47e8e8da43e325
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2019
ms.locfileid: "37427792"
---
# <a name="remove-a-student"></a><span data-ttu-id="fa1b3-103">Remover um aluno</span><span class="sxs-lookup"><span data-stu-id="fa1b3-103">Remove a student</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa1b3-104">Remove um [educationUser](../resources/educationuser.md) de uma [educationClass](../resources/educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="fa1b3-104">Removes an [educationUser](../resources/educationuser.md) from an [educationClass](../resources/educationclass.md)</span></span>

><span data-ttu-id="fa1b3-105">**Observação:** professores _e_ alunos estão na coleção **members** da aula.</span><span class="sxs-lookup"><span data-stu-id="fa1b3-105">**Note:** Teachers _and_ students are in the class **members** collection.</span></span> <span data-ttu-id="fa1b3-106">Antes de chamar essa API, garanta que **educationUser** que você está removendo não seja um professor.</span><span class="sxs-lookup"><span data-stu-id="fa1b3-106">Before calling this API, insure that the **educationUser** you are removing is not a teacher.</span></span>  <span data-ttu-id="fa1b3-107">Obtenha a lista de professores chamando [educationclass_list_teachers](educationclass-list-teachers.md) e verificando se a ID do usuário a ser removido não está na lista de professores retornada.</span><span class="sxs-lookup"><span data-stu-id="fa1b3-107">Get the list of teachers by calling [educationclass_list_teachers](educationclass-list-teachers.md) and verifying the user Id of the user to be removed is not in the returned teacher list.</span></span>

## <a name="permissions"></a><span data-ttu-id="fa1b3-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="fa1b3-108">Permissions</span></span>
<span data-ttu-id="fa1b3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa1b3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa1b3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fa1b3-111">Permission type</span></span>      | <span data-ttu-id="fa1b3-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fa1b3-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fa1b3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fa1b3-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="fa1b3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fa1b3-114">Not supported.</span></span>  |
|<span data-ttu-id="fa1b3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fa1b3-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="fa1b3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fa1b3-116">Not supported.</span></span>  |
|<span data-ttu-id="fa1b3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fa1b3-117">Application</span></span> | <span data-ttu-id="fa1b3-118">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa1b3-118">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="fa1b3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fa1b3-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/members/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="fa1b3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fa1b3-120">Request headers</span></span>
| <span data-ttu-id="fa1b3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fa1b3-121">Header</span></span>       | <span data-ttu-id="fa1b3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="fa1b3-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fa1b3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fa1b3-123">Authorization</span></span>  | <span data-ttu-id="fa1b3-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fa1b3-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fa1b3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fa1b3-126">Request body</span></span>
<span data-ttu-id="fa1b3-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fa1b3-127">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="fa1b3-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa1b3-128">Response</span></span>
<span data-ttu-id="fa1b3-129">Se bem-sucedido, esse método retornará um código de resposta `204 No Content` e um corpo de resposta vazio.</span><span class="sxs-lookup"><span data-stu-id="fa1b3-129">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa1b3-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fa1b3-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fa1b3-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fa1b3-131">Request</span></span>
<span data-ttu-id="fa1b3-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fa1b3-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fa1b3-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="fa1b3-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11003/members/14008
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fa1b3-134">C#</span><span class="sxs-lookup"><span data-stu-id="fa1b3-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationclass-from-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fa1b3-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fa1b3-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationclass-from-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fa1b3-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fa1b3-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationclass-from-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="fa1b3-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa1b3-137">Response</span></span>
<span data-ttu-id="fa1b3-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fa1b3-138">The following is an example of the response.</span></span> 
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
<!--
{
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
