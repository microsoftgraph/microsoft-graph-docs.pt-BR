---
title: Listar usuários de uma educationSchool
description: Recupere uma lista de usuários em uma escola.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: d37bec88be07f9dba3e91d44558508ce82004c74
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232001"
---
# <a name="list-users-of-an-educationschool"></a><span data-ttu-id="a30fc-103">Listar usuários de uma educationSchool</span><span class="sxs-lookup"><span data-stu-id="a30fc-103">List users of an educationSchool</span></span>

<span data-ttu-id="a30fc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a30fc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a30fc-105">Obter os [recursos educationUser](../resources/educationuser.md) associados a uma [educationSchool](../resources/educationschool.md).</span><span class="sxs-lookup"><span data-stu-id="a30fc-105">Get the [educationUser](../resources/educationuser.md) resources associated with an [educationSchool](../resources/educationschool.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a30fc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a30fc-106">Permissions</span></span>

<span data-ttu-id="a30fc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a30fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a30fc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a30fc-109">Permission type</span></span>                        | <span data-ttu-id="a30fc-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a30fc-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="a30fc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a30fc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a30fc-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a30fc-112">Not supported.</span></span>                              |
| <span data-ttu-id="a30fc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a30fc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a30fc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a30fc-114">Not supported.</span></span>                              |
| <span data-ttu-id="a30fc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a30fc-115">Application</span></span>                            | <span data-ttu-id="a30fc-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a30fc-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a30fc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a30fc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/schools/{educationSchoolId}/users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a30fc-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a30fc-118">Optional query parameters</span></span>

<span data-ttu-id="a30fc-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$search`, `$count`, e `$filter`.</span><span class="sxs-lookup"><span data-stu-id="a30fc-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span>

<span data-ttu-id="a30fc-120">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="a30fc-120">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="a30fc-121">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="a30fc-121">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

<span data-ttu-id="a30fc-122">Para obter mais informações sobre as opções de consulta OData, veja [ Parâmetros de consulta OData ](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a30fc-122">For more information on OData query options, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a30fc-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a30fc-123">Request headers</span></span>
| <span data-ttu-id="a30fc-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a30fc-124">Header</span></span>       | <span data-ttu-id="a30fc-125">Valor</span><span class="sxs-lookup"><span data-stu-id="a30fc-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a30fc-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="a30fc-126">Authorization</span></span>  | <span data-ttu-id="a30fc-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a30fc-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a30fc-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a30fc-129">Request body</span></span>
<span data-ttu-id="a30fc-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a30fc-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="a30fc-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="a30fc-131">Response</span></span>
<span data-ttu-id="a30fc-132">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationUser](../resources/educationuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a30fc-132">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a30fc-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a30fc-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a30fc-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a30fc-134">Request</span></span>
<span data-ttu-id="a30fc-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a30fc-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a30fc-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="a30fc-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationschool_get_users"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/schools/{school-id}/users
```
# <a name="c"></a>[<span data-ttu-id="a30fc-137">C#</span><span class="sxs-lookup"><span data-stu-id="a30fc-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationschool-get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a30fc-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a30fc-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationschool-get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a30fc-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a30fc-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationschool-get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a30fc-140">Java</span><span class="sxs-lookup"><span data-stu-id="a30fc-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationschool-get-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a30fc-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="a30fc-141">Response</span></span>
<span data-ttu-id="a30fc-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a30fc-142">The following is an example of the response.</span></span> 

><span data-ttu-id="a30fc-143">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a30fc-143">**Note:** The response object shown here might be shortened for readability.</span></span>

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
      "id": "13012",
      "displayName": "Dion Matheson",
      "givenName": "Dion",
      "middleName": " ",
      "surname": "Matheson",
      "mail": "DionM@contoso.com",
      "mobilePhone": "+1 (253) 555-0101",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "externalSource": "sis",
      "mailingAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
      "primaryRole": "student",
      "residenceAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
