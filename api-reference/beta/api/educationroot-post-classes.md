---
title: Criar educationClass
description: Crie uma nova aula. Isso também criará um grupo universal. Quando você usar essa API para criar uma classe, ela adicionará propriedades especiais ao grupo, que será
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 7d3856d17954d04a02a95a24571d16f4b51a149f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42426091"
---
# <a name="create-educationclass"></a><span data-ttu-id="f7a66-105">Criar educationClass</span><span class="sxs-lookup"><span data-stu-id="f7a66-105">Create educationClass</span></span>

<span data-ttu-id="f7a66-106">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f7a66-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7a66-107">Crie uma nova aula.</span><span class="sxs-lookup"><span data-stu-id="f7a66-107">Create a new class.</span></span> <span data-ttu-id="f7a66-108">Isso também criará um grupo universal.</span><span class="sxs-lookup"><span data-stu-id="f7a66-108">This will also create a universal group.</span></span> <span data-ttu-id="f7a66-109">Quando você usar essa API para criar uma aula, ela adicionará propriedades especiais ao grupo, que adicionará recursos como atribuições e tratamento especial no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="f7a66-109">When you use this API to create a class, it will add special properties to the group, which will add features such as assignments and special handling within Microsoft Teams.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7a66-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="f7a66-110">Permissions</span></span>
<span data-ttu-id="f7a66-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7a66-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7a66-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f7a66-113">Permission type</span></span>      | <span data-ttu-id="f7a66-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f7a66-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7a66-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f7a66-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="f7a66-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7a66-116">Not supported.</span></span>  |
|<span data-ttu-id="f7a66-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f7a66-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f7a66-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7a66-118">Not supported.</span></span>  |
|<span data-ttu-id="f7a66-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f7a66-119">Application</span></span> | <span data-ttu-id="f7a66-120">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7a66-120">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f7a66-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f7a66-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes
```
## <a name="request-headers"></a><span data-ttu-id="f7a66-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f7a66-122">Request headers</span></span>
| <span data-ttu-id="f7a66-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f7a66-123">Header</span></span>       | <span data-ttu-id="f7a66-124">Valor</span><span class="sxs-lookup"><span data-stu-id="f7a66-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f7a66-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f7a66-125">Authorization</span></span>  | <span data-ttu-id="f7a66-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f7a66-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f7a66-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f7a66-128">Content-Type</span></span>  | <span data-ttu-id="f7a66-129">application/json</span><span class="sxs-lookup"><span data-stu-id="f7a66-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f7a66-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f7a66-130">Request body</span></span>
<span data-ttu-id="f7a66-131">No corpo da solicitação, forneça uma representação JSON de um objeto [educationClass](../resources/educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="f7a66-131">In the request body, supply a JSON representation of an [educationClass](../resources/educationclass.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="f7a66-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7a66-132">Response</span></span>
<span data-ttu-id="f7a66-133">Se bem-sucedido, esse método retornará um código de resposta `201 Created` e um objeto [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f7a66-133">If successful, this method returns a `201 Created` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7a66-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f7a66-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f7a66-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f7a66-135">Request</span></span>
<span data-ttu-id="f7a66-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f7a66-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f7a66-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="f7a66-137">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="f7a66-138">C#</span><span class="sxs-lookup"><span data-stu-id="f7a66-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationclass-from-educationroot-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f7a66-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f7a66-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationclass-from-educationroot-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f7a66-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f7a66-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationclass-from-educationroot-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f7a66-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7a66-141">Response</span></span>
<span data-ttu-id="f7a66-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f7a66-142">The following is an example of the response.</span></span> 

><span data-ttu-id="f7a66-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f7a66-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
