---
title: Criar educationClass
description: Crie uma nova aula. Isso também criará um grupo universal. Quando você usa essa API para criar uma classe, ela adicionará propriedades especiais ao grupo, que adicionará
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: df566e35dd2bed527ef36f181cd9c4c92791843e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52043639"
---
# <a name="create-educationclass"></a><span data-ttu-id="088a7-105">Criar educationClass</span><span class="sxs-lookup"><span data-stu-id="088a7-105">Create educationClass</span></span>

<span data-ttu-id="088a7-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="088a7-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="088a7-107">Crie uma nova aula.</span><span class="sxs-lookup"><span data-stu-id="088a7-107">Create a new class.</span></span> <span data-ttu-id="088a7-108">Isso também criará um grupo universal.</span><span class="sxs-lookup"><span data-stu-id="088a7-108">This will also create a universal group.</span></span> <span data-ttu-id="088a7-109">Quando você usa essa API para criar uma classe, ela adicionará propriedades especiais ao grupo, que adicionará recursos como atribuições e tratamento especial no Microsoft Teams quando as equipes são criadas usando o grupo.</span><span class="sxs-lookup"><span data-stu-id="088a7-109">When you use this API to create a class, it will add special properties to the group, which will add features such as assignments and special handling within Microsoft Teams when teams are created using the group.</span></span> <span data-ttu-id="088a7-110">Observe que essa API cria apenas o grupo universal e não cria uma equipe.</span><span class="sxs-lookup"><span data-stu-id="088a7-110">Please note that this API only creates the universal group and does not create a team.</span></span> <span data-ttu-id="088a7-111">Microsoft Teams fornece uma interface de usuário para que os professores criem equipes para suas próprias classes usando os grupos criados por essa API.</span><span class="sxs-lookup"><span data-stu-id="088a7-111">Microsoft Teams provides a user interface for teachers to create teams for their own classes using the groups created by this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="088a7-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="088a7-112">Permissions</span></span>
<span data-ttu-id="088a7-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="088a7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="088a7-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="088a7-115">Permission type</span></span>      | <span data-ttu-id="088a7-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="088a7-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="088a7-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="088a7-117">Delegated (work or school account)</span></span> |  <span data-ttu-id="088a7-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="088a7-118">Not supported.</span></span>  |
|<span data-ttu-id="088a7-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="088a7-119">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="088a7-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="088a7-120">Not supported.</span></span>  |
|<span data-ttu-id="088a7-121">Application</span><span class="sxs-lookup"><span data-stu-id="088a7-121">Application</span></span> | <span data-ttu-id="088a7-122">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="088a7-122">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="088a7-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="088a7-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes
```
## <a name="request-headers"></a><span data-ttu-id="088a7-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="088a7-124">Request headers</span></span>
| <span data-ttu-id="088a7-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="088a7-125">Header</span></span>       | <span data-ttu-id="088a7-126">Valor</span><span class="sxs-lookup"><span data-stu-id="088a7-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="088a7-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="088a7-127">Authorization</span></span>  | <span data-ttu-id="088a7-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="088a7-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="088a7-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="088a7-130">Content-Type</span></span>  | <span data-ttu-id="088a7-131">application/json</span><span class="sxs-lookup"><span data-stu-id="088a7-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="088a7-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="088a7-132">Request body</span></span>
<span data-ttu-id="088a7-133">No corpo da solicitação, forneça uma representação JSON de um objeto [educationClass](../resources/educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="088a7-133">In the request body, supply a JSON representation of an [educationClass](../resources/educationclass.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="088a7-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="088a7-134">Response</span></span>
<span data-ttu-id="088a7-135">Se bem-sucedido, esse método retornará um código de resposta `201 Created` e um objeto [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="088a7-135">If successful, this method returns a `201 Created` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="088a7-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="088a7-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="088a7-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="088a7-137">Request</span></span>
<span data-ttu-id="088a7-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="088a7-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="088a7-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="088a7-139">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="088a7-140">C#</span><span class="sxs-lookup"><span data-stu-id="088a7-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationclass-from-educationroot-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="088a7-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="088a7-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationclass-from-educationroot-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="088a7-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="088a7-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationclass-from-educationroot-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="088a7-143">Java</span><span class="sxs-lookup"><span data-stu-id="088a7-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationclass-from-educationroot-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="088a7-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="088a7-144">Response</span></span>
<span data-ttu-id="088a7-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="088a7-145">The following is an example of the response.</span></span> 

><span data-ttu-id="088a7-146">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="088a7-146">**Note:** The response object shown here might be shortened for readability.</span></span>

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


