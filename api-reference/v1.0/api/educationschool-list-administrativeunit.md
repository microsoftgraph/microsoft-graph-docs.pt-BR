---
title: Listar administrativeUnit an educationSchool
description: Obter uma lista de administrativeUnits associado a um objeto educationSchool.
author: mmast
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: a8ca5a51c6fb71c3cab0d6f0a7be239eb2101999
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474845"
---
# <a name="list-administrativeunit-an-educationschool"></a><span data-ttu-id="68f79-103">Listar administrativeUnit an educationSchool</span><span class="sxs-lookup"><span data-stu-id="68f79-103">List administrativeUnit an educationSchool</span></span>

<span data-ttu-id="68f79-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68f79-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="68f79-105">Obter uma lista **de administrativeUnits** associado a um [objeto educationSchool.](../resources/educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="68f79-105">Get a list of **administrativeUnits** associated with an [educationSchool](../resources/educationschool.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="68f79-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="68f79-106">Permissions</span></span>

<span data-ttu-id="68f79-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68f79-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="68f79-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="68f79-109">Permission type</span></span>                        | <span data-ttu-id="68f79-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="68f79-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="68f79-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="68f79-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="68f79-112">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="68f79-112">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="68f79-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="68f79-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68f79-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="68f79-114">Not supported.</span></span>                              |
| <span data-ttu-id="68f79-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="68f79-115">Application</span></span>                            | <span data-ttu-id="68f79-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68f79-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="68f79-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="68f79-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
GET /education/schools/{educationSchoolId}/administrativeUnit
```

## <a name="optional-query-parameters"></a><span data-ttu-id="68f79-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="68f79-118">Optional query parameters</span></span>

<span data-ttu-id="68f79-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="68f79-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="68f79-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="68f79-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="68f79-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="68f79-121">Request headers</span></span>

| <span data-ttu-id="68f79-122">Nome</span><span class="sxs-lookup"><span data-stu-id="68f79-122">Name</span></span>          | <span data-ttu-id="68f79-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="68f79-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="68f79-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="68f79-124">Authorization</span></span> | <span data-ttu-id="68f79-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="68f79-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="68f79-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="68f79-127">Request body</span></span>

<span data-ttu-id="68f79-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="68f79-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="68f79-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="68f79-129">Response</span></span>

<span data-ttu-id="68f79-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [administrativeUnit](../resources/administrativeunit.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="68f79-130">If successful, this method returns a `200 OK` response code and a collection of [administrativeUnit](../resources/administrativeunit.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="68f79-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="68f79-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="68f79-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="68f79-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="68f79-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="68f79-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_administrativeunit"
}
-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes/{educationClassId}/members/{educationUserId}/schools/{educationSchoolId}/administrativeUnit
```
# <a name="c"></a>[<span data-ttu-id="68f79-134">C#</span><span class="sxs-lookup"><span data-stu-id="68f79-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="68f79-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="68f79-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="68f79-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="68f79-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="68f79-137">Java</span><span class="sxs-lookup"><span data-stu-id="68f79-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-administrativeunit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="68f79-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="68f79-138">Response</span></span>

> <span data-ttu-id="68f79-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="68f79-139">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.administrativeUnit)"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.administrativeUnit",
      "id": "03e281d6-81d6-03e2-d681-e203d681e203",
      "deletedDateTime": "String (timestamp)",
      "displayName": "String",
      "description": "String",
      "visibility": "String"
    }
  ]
}
```
