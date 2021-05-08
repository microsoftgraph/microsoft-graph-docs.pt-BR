---
title: Listar membros de uma educationClass
description: Recupere os professores e alunos de uma aula. Se o token delegado for usado, os membros poderão ser vistos apenas por outros membros da aula.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: eadc2f00fee83f3663ab983118f92ce84f8cc607
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232088"
---
# <a name="list-members-of-an-educationclass"></a><span data-ttu-id="6b9eb-104">Listar membros de uma educationClass</span><span class="sxs-lookup"><span data-stu-id="6b9eb-104">List members of an educationClass</span></span>

<span data-ttu-id="6b9eb-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b9eb-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6b9eb-106">Recupera os [membros educationUser](../resources/educationuser.md) de uma [educationClass](../resources/educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="6b9eb-106">Retrieves the [educationUser](../resources/educationuser.md) members of an [educationClass](../resources/educationclass.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6b9eb-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="6b9eb-107">Permissions</span></span>
<span data-ttu-id="6b9eb-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b9eb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6b9eb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6b9eb-110">Permission type</span></span>                        | <span data-ttu-id="6b9eb-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6b9eb-111">Permissions (from least to most privileged)</span></span>                         |
| :------------------------------------- | :------------------------------------------------------------------ |
| <span data-ttu-id="6b9eb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6b9eb-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="6b9eb-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="6b9eb-113">EduRoster.ReadBasic</span></span>                                                 |
| <span data-ttu-id="6b9eb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6b9eb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b9eb-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="6b9eb-115">Not supported</span></span>                                                       |
| <span data-ttu-id="6b9eb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6b9eb-116">Application</span></span>                            | <span data-ttu-id="6b9eb-117">EduRoster.Read.All, EduRoster.ReadWrite.All mais Member.Read.Hidden</span><span class="sxs-lookup"><span data-stu-id="6b9eb-117">EduRoster.Read.All, EduRoster.ReadWrite.All plus Member.Read.Hidden</span></span> |

> [!NOTE]
> <span data-ttu-id="6b9eb-118">Se o token delegado for usado, os membros só poderão ver informações sobre suas próprias aulas.</span><span class="sxs-lookup"><span data-stu-id="6b9eb-118">Note that if the delegated token is used, members can only see information about their own classes.</span></span>

## <a name="http-request"></a><span data-ttu-id="6b9eb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6b9eb-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6b9eb-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6b9eb-120">Optional query parameters</span></span>

<span data-ttu-id="6b9eb-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$search`, `$count`, e `$filter`.</span><span class="sxs-lookup"><span data-stu-id="6b9eb-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span>

<span data-ttu-id="6b9eb-122">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="6b9eb-122">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="6b9eb-123">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="6b9eb-123">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

<span data-ttu-id="6b9eb-124">Para obter mais informações sobre as opções de consulta OData, veja [ Parâmetros de consulta OData ](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="6b9eb-124">For more information on OData query options, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6b9eb-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6b9eb-125">Request headers</span></span>
| <span data-ttu-id="6b9eb-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6b9eb-126">Header</span></span>       | <span data-ttu-id="6b9eb-127">Valor</span><span class="sxs-lookup"><span data-stu-id="6b9eb-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6b9eb-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="6b9eb-128">Authorization</span></span>  | <span data-ttu-id="6b9eb-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6b9eb-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6b9eb-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6b9eb-131">Request body</span></span>
<span data-ttu-id="6b9eb-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6b9eb-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="6b9eb-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b9eb-133">Response</span></span>
<span data-ttu-id="6b9eb-134">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationUser](../resources/educationuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6b9eb-134">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6b9eb-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6b9eb-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6b9eb-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6b9eb-136">Request</span></span>
<span data-ttu-id="6b9eb-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6b9eb-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6b9eb-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="6b9eb-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationclass_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes/{class-id}/members
```
# <a name="c"></a>[<span data-ttu-id="6b9eb-139">C#</span><span class="sxs-lookup"><span data-stu-id="6b9eb-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationclass-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6b9eb-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6b9eb-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationclass-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6b9eb-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6b9eb-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationclass-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6b9eb-142">Java</span><span class="sxs-lookup"><span data-stu-id="6b9eb-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationclass-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6b9eb-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b9eb-143">Response</span></span>
<span data-ttu-id="6b9eb-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6b9eb-144">The following is an example of the response.</span></span> 

><span data-ttu-id="6b9eb-145">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6b9eb-145">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 593

{
  "value": [
    {
      "id": "13013",
      "displayName": "Ora Klein",
      "givenName": "Ora",
      "middleName": " ",
      "surname": "Klein",
      "mail": "OraK@contoso.com",
      "mobilePhone": "+1 (253) 555-0101",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "externalSource": "School of Fine Art",
      "mailingAddress": {
        "city": "Buffalo",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "NY",
        "street": "12345 Main St."
      },
      "primaryRole": "teacher",
      "residenceAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
      "teacher": {
        "externalId": "13013",
        "teacherNumber": "8802",
      }
    },
    {
      "id": "13005",
      "displayName": "Erna Parker",
      "givenName": "Erna",
      "middleName": " ",
      "surname": "Parker",
      "mail": "ernap@contoso.com",
      "mobilePhone": "+1 (253) 555-0104",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "externalSource": "School of Fine Art",
      "mailingAddress": {
        "city": "Buffalo",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "NY",
        "street": "12345 Main St."
      },
      "student": {
        "birthDate": "2001-01-01T00:00:00Z",
        "externalId": "13005",
        "gender": "female",
        "grade": "9",
        "graduationYear": "2019",
        "studentNumber": "13005",
      },
      "primaryRole": "student",
      "residenceAddress": {
        "city": "Long Beach",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Maple St."
      },
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
