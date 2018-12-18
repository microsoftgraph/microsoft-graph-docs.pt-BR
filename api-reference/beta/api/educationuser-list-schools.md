---
title: Listar escolas
description: Recupere uma lista de escolas de um usuário.
author: mmast-msft
ms.openlocfilehash: 35810f4b1928249576ac1216356701489f68feca
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303266"
---
# <a name="list-schools"></a><span data-ttu-id="a6a60-103">Listar escolas</span><span class="sxs-lookup"><span data-stu-id="a6a60-103">List schools</span></span>

> <span data-ttu-id="a6a60-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a6a60-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a6a60-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a6a60-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a6a60-106">Recupere uma lista de escolas de um usuário.</span><span class="sxs-lookup"><span data-stu-id="a6a60-106">Retrieve a list of schools for a user.</span></span>

><span data-ttu-id="a6a60-107">**Observação:** se o token delegado for usado, os membros só poderão ver informações sobre as próprias escolas.</span><span class="sxs-lookup"><span data-stu-id="a6a60-107">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="a6a60-108">Nesse caso, use o recurso `...beta/education/me/schools`.</span><span class="sxs-lookup"><span data-stu-id="a6a60-108">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="a6a60-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="a6a60-109">Permissions</span></span>
<span data-ttu-id="a6a60-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6a60-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6a60-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a6a60-112">Permission type</span></span>      | <span data-ttu-id="a6a60-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a6a60-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a6a60-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a6a60-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="a6a60-115">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="a6a60-115">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="a6a60-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a6a60-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="a6a60-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6a60-117">Not supported.</span></span>  |
|<span data-ttu-id="a6a60-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a6a60-118">Application</span></span> | <span data-ttu-id="a6a60-119">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6a60-119">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="a6a60-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a6a60-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/schools
GET /education/users/{id}/schools
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a6a60-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a6a60-121">Optional query parameters</span></span>
<span data-ttu-id="a6a60-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a6a60-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a6a60-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a6a60-123">Request headers</span></span>
| <span data-ttu-id="a6a60-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a6a60-124">Header</span></span>       | <span data-ttu-id="a6a60-125">Valor</span><span class="sxs-lookup"><span data-stu-id="a6a60-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a6a60-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="a6a60-126">Authorization</span></span>  | <span data-ttu-id="a6a60-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a6a60-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a6a60-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a6a60-129">Request body</span></span>
<span data-ttu-id="a6a60-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a6a60-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="a6a60-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6a60-131">Response</span></span>
<span data-ttu-id="a6a60-132">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationSchool](../resources/educationschool.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a6a60-132">If successful, this method returns a `200 OK` response code and a collection of [educationSchool](../resources/educationschool.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a6a60-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a6a60-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a6a60-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a6a60-134">Request</span></span>
<span data-ttu-id="a6a60-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a6a60-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_schools"
}-->
```http
GET https://graph.microsoft.com/beta/education/me/schools
```
##### <a name="response"></a><span data-ttu-id="a6a60-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6a60-136">Response</span></span>
<span data-ttu-id="a6a60-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a6a60-137">The following is an example of the response.</span></span> 

><span data-ttu-id="a6a60-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a6a60-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 345

{
  "value": [
    {
      "id": "10001",
      "displayName": "Contoso High School",
      "description": "Public 9-12 high school",
      "status": "active",
      "externalSource": "sis",
      "principalEmail": "amyr@contoso.com",
      "principalName": "Amy Roebuck",
      "externalPrincipalId": "14007",
      "highestGrade": "12",
      "lowestGrade": "9",
      "schoolNumber": "10001",
      "address": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "externalId": "10001",
      "fax": "+1 (253) 555-0101",
      "phone": "+1 (253) 555-0102",
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List schools",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->