---
title: Listar membros
description: Recupere os professores e alunos de uma aula. Se o token delegado for usado, os membros poderão ser vistos apenas por outros membros da aula.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 09c02d13a6c8c74b8e9cca690f605fa4ee128e67
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915288"
---
# <a name="list-members"></a><span data-ttu-id="d88fc-104">Listar membros</span><span class="sxs-lookup"><span data-stu-id="d88fc-104">List members</span></span>

> <span data-ttu-id="d88fc-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d88fc-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d88fc-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d88fc-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d88fc-107">Recupere os professores e alunos de uma aula.</span><span class="sxs-lookup"><span data-stu-id="d88fc-107">Retrieves the teachers and students for a class.</span></span> <span data-ttu-id="d88fc-108">Se o token delegado for usado, os membros poderão ser vistos apenas por outros membros da aula.</span><span class="sxs-lookup"><span data-stu-id="d88fc-108">Note that if the delegated token is used, members can only be seen by other members of the class.</span></span>

## <a name="permissions"></a><span data-ttu-id="d88fc-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="d88fc-109">Permissions</span></span>
<span data-ttu-id="d88fc-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d88fc-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d88fc-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d88fc-112">Permission type</span></span>      | <span data-ttu-id="d88fc-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d88fc-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d88fc-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d88fc-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="d88fc-115">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="d88fc-115">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="d88fc-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d88fc-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d88fc-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d88fc-117">Not supported</span></span>  |
|<span data-ttu-id="d88fc-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d88fc-118">Application</span></span> | <span data-ttu-id="d88fc-119">EduRoster.Read.All, EduRoster.ReadWrite.All mais Member.Read.Hidden</span><span class="sxs-lookup"><span data-stu-id="d88fc-119">EduRoster.Read.All, EduRoster.ReadWrite.All plus Member.Read.Hidden</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d88fc-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d88fc-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d88fc-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d88fc-121">Optional query parameters</span></span>
<span data-ttu-id="d88fc-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d88fc-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d88fc-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d88fc-123">Request headers</span></span>
| <span data-ttu-id="d88fc-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d88fc-124">Header</span></span>       | <span data-ttu-id="d88fc-125">Valor</span><span class="sxs-lookup"><span data-stu-id="d88fc-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d88fc-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="d88fc-126">Authorization</span></span>  | <span data-ttu-id="d88fc-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d88fc-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d88fc-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d88fc-129">Request body</span></span>
<span data-ttu-id="d88fc-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d88fc-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d88fc-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d88fc-131">Response</span></span>
<span data-ttu-id="d88fc-132">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationUser](../resources/educationuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d88fc-132">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d88fc-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d88fc-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d88fc-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d88fc-134">Request</span></span>
<span data-ttu-id="d88fc-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d88fc-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11016/members
```
##### <a name="response"></a><span data-ttu-id="d88fc-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d88fc-136">Response</span></span>
<span data-ttu-id="d88fc-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d88fc-137">The following is an example of the response.</span></span> 

><span data-ttu-id="d88fc-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d88fc-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "externalId": "13013",
      "teacherNumber": "8802",
      "residenceAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
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
      "primaryRole": "student",
      "externalId": "13005",
      "birthDate": "2001-01-01T00:00:00Z",
      "gender": "female",
      "grade": "9",
      "graduationYear": "2019",
      "studentNumber": "13005",
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
  "tocPath": ""
}-->
