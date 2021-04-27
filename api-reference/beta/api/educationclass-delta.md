---
title: 'educationClass: delta'
description: Get newly created or updated classes, including membership changes, without having to perform a full read of the entire class collection.
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: e8b93c8ddd251bbc25efc9203417d6736e6bf62c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52044071"
---
# <a name="educationclass-delta"></a><span data-ttu-id="30067-103">educationClass: delta</span><span class="sxs-lookup"><span data-stu-id="30067-103">educationClass: delta</span></span>

<span data-ttu-id="30067-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30067-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30067-105">Get newly created or updated classes, including membership changes, without having to perform a full read of the entire class collection.</span><span class="sxs-lookup"><span data-stu-id="30067-105">Get newly created or updated classes, including membership changes, without having to perform a full read of the entire class collection.</span></span> <span data-ttu-id="30067-106">Consulte [Usar consulta delta para](/graph/delta-query-overview) obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="30067-106">See [Use delta query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="30067-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="30067-107">Permissions</span></span>

<span data-ttu-id="30067-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30067-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="30067-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="30067-110">Permission type</span></span>                        | <span data-ttu-id="30067-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="30067-111">Permissions (from least to most privileged)</span></span>                              |
| :------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="30067-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="30067-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="30067-113">EduRoster.ReadBasic, EduRoster.Read ou EduRoster.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="30067-113">EduRoster.ReadBasic, EduRoster.Read, or EduRoster.ReadWrite</span></span>              |
| <span data-ttu-id="30067-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="30067-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30067-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="30067-115">Not supported.</span></span>                                                           |
| <span data-ttu-id="30067-116">Application</span><span class="sxs-lookup"><span data-stu-id="30067-116">Application</span></span>                            | <span data-ttu-id="30067-117">EduRoster.ReadBasic.All, EduRoster.Read.All ou EduRoster.WriteWrite.All</span><span class="sxs-lookup"><span data-stu-id="30067-117">EduRoster.ReadBasic.All, EduRoster.Read.All, or EduRoster.WriteWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="30067-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="30067-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/classes/delta
```

## <a name="request-headers"></a><span data-ttu-id="30067-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="30067-119">Request headers</span></span>

| <span data-ttu-id="30067-120">Nome</span><span class="sxs-lookup"><span data-stu-id="30067-120">Name</span></span>          | <span data-ttu-id="30067-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="30067-121">Description</span></span>   |
| :------------ | :------------ |
| <span data-ttu-id="30067-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="30067-122">Authorization</span></span> | <span data-ttu-id="30067-123">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="30067-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="30067-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="30067-124">Request body</span></span>

<span data-ttu-id="30067-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="30067-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="30067-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="30067-126">Response</span></span>

<span data-ttu-id="30067-127">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto da coleção educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="30067-127">If successful, this method returns a `200 OK` response code and an [educationClass](../resources/educationclass.md) collection object in the response body.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="30067-128">os deltas educationClass não incluem classes excluídas.</span><span class="sxs-lookup"><span data-stu-id="30067-128">educationClass deltas do not include deleted classes.</span></span>

## <a name="example"></a><span data-ttu-id="30067-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="30067-129">Example</span></span>

<span data-ttu-id="30067-130">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="30067-130">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="30067-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="30067-131">Request</span></span>

<span data-ttu-id="30067-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="30067-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="30067-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="30067-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationclass_delta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/delta
```
# <a name="c"></a>[<span data-ttu-id="30067-134">C#</span><span class="sxs-lookup"><span data-stu-id="30067-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationclass-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="30067-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="30067-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationclass-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="30067-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="30067-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationclass-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="30067-137">Java</span><span class="sxs-lookup"><span data-stu-id="30067-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationclass-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="30067-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="30067-138">Response</span></span>

<span data-ttu-id="30067-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="30067-139">The following is an example of the response.</span></span>

> <span data-ttu-id="30067-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="30067-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 585

{
  "value": [
    {
      "classCode": "String",
      "course": { "@odata.type": "microsoft.graph.educationCourse" },
      "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
      "description": "String",
      "displayName": "String",
      "externalId": "String",
      "externalName": "String",
      "externalSource": "string",
      "grade": "string",
      "id": "String (identifier)",
      "mailNickname": "String",
      "term": { "@odata.type": "microsoft.graph.educationTerm" }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationClass: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


