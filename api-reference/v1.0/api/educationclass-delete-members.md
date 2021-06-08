---
title: Remover membro do educationClass
description: Remove um educationUser de uma educationClass
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: d98245691a08ede09d16a290b1aef67935c4753c
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52783651"
---
# <a name="remove-member-from-educationclass"></a><span data-ttu-id="b900e-103">Remover membro do educationClass</span><span class="sxs-lookup"><span data-stu-id="b900e-103">Remove member from educationClass</span></span>

<span data-ttu-id="b900e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b900e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b900e-105">Remove um [educationUser](../resources/educationuser.md) de uma [educationClass](../resources/educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="b900e-105">Removes an [educationUser](../resources/educationuser.md) from an [educationClass](../resources/educationclass.md)</span></span>

> <span data-ttu-id="b900e-106">**Observação:** professores _e_ alunos estão na coleção **members** da aula.</span><span class="sxs-lookup"><span data-stu-id="b900e-106">**Note:** Teachers _and_ students are in the class **members** collection.</span></span> <span data-ttu-id="b900e-107">Antes de chamar essa API, garanta que **educationUser** que você está removendo não seja um professor.</span><span class="sxs-lookup"><span data-stu-id="b900e-107">Before calling this API, insure that the **educationUser** you are removing is not a teacher.</span></span> <span data-ttu-id="b900e-108">Obtenha a lista de professores chamando [educationclass_list_teachers](educationclass-list-teachers.md) e verificando se a ID do usuário a ser removido não está na lista de professores retornada.</span><span class="sxs-lookup"><span data-stu-id="b900e-108">Get the list of teachers by calling [educationclass_list_teachers](educationclass-list-teachers.md) and verifying the user Id of the user to be removed is not in the returned teacher list.</span></span>

## <a name="permissions"></a><span data-ttu-id="b900e-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="b900e-109">Permissions</span></span>
<span data-ttu-id="b900e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b900e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b900e-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b900e-112">Permission type</span></span>      | <span data-ttu-id="b900e-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b900e-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b900e-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b900e-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="b900e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b900e-115">Not supported.</span></span>  |
|<span data-ttu-id="b900e-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b900e-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="b900e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b900e-117">Not supported.</span></span>  |
|<span data-ttu-id="b900e-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b900e-118">Application</span></span> | <span data-ttu-id="b900e-119">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b900e-119">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b900e-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b900e-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/members/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="b900e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b900e-121">Request headers</span></span>
| <span data-ttu-id="b900e-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b900e-122">Header</span></span>       | <span data-ttu-id="b900e-123">Valor</span><span class="sxs-lookup"><span data-stu-id="b900e-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b900e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="b900e-124">Authorization</span></span>  | <span data-ttu-id="b900e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b900e-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b900e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b900e-127">Request body</span></span>
<span data-ttu-id="b900e-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b900e-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="b900e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b900e-129">Response</span></span>
<span data-ttu-id="b900e-130">Se bem-sucedido, esse método retornará um código de resposta `204 No Content` e um corpo de resposta vazio.</span><span class="sxs-lookup"><span data-stu-id="b900e-130">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="b900e-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b900e-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b900e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b900e-132">Request</span></span>
<span data-ttu-id="b900e-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b900e-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b900e-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="b900e-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool_1"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/classes/{class-id}/members/{member-id}
```
# <a name="c"></a>[<span data-ttu-id="b900e-135">C#</span><span class="sxs-lookup"><span data-stu-id="b900e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationclass-from-educationschool-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b900e-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b900e-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationclass-from-educationschool-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b900e-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b900e-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationclass-from-educationschool-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b900e-138">Java</span><span class="sxs-lookup"><span data-stu-id="b900e-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationclass-from-educationschool-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b900e-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="b900e-139">Response</span></span>
<span data-ttu-id="b900e-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b900e-140">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
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
