---
title: Obter educationUser
description: Leia as propriedades e as relações de um objeto educationUser.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: e550f1dc17f562f0d9f6db51001b4bcc26166eed
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231274"
---
# <a name="get-educationuser"></a><span data-ttu-id="a0dc9-103">Obter educationUser</span><span class="sxs-lookup"><span data-stu-id="a0dc9-103">Get educationUser</span></span>

<span data-ttu-id="a0dc9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0dc9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a0dc9-105">Leia as propriedades e as relações de um [objeto educationUser.](../resources/educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="a0dc9-105">Read the properties and relationships of an [educationUser](../resources/educationuser.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a0dc9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a0dc9-106">Permissions</span></span>
<span data-ttu-id="a0dc9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0dc9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0dc9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a0dc9-109">Permission type</span></span>      | <span data-ttu-id="a0dc9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a0dc9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a0dc9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a0dc9-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="a0dc9-112">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="a0dc9-112">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="a0dc9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a0dc9-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="a0dc9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0dc9-114">Not supported.</span></span>  |
|<span data-ttu-id="a0dc9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a0dc9-115">Application</span></span> | <span data-ttu-id="a0dc9-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0dc9-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 
## <a name="http-request"></a><span data-ttu-id="a0dc9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a0dc9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me
GET /education/users/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a0dc9-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a0dc9-118">Optional query parameters</span></span>
<span data-ttu-id="a0dc9-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a0dc9-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a0dc9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a0dc9-120">Request headers</span></span>
| <span data-ttu-id="a0dc9-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a0dc9-121">Header</span></span>       | <span data-ttu-id="a0dc9-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a0dc9-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a0dc9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a0dc9-123">Authorization</span></span>  | <span data-ttu-id="a0dc9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a0dc9-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a0dc9-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a0dc9-126">Request body</span></span>
<span data-ttu-id="a0dc9-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a0dc9-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="a0dc9-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0dc9-128">Response</span></span>
<span data-ttu-id="a0dc9-129">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [educationUser](../resources/educationuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a0dc9-129">If successful, this method returns a `200 OK` response code and an [educationUser](../resources/educationuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a0dc9-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a0dc9-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a0dc9-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a0dc9-131">Request</span></span>
<span data-ttu-id="a0dc9-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a0dc9-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a0dc9-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a0dc9-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationuser_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/users/{user-id}
```
# <a name="c"></a>[<span data-ttu-id="a0dc9-134">C#</span><span class="sxs-lookup"><span data-stu-id="a0dc9-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationuser-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a0dc9-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a0dc9-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationuser-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a0dc9-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a0dc9-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationuser-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a0dc9-137">Java</span><span class="sxs-lookup"><span data-stu-id="a0dc9-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationuser-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a0dc9-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0dc9-138">Response</span></span>
<span data-ttu-id="a0dc9-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a0dc9-139">The following is an example of the response.</span></span> 

><span data-ttu-id="a0dc9-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a0dc9-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.educationUser",
    "id": "90eedea1-dea1-90ee-a1de-ee90a1deee90",
    "primaryRole": "String",
    "middleName": "String",
    "externalSource": "String",
    "externalSourceDetail": "String",
    "residenceAddress": {
      "@odata.type": "microsoft.graph.physicalAddress"
    },
    "mailingAddress": {
      "@odata.type": "microsoft.graph.physicalAddress"
    },
    "student": {
      "@odata.type": "microsoft.graph.educationStudent"
    },
    "teacher": {
      "@odata.type": "microsoft.graph.educationTeacher"
    },
    "createdBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "accountEnabled": "Boolean",
    "assignedLicenses": [
      {
        "@odata.type": "microsoft.graph.assignedLicense"
      }
    ],
    "assignedPlans": [
      {
        "@odata.type": "microsoft.graph.assignedPlan"
      }
    ],
    "businessPhones": [
      "String"
    ],
    "department": "String",
    "displayName": "String",
    "givenName": "String",
    "mail": "String",
    "mailNickname": "String",
    "mobilePhone": "String",
    "passwordPolicies": "String",
    "passwordProfile": {
      "@odata.type": "microsoft.graph.passwordProfile"
    },
    "officeLocation": "String",
    "preferredLanguage": "String",
    "provisionedPlans": [
      {
        "@odata.type": "microsoft.graph.provisionedPlan"
      }
    ],
    "refreshTokensValidFromDateTime": "String (timestamp)",
    "showInAddressList": "Boolean",
    "surname": "String",
    "usageLocation": "String",
    "userPrincipalName": "String",
    "userType": "String",
    "onPremisesInfo": {
      "@odata.type": "microsoft.graph.educationOnPremisesInfo"
    }
  }
}
```
