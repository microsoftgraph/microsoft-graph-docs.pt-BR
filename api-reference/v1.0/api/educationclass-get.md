---
title: Obter educationClass
description: Recuperar uma classe do sistema
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 76393b5d6e80fc00a78c0f4344ee4d567c880afe
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474986"
---
# <a name="get-educationclass"></a><span data-ttu-id="4100a-103">Obter educationClass</span><span class="sxs-lookup"><span data-stu-id="4100a-103">Get educationClass</span></span>

<span data-ttu-id="4100a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4100a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4100a-105">Recupere uma aula do sistema.</span><span class="sxs-lookup"><span data-stu-id="4100a-105">Retrieve a class from the system.</span></span> <span data-ttu-id="4100a-106">Uma aula é um grupo universal com uma propriedade especial que indica ao sistema que o grupo é uma aula.</span><span class="sxs-lookup"><span data-stu-id="4100a-106">A class is a universal group with a special property that indicates to the system that the group is a class.</span></span> <span data-ttu-id="4100a-107">Os membros do grupo representam os alunos; os administradores de grupo representam os professores da classe.</span><span class="sxs-lookup"><span data-stu-id="4100a-107">Group members represent the students; group admins represent the teachers in the class.</span></span> <span data-ttu-id="4100a-108">Se estiver usando o token delegado, o usuário verá apenas as aulas das quais são membros.</span><span class="sxs-lookup"><span data-stu-id="4100a-108">If you're using the delegated token, the user will only see classes in which they are members.</span></span>

## <a name="permissions"></a><span data-ttu-id="4100a-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="4100a-109">Permissions</span></span>
<span data-ttu-id="4100a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4100a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4100a-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4100a-112">Permission type</span></span>      | <span data-ttu-id="4100a-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4100a-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4100a-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4100a-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="4100a-115">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="4100a-115">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="4100a-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4100a-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="4100a-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="4100a-117">Not supported</span></span>  |
|<span data-ttu-id="4100a-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4100a-118">Application</span></span> | <span data-ttu-id="4100a-119">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4100a-119">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="4100a-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4100a-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4100a-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4100a-121">Optional query parameters</span></span>
<span data-ttu-id="4100a-122">É possível usar a opção de consulta `$select` para obter propriedades específicas do grupo, inclusive aquelas que não são retornadas por padrão.</span><span class="sxs-lookup"><span data-stu-id="4100a-122">You can use `$select` to get specific group properties, including those that are not returned by default.</span></span>

<span data-ttu-id="4100a-123">Para saber mais sobre as opções de consulta do OData, confira [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="4100a-123">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>
## <a name="request-headers"></a><span data-ttu-id="4100a-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4100a-124">Request headers</span></span>
| <span data-ttu-id="4100a-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4100a-125">Header</span></span>       | <span data-ttu-id="4100a-126">Valor</span><span class="sxs-lookup"><span data-stu-id="4100a-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4100a-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="4100a-127">Authorization</span></span>  | <span data-ttu-id="4100a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4100a-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4100a-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4100a-130">Request body</span></span>
<span data-ttu-id="4100a-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4100a-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="4100a-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="4100a-132">Response</span></span>
<span data-ttu-id="4100a-133">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4100a-133">If successful, this method returns a `200 OK` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4100a-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4100a-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4100a-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4100a-135">Request</span></span>
<span data-ttu-id="4100a-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4100a-136">Here is an example of the request.</span></span>

<span data-ttu-id="4100a-137">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4100a-137">If successful, this method returns a `200 OK` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4100a-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4100a-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4100a-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4100a-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="4100a-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="4100a-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationclass"
}
-->

```msgraph-interactive
GET /education/classes/{educationClassId}
```
# <a name="c"></a>[<span data-ttu-id="4100a-141">C#</span><span class="sxs-lookup"><span data-stu-id="4100a-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationclass-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4100a-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4100a-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationclass-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4100a-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4100a-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationclass-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4100a-144">Java</span><span class="sxs-lookup"><span data-stu-id="4100a-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationclass-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4100a-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="4100a-145">Response</span></span>

><span data-ttu-id="4100a-146">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4100a-146">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.educationClass",
    "id": "64ef8ce5-8ce5-64ef-e58c-ef64e58cef64",
    "displayName": "String",
    "mailNickname": "String",
    "description": "String",
    "createdBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "classCode": "String",
    "externalName": "String",
    "externalId": "String",
    "externalSource": "String",
    "externalSourceDetail": "String",
    "grade": "String",
    "term": {
      "@odata.type": "microsoft.graph.educationTerm"
    }
  }
}
```
