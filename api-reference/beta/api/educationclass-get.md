---
title: Obter educationClass
description: "  administradores de grupo representam os professores da turma. Se estiver usando o token delegado, o usuário verá apenas as aulas das quais são membros."
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 576d07f13e506737393d9ca19430e556fcfc47d1
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35860631"
---
# <a name="get-educationclass"></a><span data-ttu-id="eaca9-104">Obter educationClass</span><span class="sxs-lookup"><span data-stu-id="eaca9-104">Get educationClass</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eaca9-105">Recupere uma aula do sistema.</span><span class="sxs-lookup"><span data-stu-id="eaca9-105">Retrieve a class from the system.</span></span> <span data-ttu-id="eaca9-106">Uma aula é um grupo universal com uma propriedade especial que indica ao sistema que o grupo é uma aula.</span><span class="sxs-lookup"><span data-stu-id="eaca9-106">A class is a universal group with a special property that indicates to the system that the group is a class.</span></span> <span data-ttu-id="eaca9-107">Os membros do grupo representam os alunos; os administradores do grupo representam os professores da aula.</span><span class="sxs-lookup"><span data-stu-id="eaca9-107">Group members represent the students;  group admins represent the teachers in the class.</span></span> <span data-ttu-id="eaca9-108">Se estiver usando o token delegado, o usuário verá apenas as aulas das quais são membros.</span><span class="sxs-lookup"><span data-stu-id="eaca9-108">If you're using the delegated token, the user will only see classes in which they are members.</span></span>

## <a name="permissions"></a><span data-ttu-id="eaca9-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="eaca9-109">Permissions</span></span>
<span data-ttu-id="eaca9-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eaca9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eaca9-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eaca9-112">Permission type</span></span>      | <span data-ttu-id="eaca9-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eaca9-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eaca9-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eaca9-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="eaca9-115">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="eaca9-115">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="eaca9-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eaca9-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="eaca9-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="eaca9-117">Not supported</span></span>  |
|<span data-ttu-id="eaca9-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eaca9-118">Application</span></span> | <span data-ttu-id="eaca9-119">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eaca9-119">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="eaca9-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eaca9-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="eaca9-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="eaca9-121">Optional query parameters</span></span>
<span data-ttu-id="eaca9-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="eaca9-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="eaca9-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eaca9-123">Request headers</span></span>
| <span data-ttu-id="eaca9-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="eaca9-124">Header</span></span>       | <span data-ttu-id="eaca9-125">Valor</span><span class="sxs-lookup"><span data-stu-id="eaca9-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="eaca9-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="eaca9-126">Authorization</span></span>  | <span data-ttu-id="eaca9-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eaca9-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="eaca9-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eaca9-129">Request body</span></span>
<span data-ttu-id="eaca9-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="eaca9-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="eaca9-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="eaca9-131">Response</span></span>
<span data-ttu-id="eaca9-132">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eaca9-132">If successful, this method returns a `200 OK` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="eaca9-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eaca9-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eaca9-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eaca9-134">Request</span></span>
<span data-ttu-id="eaca9-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eaca9-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="eaca9-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="eaca9-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationclass"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11023
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="eaca9-137">C#</span><span class="sxs-lookup"><span data-stu-id="eaca9-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationclass-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="eaca9-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="eaca9-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationclass-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="eaca9-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="eaca9-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationclass-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="eaca9-140">Java</span><span class="sxs-lookup"><span data-stu-id="eaca9-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationclass-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="eaca9-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="eaca9-141">Response</span></span>
<span data-ttu-id="eaca9-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="eaca9-142">The following is an example of the response.</span></span> 

><span data-ttu-id="eaca9-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eaca9-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Get educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
