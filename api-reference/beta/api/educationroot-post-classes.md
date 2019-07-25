---
title: Criar educationClass
description: Crie uma nova aula. Isso também criará um grupo universal. Quando você usar essa API para criar uma classe, ela adicionará propriedades especiais ao grupo, que será
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: c865a15b8cca394bcce6316e1acc8633dcb7ac8b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35860420"
---
# <a name="create-educationclass"></a><span data-ttu-id="51daf-105">Criar educationClass</span><span class="sxs-lookup"><span data-stu-id="51daf-105">Create educationClass</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51daf-106">Crie uma nova aula.</span><span class="sxs-lookup"><span data-stu-id="51daf-106">Create a new class.</span></span> <span data-ttu-id="51daf-107">Isso também criará um grupo universal.</span><span class="sxs-lookup"><span data-stu-id="51daf-107">This will also create a universal group.</span></span> <span data-ttu-id="51daf-108">Quando você usar essa API para criar uma aula, ela adicionará propriedades especiais ao grupo, que adicionará recursos como atribuições e tratamento especial no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="51daf-108">When you use this API to create a class, it will add special properties to the group, which will add features such as assignments and special handling within Microsoft Teams.</span></span>

## <a name="permissions"></a><span data-ttu-id="51daf-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="51daf-109">Permissions</span></span>
<span data-ttu-id="51daf-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51daf-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51daf-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="51daf-112">Permission type</span></span>      | <span data-ttu-id="51daf-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="51daf-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="51daf-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="51daf-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="51daf-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="51daf-115">Not supported.</span></span>  |
|<span data-ttu-id="51daf-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="51daf-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="51daf-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="51daf-117">Not supported.</span></span>  |
|<span data-ttu-id="51daf-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="51daf-118">Application</span></span> | <span data-ttu-id="51daf-119">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51daf-119">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="51daf-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="51daf-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes
```
## <a name="request-headers"></a><span data-ttu-id="51daf-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="51daf-121">Request headers</span></span>
| <span data-ttu-id="51daf-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="51daf-122">Header</span></span>       | <span data-ttu-id="51daf-123">Valor</span><span class="sxs-lookup"><span data-stu-id="51daf-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="51daf-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="51daf-124">Authorization</span></span>  | <span data-ttu-id="51daf-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="51daf-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="51daf-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="51daf-127">Content-Type</span></span>  | <span data-ttu-id="51daf-128">application/json</span><span class="sxs-lookup"><span data-stu-id="51daf-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="51daf-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="51daf-129">Request body</span></span>
<span data-ttu-id="51daf-130">No corpo da solicitação, forneça uma representação JSON de um objeto [educationClass](../resources/educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="51daf-130">In the request body, supply a JSON representation of an [educationClass](../resources/educationclass.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="51daf-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="51daf-131">Response</span></span>
<span data-ttu-id="51daf-132">Se bem-sucedido, esse método retornará um código de resposta `201 Created` e um objeto [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="51daf-132">If successful, this method returns a `201 Created` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51daf-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="51daf-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="51daf-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="51daf-134">Request</span></span>
<span data-ttu-id="51daf-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="51daf-135">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="51daf-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="51daf-136">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="51daf-137">C#</span><span class="sxs-lookup"><span data-stu-id="51daf-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationclass-from-educationroot-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="51daf-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="51daf-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationclass-from-educationroot-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="51daf-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="51daf-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationclass-from-educationroot-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="51daf-140">Java</span><span class="sxs-lookup"><span data-stu-id="51daf-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationclass-from-educationroot-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="51daf-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="51daf-141">Response</span></span>
<span data-ttu-id="51daf-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="51daf-142">The following is an example of the response.</span></span> 

><span data-ttu-id="51daf-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="51daf-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
