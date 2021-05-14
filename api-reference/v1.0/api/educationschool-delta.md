---
title: 'educationSchool: delta'
description: Get newly created or updated schools without having to perform a full read of the entire school collection.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 5f77334e3149dd963a0a2092faae5aa11bd8bd9a
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474915"
---
# <a name="educationschool-delta"></a><span data-ttu-id="9c071-103">educationSchool: delta</span><span class="sxs-lookup"><span data-stu-id="9c071-103">educationSchool: delta</span></span>

<span data-ttu-id="9c071-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c071-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9c071-105">Get newly created or updated schools without having to perform a full read of the entire school collection.</span><span class="sxs-lookup"><span data-stu-id="9c071-105">Get newly created or updated schools without having to perform a full read of the entire school collection.</span></span> <span data-ttu-id="9c071-106">Consulte [Usar consulta delta para](/graph/delta-query-overview) obter detalhes.</span><span class="sxs-lookup"><span data-stu-id="9c071-106">See [Use delta query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="9c071-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="9c071-107">Permissions</span></span>

<span data-ttu-id="9c071-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c071-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9c071-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9c071-110">Permission type</span></span>                        | <span data-ttu-id="9c071-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9c071-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="9c071-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9c071-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="9c071-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="9c071-113">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="9c071-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9c071-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c071-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9c071-115">Not supported.</span></span>                              |
| <span data-ttu-id="9c071-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9c071-116">Application</span></span>                            | <span data-ttu-id="9c071-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c071-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9c071-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9c071-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
GET /education/schools/delta
```

## <a name="request-headers"></a><span data-ttu-id="9c071-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9c071-119">Request headers</span></span>

| <span data-ttu-id="9c071-120">Nome</span><span class="sxs-lookup"><span data-stu-id="9c071-120">Name</span></span>          | <span data-ttu-id="9c071-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c071-121">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="9c071-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9c071-122">Authorization</span></span> | <span data-ttu-id="9c071-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9c071-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9c071-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9c071-125">Request body</span></span>

<span data-ttu-id="9c071-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9c071-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9c071-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c071-127">Response</span></span>

<span data-ttu-id="9c071-128">Se tiver êxito, essa função retornará um código `200 OK` de resposta e uma coleção [educationSchool](../resources/educationschool.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9c071-128">If successful, this function returns a `200 OK` response code and a [educationSchool](../resources/educationschool.md) collection in the response body.</span></span> <span data-ttu-id="9c071-129">A resposta também inclui uma URL `nextLink` ou `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="9c071-129">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="9c071-130">Se uma URL `nextLink` é retornada, existem páginas de dado adicionais a serem recuperadas na sessão.</span><span class="sxs-lookup"><span data-stu-id="9c071-130">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="9c071-131">O aplicativo continua fazendo solicitações usando a URL `nextLink` até uma URL `deltaLink` ser incluída na resposta.</span><span class="sxs-lookup"><span data-stu-id="9c071-131">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
- <span data-ttu-id="9c071-132">Se uma URL `deltaLink` é retornada, não há mais nenhum dado sobre o estado do recurso a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="9c071-132">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="9c071-133">Persista e use `deltaLink` a URL para saber mais sobre as alterações no recurso no futuro.</span><span class="sxs-lookup"><span data-stu-id="9c071-133">Persist and use the `deltaLink` URL to learn about changes to the resource in the future.</span></span>

<span data-ttu-id="9c071-134">Para obter detalhes, consulte [Using delta query](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="9c071-134">For details, see [Using delta query](/graph/delta-query-overview).</span></span> <span data-ttu-id="9c071-135">Por exemplo, solicitações, [consulte Obter alterações incrementais para usuários](/graph/delta-query-users).</span><span class="sxs-lookup"><span data-stu-id="9c071-135">For example requests, see [Get incremental changes for users](/graph/delta-query-users).</span></span>

## <a name="examples"></a><span data-ttu-id="9c071-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9c071-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9c071-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9c071-137">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="9c071-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="9c071-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationschool_delta"
}
-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/schools/delta
```
# <a name="c"></a>[<span data-ttu-id="9c071-139">C#</span><span class="sxs-lookup"><span data-stu-id="9c071-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationschool-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9c071-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9c071-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationschool-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9c071-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9c071-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationschool-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9c071-142">Java</span><span class="sxs-lookup"><span data-stu-id="9c071-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationschool-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9c071-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c071-143">Response</span></span>

> <span data-ttu-id="9c071-144">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9c071-144">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.educationSchool)"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(educationSchool)",
  "@odata.nextLink": "https://graph.microsoft.com/v1.0/education/schools/delta?$skiptoken=VwhMSQw1l1O5v2F1ZPm...",
  "value": [
    {
      "@odata.type": "#microsoft.graph.educationSchool",
      "id": "String (identifier)",
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
  ]
}
```
