---
title: Obter educationSchool
description: Recupere as propriedades e relações do objeto de escola.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 147719bc340cb987ccf0dd4370ed5e2732a263f7
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48457623"
---
# <a name="get-educationschool"></a><span data-ttu-id="27e68-103">Obter educationSchool</span><span class="sxs-lookup"><span data-stu-id="27e68-103">Get educationSchool</span></span>

<span data-ttu-id="27e68-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27e68-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27e68-105">Recupere as propriedades e relações do objeto de escola.</span><span class="sxs-lookup"><span data-stu-id="27e68-105">Retrieve the properties and relationships of the school object.</span></span>

## <a name="permissions"></a><span data-ttu-id="27e68-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="27e68-106">Permissions</span></span>
<span data-ttu-id="27e68-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27e68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27e68-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="27e68-109">Permission type</span></span>      | <span data-ttu-id="27e68-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="27e68-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="27e68-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="27e68-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="27e68-112">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="27e68-112">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="27e68-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="27e68-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="27e68-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27e68-114">Not supported.</span></span>  |
|<span data-ttu-id="27e68-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="27e68-115">Application</span></span> | <span data-ttu-id="27e68-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27e68-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="27e68-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27e68-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools
GET /education/me/schools
GET /education/users/schools
```
## <a name="optional-query-parameters"></a><span data-ttu-id="27e68-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="27e68-118">Optional query parameters</span></span>
<span data-ttu-id="27e68-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="27e68-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="27e68-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="27e68-120">Request headers</span></span>
| <span data-ttu-id="27e68-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="27e68-121">Header</span></span>       | <span data-ttu-id="27e68-122">Valor</span><span class="sxs-lookup"><span data-stu-id="27e68-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="27e68-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="27e68-123">Authorization</span></span>  | <span data-ttu-id="27e68-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27e68-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="27e68-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="27e68-126">Request body</span></span>
<span data-ttu-id="27e68-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="27e68-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="27e68-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="27e68-128">Response</span></span>
<span data-ttu-id="27e68-129">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [educationSchool](../resources/educationschool.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27e68-129">If successful, this method returns a `200 OK` response code and an [educationSchool](../resources/educationschool.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="27e68-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="27e68-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="27e68-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27e68-131">Request</span></span>
<span data-ttu-id="27e68-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="27e68-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="27e68-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="27e68-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationschool"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/schools/10001
```
# <a name="c"></a>[<span data-ttu-id="27e68-134">C#</span><span class="sxs-lookup"><span data-stu-id="27e68-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="27e68-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="27e68-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="27e68-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="27e68-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="27e68-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="27e68-137">Response</span></span>
<span data-ttu-id="27e68-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="27e68-138">The following is an example of the response.</span></span> 

><span data-ttu-id="27e68-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="27e68-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 292

{
  "schoolPrincipalEmail": "AmyRoebuck@contoso.com",
  "schoolPrincipalName": "Amy Roebuck",
  "externalSchoolPrincipalId": "14007",
  "lowestGrade": "9",
  "highestGrade": "12"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get educationSchool",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
