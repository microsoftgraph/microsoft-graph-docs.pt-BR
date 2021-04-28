---
title: Obter educationClass
description: "  os administradores de grupo representam os professores da classe. Se estiver usando o token delegado, o usuário verá apenas as aulas das quais são membros."
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 4bbbe40a291657813023596d3fd42cdfcd5c3310
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048761"
---
# <a name="get-educationclass"></a><span data-ttu-id="759f2-104">Obter educationClass</span><span class="sxs-lookup"><span data-stu-id="759f2-104">Get educationClass</span></span>

<span data-ttu-id="759f2-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="759f2-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="759f2-106">Recupere uma aula do sistema.</span><span class="sxs-lookup"><span data-stu-id="759f2-106">Retrieve a class from the system.</span></span> <span data-ttu-id="759f2-107">Uma aula é um grupo universal com uma propriedade especial que indica ao sistema que o grupo é uma aula.</span><span class="sxs-lookup"><span data-stu-id="759f2-107">A class is a universal group with a special property that indicates to the system that the group is a class.</span></span> <span data-ttu-id="759f2-108">Os membros do grupo representam os alunos; os administradores do grupo representam os professores da aula.</span><span class="sxs-lookup"><span data-stu-id="759f2-108">Group members represent the students;  group admins represent the teachers in the class.</span></span> <span data-ttu-id="759f2-109">Se estiver usando o token delegado, o usuário verá apenas as aulas das quais são membros.</span><span class="sxs-lookup"><span data-stu-id="759f2-109">If you're using the delegated token, the user will only see classes in which they are members.</span></span>

## <a name="permissions"></a><span data-ttu-id="759f2-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="759f2-110">Permissions</span></span>
<span data-ttu-id="759f2-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="759f2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="759f2-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="759f2-113">Permission type</span></span>      | <span data-ttu-id="759f2-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="759f2-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="759f2-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="759f2-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="759f2-116">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="759f2-116">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="759f2-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="759f2-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="759f2-118">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="759f2-118">Not supported</span></span>  |
|<span data-ttu-id="759f2-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="759f2-119">Application</span></span> | <span data-ttu-id="759f2-120">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="759f2-120">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="759f2-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="759f2-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="759f2-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="759f2-122">Optional query parameters</span></span>
<span data-ttu-id="759f2-123">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="759f2-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="759f2-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="759f2-124">Request headers</span></span>
| <span data-ttu-id="759f2-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="759f2-125">Header</span></span>       | <span data-ttu-id="759f2-126">Valor</span><span class="sxs-lookup"><span data-stu-id="759f2-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="759f2-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="759f2-127">Authorization</span></span>  | <span data-ttu-id="759f2-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="759f2-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="759f2-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="759f2-130">Request body</span></span>
<span data-ttu-id="759f2-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="759f2-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="759f2-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="759f2-132">Response</span></span>
<span data-ttu-id="759f2-133">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="759f2-133">If successful, this method returns a `200 OK` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="759f2-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="759f2-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="759f2-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="759f2-135">Request</span></span>
<span data-ttu-id="759f2-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="759f2-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="759f2-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="759f2-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationclass"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes/{class-id}
```
# <a name="c"></a>[<span data-ttu-id="759f2-138">C#</span><span class="sxs-lookup"><span data-stu-id="759f2-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationclass-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="759f2-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="759f2-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationclass-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="759f2-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="759f2-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationclass-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="759f2-141">Java</span><span class="sxs-lookup"><span data-stu-id="759f2-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationclass-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="759f2-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="759f2-142">Response</span></span>
<span data-ttu-id="759f2-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="759f2-143">The following is an example of the response.</span></span> 

><span data-ttu-id="759f2-144">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="759f2-144">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 224

{
  "id": "11023",
  "description": "English Level 2",
  "classCode": "11023",
  "createdBy": {
    "user": {
      "displayName": "Susana Rocha",
      "id": "14012",
    }
  },
  "displayName": "English - Language 2",
  "externalId": "301",
  "externalName": "English Level 1",
  "externalSource": "School of Fine Art",
  "mailNickname": "fineartschool.net "
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
