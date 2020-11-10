---
title: Criar educationClass
description: Crie uma nova aula. Isso também criará um grupo universal. Quando você usar essa API para criar uma classe, ela adicionará propriedades especiais ao grupo, que será
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 18852970d0c5fe13568769639e89452f9b0e2c23
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48966057"
---
# <a name="create-educationclass"></a><span data-ttu-id="9631a-105">Criar educationClass</span><span class="sxs-lookup"><span data-stu-id="9631a-105">Create educationClass</span></span>

<span data-ttu-id="9631a-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9631a-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9631a-107">Crie uma nova aula.</span><span class="sxs-lookup"><span data-stu-id="9631a-107">Create a new class.</span></span> <span data-ttu-id="9631a-108">Isso também criará um grupo universal.</span><span class="sxs-lookup"><span data-stu-id="9631a-108">This will also create a universal group.</span></span> <span data-ttu-id="9631a-109">Quando você usar essa API para criar uma classe, ela adicionará propriedades especiais ao grupo, que adicionará recursos como atribuições e tratamento especial no Microsoft Teams quando o Teams for criado usando o grupo.</span><span class="sxs-lookup"><span data-stu-id="9631a-109">When you use this API to create a class, it will add special properties to the group, which will add features such as assignments and special handling within Microsoft Teams when teams are created using the group.</span></span> <span data-ttu-id="9631a-110">Observe que essa API apenas cria o grupo universal e não cria uma equipe.</span><span class="sxs-lookup"><span data-stu-id="9631a-110">Please note that this API only creates the universal group and does not create a team.</span></span> <span data-ttu-id="9631a-111">O Microsoft Teams oferece uma interface do usuário para que os professores criem equipes para suas próprias classes usando os grupos criados por essa API.</span><span class="sxs-lookup"><span data-stu-id="9631a-111">Microsoft Teams provides a user interface for teachers to create teams for their own classes using the groups created by this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="9631a-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="9631a-112">Permissions</span></span>
<span data-ttu-id="9631a-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9631a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9631a-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9631a-115">Permission type</span></span>      | <span data-ttu-id="9631a-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9631a-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9631a-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9631a-117">Delegated (work or school account)</span></span> |  <span data-ttu-id="9631a-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9631a-118">Not supported.</span></span>  |
|<span data-ttu-id="9631a-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9631a-119">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="9631a-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9631a-120">Not supported.</span></span>  |
|<span data-ttu-id="9631a-121">Application</span><span class="sxs-lookup"><span data-stu-id="9631a-121">Application</span></span> | <span data-ttu-id="9631a-122">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9631a-122">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="9631a-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9631a-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes
```
## <a name="request-headers"></a><span data-ttu-id="9631a-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9631a-124">Request headers</span></span>
| <span data-ttu-id="9631a-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9631a-125">Header</span></span>       | <span data-ttu-id="9631a-126">Valor</span><span class="sxs-lookup"><span data-stu-id="9631a-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9631a-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="9631a-127">Authorization</span></span>  | <span data-ttu-id="9631a-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9631a-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9631a-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9631a-130">Content-Type</span></span>  | <span data-ttu-id="9631a-131">application/json</span><span class="sxs-lookup"><span data-stu-id="9631a-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9631a-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9631a-132">Request body</span></span>
<span data-ttu-id="9631a-133">No corpo da solicitação, forneça uma representação JSON de um objeto [educationClass](../resources/educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="9631a-133">In the request body, supply a JSON representation of an [educationClass](../resources/educationclass.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="9631a-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="9631a-134">Response</span></span>
<span data-ttu-id="9631a-135">Se bem-sucedido, esse método retornará um código de resposta `201 Created` e um objeto [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9631a-135">If successful, this method returns a `201 Created` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9631a-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9631a-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9631a-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9631a-137">Request</span></span>
<span data-ttu-id="9631a-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9631a-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9631a-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="9631a-139">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="9631a-140">C#</span><span class="sxs-lookup"><span data-stu-id="9631a-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationclass-from-educationroot-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9631a-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9631a-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationclass-from-educationroot-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9631a-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9631a-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationclass-from-educationroot-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9631a-143">Java</span><span class="sxs-lookup"><span data-stu-id="9631a-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationclass-from-educationroot-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9631a-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="9631a-144">Response</span></span>
<span data-ttu-id="9631a-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9631a-145">The following is an example of the response.</span></span> 

><span data-ttu-id="9631a-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9631a-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


