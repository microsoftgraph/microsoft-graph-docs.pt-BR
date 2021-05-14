---
title: Obter educationSchool
description: Leia as propriedades e as relações de um objeto educationSchool.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 3ec682a7674bc24eca3d168e3f92b3d3c05f3bda
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474888"
---
# <a name="get-educationschool"></a><span data-ttu-id="45858-103">Obter educationSchool</span><span class="sxs-lookup"><span data-stu-id="45858-103">Get educationSchool</span></span>

<span data-ttu-id="45858-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45858-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="45858-105">Leia as propriedades e as relações de um [objeto educationSchool.](../resources/educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="45858-105">Read the properties and relationships of an [educationSchool](../resources/educationschool.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="45858-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="45858-106">Permissions</span></span>

<span data-ttu-id="45858-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45858-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="45858-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="45858-109">Permission type</span></span>                        | <span data-ttu-id="45858-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="45858-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="45858-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="45858-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="45858-112">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="45858-112">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="45858-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="45858-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45858-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="45858-114">Not supported.</span></span>                              |
| <span data-ttu-id="45858-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="45858-115">Application</span></span>                            | <span data-ttu-id="45858-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45858-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="45858-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="45858-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
GET /education/schools/{educationSchoolId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="45858-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="45858-118">Optional query parameters</span></span>

<span data-ttu-id="45858-119">Este método dá suporte aos mesmos parâmetros de consulta OData que [Get User](../api/user-get.md#optional-query-parameters).</span><span class="sxs-lookup"><span data-stu-id="45858-119">This method supports the same OData query parameters as [Get User](../api/user-get.md#optional-query-parameters).</span></span> <span data-ttu-id="45858-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="45858-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="45858-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="45858-121">Request headers</span></span>

| <span data-ttu-id="45858-122">Nome</span><span class="sxs-lookup"><span data-stu-id="45858-122">Name</span></span>          | <span data-ttu-id="45858-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="45858-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="45858-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="45858-124">Authorization</span></span> | <span data-ttu-id="45858-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="45858-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="45858-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="45858-127">Request body</span></span>

<span data-ttu-id="45858-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="45858-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45858-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="45858-129">Response</span></span>

<span data-ttu-id="45858-130">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [educationSchool](../resources/educationschool.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="45858-130">If successful, this method returns a `200 OK` response code and an [educationSchool](../resources/educationschool.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="45858-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="45858-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="45858-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="45858-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="45858-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="45858-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationschool"
}
-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/schools/{educationSchoolId}
```
# <a name="c"></a>[<span data-ttu-id="45858-134">C#</span><span class="sxs-lookup"><span data-stu-id="45858-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="45858-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="45858-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="45858-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="45858-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="45858-137">Java</span><span class="sxs-lookup"><span data-stu-id="45858-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationschool-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="45858-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="45858-138">Response</span></span>

><span data-ttu-id="45858-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="45858-139">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.educationSchool",
    "id": "1c23c12e-c12e-1c23-2ec1-231c2ec1231c",
    "displayName": "String",
    "description": "String",
    "externalSource": "String",
    "externalSourceDetail": "String",
    "principalEmail": "String",
    "principalName": "String",
    "externalPrincipalId": "String",
    "lowestGrade": "String",
    "highestGrade": "String",
    "schoolNumber": "String",
    "externalId": "String",
    "phone": "String",
    "fax": "String",
    "createdBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "address": {
      "@odata.type": "microsoft.graph.physicalAddress"
    }
  }
}
```
