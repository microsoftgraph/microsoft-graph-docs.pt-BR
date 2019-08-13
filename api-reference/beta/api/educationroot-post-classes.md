---
title: Criar educationClass
description: Crie uma nova aula. Isso também criará um grupo universal. Quando você usar essa API para criar uma classe, ela adicionará propriedades especiais ao grupo, que será
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: eb72a1e557240a988c71ae47d0c855ea0c3025a5
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36323959"
---
# <a name="create-educationclass"></a><span data-ttu-id="afb29-105">Criar educationClass</span><span class="sxs-lookup"><span data-stu-id="afb29-105">Create educationClass</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="afb29-106">Crie uma nova aula.</span><span class="sxs-lookup"><span data-stu-id="afb29-106">Create a new class.</span></span> <span data-ttu-id="afb29-107">Isso também criará um grupo universal.</span><span class="sxs-lookup"><span data-stu-id="afb29-107">This will also create a universal group.</span></span> <span data-ttu-id="afb29-108">Quando você usar essa API para criar uma aula, ela adicionará propriedades especiais ao grupo, que adicionará recursos como atribuições e tratamento especial no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="afb29-108">When you use this API to create a class, it will add special properties to the group, which will add features such as assignments and special handling within Microsoft Teams.</span></span>

## <a name="permissions"></a><span data-ttu-id="afb29-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="afb29-109">Permissions</span></span>
<span data-ttu-id="afb29-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="afb29-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="afb29-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="afb29-112">Permission type</span></span>      | <span data-ttu-id="afb29-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="afb29-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="afb29-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="afb29-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="afb29-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="afb29-115">Not supported.</span></span>  |
|<span data-ttu-id="afb29-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="afb29-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="afb29-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="afb29-117">Not supported.</span></span>  |
|<span data-ttu-id="afb29-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="afb29-118">Application</span></span> | <span data-ttu-id="afb29-119">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afb29-119">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="afb29-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="afb29-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes
```
## <a name="request-headers"></a><span data-ttu-id="afb29-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="afb29-121">Request headers</span></span>
| <span data-ttu-id="afb29-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="afb29-122">Header</span></span>       | <span data-ttu-id="afb29-123">Valor</span><span class="sxs-lookup"><span data-stu-id="afb29-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="afb29-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="afb29-124">Authorization</span></span>  | <span data-ttu-id="afb29-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="afb29-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="afb29-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="afb29-127">Content-Type</span></span>  | <span data-ttu-id="afb29-128">application/json</span><span class="sxs-lookup"><span data-stu-id="afb29-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="afb29-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="afb29-129">Request body</span></span>
<span data-ttu-id="afb29-130">No corpo da solicitação, forneça uma representação JSON de um objeto [educationClass](../resources/educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="afb29-130">In the request body, supply a JSON representation of an [educationClass](../resources/educationclass.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="afb29-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="afb29-131">Response</span></span>
<span data-ttu-id="afb29-132">Se bem-sucedido, esse método retornará um código de resposta `201 Created` e um objeto [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="afb29-132">If successful, this method returns a `201 Created` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="afb29-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="afb29-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="afb29-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="afb29-134">Request</span></span>
<span data-ttu-id="afb29-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="afb29-135">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="afb29-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="afb29-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationroot"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes
Content-type: application/json
Content-length: 224

{
  "description": "Health Level 1",
  "classCode": "Health 501",
  "displayName": "Health 1",
  "externalId": "11019",
  "externalName": "Health Level 1",
  "externalSource": "sis",
  "mailNickname": "fineartschool.net"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="afb29-137">C#</span><span class="sxs-lookup"><span data-stu-id="afb29-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationclass-from-educationroot-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="afb29-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="afb29-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationclass-from-educationroot-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="afb29-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="afb29-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationclass-from-educationroot-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="afb29-140">Java</span><span class="sxs-lookup"><span data-stu-id="afb29-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationclass-from-educationroot-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="afb29-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="afb29-141">Response</span></span>
<span data-ttu-id="afb29-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="afb29-142">The following is an example of the response.</span></span> 

><span data-ttu-id="afb29-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="afb29-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 224

{
    "id": "11019",
    "description": "Health Level 1",
    "classCode": "Health 501",
    "createdBy": {
      "user": {
        "displayName": "Susana Rocha",
        "id": "14012",
      }
    },
    "displayName": "Health 1",
    "externalId": "11019",
    "externalName": "Health Level 1",
    "externalSource": "sis",
    "mailNickname": "fineartschool.net"
}
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
  "suppressions": [
  ]
}
-->
