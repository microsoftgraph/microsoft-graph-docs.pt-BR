---
title: Obter educationClass
description: Recuperar uma classe do sistema
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 52f24e1f3c02b955874a78cdba447b697485f4a3
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232008"
---
# <a name="get-educationclass"></a><span data-ttu-id="f22f1-103">Obter educationClass</span><span class="sxs-lookup"><span data-stu-id="f22f1-103">Get educationClass</span></span>

<span data-ttu-id="f22f1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f22f1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f22f1-105">Recupere uma aula do sistema.</span><span class="sxs-lookup"><span data-stu-id="f22f1-105">Retrieve a class from the system.</span></span> <span data-ttu-id="f22f1-106">Uma aula é um grupo universal com uma propriedade especial que indica ao sistema que o grupo é uma aula.</span><span class="sxs-lookup"><span data-stu-id="f22f1-106">A class is a universal group with a special property that indicates to the system that the group is a class.</span></span> <span data-ttu-id="f22f1-107">Os membros do grupo representam os alunos; os administradores de grupo representam os professores da classe.</span><span class="sxs-lookup"><span data-stu-id="f22f1-107">Group members represent the students; group admins represent the teachers in the class.</span></span> <span data-ttu-id="f22f1-108">Se estiver usando o token delegado, o usuário verá apenas as aulas das quais são membros.</span><span class="sxs-lookup"><span data-stu-id="f22f1-108">If you're using the delegated token, the user will only see classes in which they are members.</span></span>

## <a name="permissions"></a><span data-ttu-id="f22f1-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="f22f1-109">Permissions</span></span>
<span data-ttu-id="f22f1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f22f1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f22f1-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f22f1-112">Permission type</span></span>      | <span data-ttu-id="f22f1-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f22f1-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f22f1-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f22f1-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="f22f1-115">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="f22f1-115">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="f22f1-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f22f1-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f22f1-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f22f1-117">Not supported</span></span>  |
|<span data-ttu-id="f22f1-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f22f1-118">Application</span></span> | <span data-ttu-id="f22f1-119">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f22f1-119">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f22f1-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f22f1-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f22f1-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f22f1-121">Optional query parameters</span></span>
<span data-ttu-id="f22f1-122">É possível usar a opção de consulta `$select` para obter propriedades específicas do grupo, inclusive aquelas que não são retornadas por padrão.</span><span class="sxs-lookup"><span data-stu-id="f22f1-122">You can use `$select` to get specific group properties, including those that are not returned by default.</span></span>

<span data-ttu-id="f22f1-123">Para saber mais sobre as opções de consulta do OData, confira [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f22f1-123">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>
## <a name="request-headers"></a><span data-ttu-id="f22f1-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f22f1-124">Request headers</span></span>
| <span data-ttu-id="f22f1-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f22f1-125">Header</span></span>       | <span data-ttu-id="f22f1-126">Valor</span><span class="sxs-lookup"><span data-stu-id="f22f1-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f22f1-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="f22f1-127">Authorization</span></span>  | <span data-ttu-id="f22f1-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f22f1-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f22f1-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f22f1-130">Request body</span></span>
<span data-ttu-id="f22f1-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f22f1-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f22f1-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="f22f1-132">Response</span></span>
<span data-ttu-id="f22f1-133">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f22f1-133">If successful, this method returns a `200 OK` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f22f1-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f22f1-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f22f1-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f22f1-135">Request</span></span>
<span data-ttu-id="f22f1-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f22f1-136">Here is an example of the request.</span></span>

<span data-ttu-id="f22f1-137">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f22f1-137">If successful, this method returns a `200 OK` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f22f1-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f22f1-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f22f1-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f22f1-139">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_educationclass"
}
-->

```http
GET /education/classes/{educationClassId}
```

### <a name="response"></a><span data-ttu-id="f22f1-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="f22f1-140">Response</span></span>

><span data-ttu-id="f22f1-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f22f1-141">**Note:** The response object shown here might be shortened for readability.</span></span>

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
