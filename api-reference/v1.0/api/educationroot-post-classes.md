---
title: Criar educationClass
description: Crie uma nova aula. Isso também criará um grupo universal. Quando você usar essa API para criar uma classe, ela adicionará propriedades especiais ao grupo, que será
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 56ca90f828d5b7b14c2761b5a73983268b12b5e7
ms.sourcegitcommit: ef9e0fd8fb6047fa9272e98310eaed2c4e0a2660
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/23/2020
ms.locfileid: "44353529"
---
# <a name="create-educationclass"></a><span data-ttu-id="aef20-105">Criar educationClass</span><span class="sxs-lookup"><span data-stu-id="aef20-105">Create educationClass</span></span>

<span data-ttu-id="aef20-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aef20-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="aef20-107">Crie uma nova aula.</span><span class="sxs-lookup"><span data-stu-id="aef20-107">Create a new class.</span></span> <span data-ttu-id="aef20-108">Isso também criará um grupo universal.</span><span class="sxs-lookup"><span data-stu-id="aef20-108">This will also create a universal group.</span></span> <span data-ttu-id="aef20-109">Quando você usar essa API para criar uma classe, ela adicionará propriedades especiais ao grupo, que adicionará recursos como atribuições e tratamento especial no Microsoft Teams quando o Teams for criado usando o grupo.</span><span class="sxs-lookup"><span data-stu-id="aef20-109">When you use this API to create a class, it will add special properties to the group, which will add features such as assignments and special handling within Microsoft Teams when teams are created using the group.</span></span> <span data-ttu-id="aef20-110">Observe que essa API apenas cria o grupo universal e não cria uma equipe.</span><span class="sxs-lookup"><span data-stu-id="aef20-110">Please note that this API only creates the universal group and does not create a team.</span></span> <span data-ttu-id="aef20-111">O Microsoft Teams oferece uma interface do usuário para que os professores criem equipes para suas próprias classes usando os grupos criados por essa API.</span><span class="sxs-lookup"><span data-stu-id="aef20-111">Microsoft Teams provides a user interface for teachers to create teams for their own classes using the groups created by this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="aef20-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="aef20-112">Permissions</span></span>
<span data-ttu-id="aef20-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aef20-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aef20-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aef20-115">Permission type</span></span>      | <span data-ttu-id="aef20-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aef20-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aef20-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aef20-117">Delegated (work or school account)</span></span> |  <span data-ttu-id="aef20-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aef20-118">Not supported.</span></span>  |
|<span data-ttu-id="aef20-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aef20-119">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="aef20-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aef20-120">Not supported.</span></span>  |
|<span data-ttu-id="aef20-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aef20-121">Application</span></span> | <span data-ttu-id="aef20-122">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aef20-122">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="aef20-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aef20-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes
```
## <a name="request-headers"></a><span data-ttu-id="aef20-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aef20-124">Request headers</span></span>
| <span data-ttu-id="aef20-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="aef20-125">Header</span></span>       | <span data-ttu-id="aef20-126">Valor</span><span class="sxs-lookup"><span data-stu-id="aef20-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="aef20-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="aef20-127">Authorization</span></span>  | <span data-ttu-id="aef20-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aef20-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="aef20-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="aef20-130">Content-Type</span></span>  | <span data-ttu-id="aef20-131">application/json</span><span class="sxs-lookup"><span data-stu-id="aef20-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="aef20-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aef20-132">Request body</span></span>
<span data-ttu-id="aef20-133">No corpo da solicitação, forneça uma representação JSON de um objeto [educationClass](../resources/educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="aef20-133">In the request body, supply a JSON representation of an [educationClass](../resources/educationclass.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="aef20-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="aef20-134">Response</span></span>
<span data-ttu-id="aef20-135">Se bem-sucedido, esse método retornará um código de resposta `201 Created` e um objeto [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aef20-135">If successful, this method returns a `201 Created` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aef20-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aef20-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aef20-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aef20-137">Request</span></span>
<span data-ttu-id="aef20-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="aef20-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="aef20-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="aef20-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationroot"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/classes
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
# <a name="c"></a>[<span data-ttu-id="aef20-140">C#</span><span class="sxs-lookup"><span data-stu-id="aef20-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationclass-from-educationroot-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aef20-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aef20-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationclass-from-educationroot-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aef20-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aef20-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationclass-from-educationroot-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="aef20-143">Java</span><span class="sxs-lookup"><span data-stu-id="aef20-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationclass-from-educationroot-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="aef20-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="aef20-144">Response</span></span>
<span data-ttu-id="aef20-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="aef20-145">The following is an example of the response.</span></span> 

><span data-ttu-id="aef20-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aef20-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
