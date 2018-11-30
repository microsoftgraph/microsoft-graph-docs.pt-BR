---
title: Listar escolas
description: Recupere uma lista de escolas nas quais a aula é ministrada.
ms.openlocfilehash: 22fd9044e70e2f1bc8cea4789cef11a78c9d374e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035306"
---
# <a name="list-schools"></a><span data-ttu-id="3e3fc-103">Listar escolas</span><span class="sxs-lookup"><span data-stu-id="3e3fc-103">List schools</span></span>

> <span data-ttu-id="3e3fc-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3e3fc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3e3fc-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3e3fc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3e3fc-106">Recupere uma lista de escolas nas quais a aula é ministrada.</span><span class="sxs-lookup"><span data-stu-id="3e3fc-106">Retrieve a list of schools in which the class is taught.</span></span>

## <a name="permissions"></a><span data-ttu-id="3e3fc-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="3e3fc-107">Permissions</span></span>
<span data-ttu-id="3e3fc-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e3fc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e3fc-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3e3fc-110">Permission type</span></span>      | <span data-ttu-id="3e3fc-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3e3fc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e3fc-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3e3fc-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="3e3fc-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="3e3fc-113">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="3e3fc-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3e3fc-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="3e3fc-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="3e3fc-115">Not supported</span></span>  |
|<span data-ttu-id="3e3fc-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3e3fc-116">Application</span></span> | <span data-ttu-id="3e3fc-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e3fc-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="3e3fc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3e3fc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/schools
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3e3fc-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3e3fc-119">Optional query parameters</span></span>
<span data-ttu-id="3e3fc-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3e3fc-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3e3fc-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3e3fc-121">Request headers</span></span>
| <span data-ttu-id="3e3fc-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3e3fc-122">Header</span></span>       | <span data-ttu-id="3e3fc-123">Valor</span><span class="sxs-lookup"><span data-stu-id="3e3fc-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3e3fc-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="3e3fc-124">Authorization</span></span>  | <span data-ttu-id="3e3fc-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3e3fc-p103">Bearer {token}. Required.</span></span>  |


## <a name="request-body"></a><span data-ttu-id="3e3fc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3e3fc-127">Request body</span></span>
<span data-ttu-id="3e3fc-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3e3fc-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="3e3fc-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e3fc-129">Response</span></span>
<span data-ttu-id="3e3fc-130">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationSchool](../resources/educationschool.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3e3fc-130">If successful, this method returns a `200 OK` response code and a collection of [educationSchool](../resources/educationschool.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3e3fc-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3e3fc-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3e3fc-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3e3fc-132">Request</span></span>
<span data-ttu-id="3e3fc-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3e3fc-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_schools"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11014/schools
```
##### <a name="response"></a><span data-ttu-id="3e3fc-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e3fc-134">Response</span></span>
<span data-ttu-id="3e3fc-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3e3fc-135">The following is an example of the response.</span></span> 

><span data-ttu-id="3e3fc-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3e3fc-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 892

{
  "value": [
    {
      "id": "10002",
      "displayName": "Fabrikam High School",
      "description": "Magnate school for the arts. Los Angeles School District",
      "status": "String",
      "externalSource": "String",
      "principalEmail": "AmyR@fabrikam.com",
      "principalName": "Amy Roebuck",
      "externalPrincipalId": "14007",
      "highestGrade": "12",
      "lowestGrade": "9",
      "schoolNumber": "10002",
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
      "externalId": "10002",
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
