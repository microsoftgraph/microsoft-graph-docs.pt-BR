---
title: Listar classes
description: 'Recupere uma lista de objetos de classe. Se o token delegado for usado, os membros só poderão ver informações sobre suas próprias aulas. '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: f572c642caffe8c944fc3c81eba4a5fc6a4a37ad
ms.sourcegitcommit: 55e9497c8e003be389f8b5d641f80dae7bf6004b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2020
ms.locfileid: "44909531"
---
# <a name="list-classes"></a><span data-ttu-id="6a176-104">Listar classes</span><span class="sxs-lookup"><span data-stu-id="6a176-104">List classes</span></span>

<span data-ttu-id="6a176-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a176-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a176-106">Recupere uma coleção de recursos educationClass.</span><span class="sxs-lookup"><span data-stu-id="6a176-106">Retrieve a collection of educationClass resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="6a176-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="6a176-107">Permissions</span></span>

<span data-ttu-id="6a176-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="6a176-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="6a176-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a176-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6a176-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6a176-110">Permission type</span></span>                        | <span data-ttu-id="6a176-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6a176-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="6a176-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6a176-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="6a176-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="6a176-113">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="6a176-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6a176-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a176-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a176-115">Not supported.</span></span>                              |
| <span data-ttu-id="6a176-116">Application</span><span class="sxs-lookup"><span data-stu-id="6a176-116">Application</span></span>                            | <span data-ttu-id="6a176-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a176-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="6a176-118">Quando as permissões delegadas são usadas, somente os recursos do educationClass de que o usuário de autenticação é um membro será retornado.</span><span class="sxs-lookup"><span data-stu-id="6a176-118">When delegated permissions are used, only educationClass resources that the authentication user is a member will be returned.</span></span>

## <a name="http-request"></a><span data-ttu-id="6a176-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6a176-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/me/classes
GET /education/users/{id}/classes
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6a176-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6a176-120">Optional query parameters</span></span>

<span data-ttu-id="6a176-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6a176-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6a176-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6a176-122">Request headers</span></span>

| <span data-ttu-id="6a176-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6a176-123">Header</span></span>        | <span data-ttu-id="6a176-124">Valor</span><span class="sxs-lookup"><span data-stu-id="6a176-124">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="6a176-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="6a176-125">Authorization</span></span> | <span data-ttu-id="6a176-126">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="6a176-126">Bearer {token}.</span></span> <span data-ttu-id="6a176-127">Required.</span><span class="sxs-lookup"><span data-stu-id="6a176-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6a176-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6a176-128">Request body</span></span>

<span data-ttu-id="6a176-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6a176-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a176-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a176-130">Response</span></span>

<span data-ttu-id="6a176-131">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6a176-131">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a176-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6a176-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6a176-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6a176-133">Request</span></span>

<span data-ttu-id="6a176-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6a176-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6a176-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="6a176-135">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_classes"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/me/classes
```

# <a name="c"></a>[<span data-ttu-id="6a176-136">C#</span><span class="sxs-lookup"><span data-stu-id="6a176-136">C#</span></span>](#tab/csharp)

[!INCLUDE [sample-code](../includes/snippets/csharp/get-classes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6a176-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6a176-137">JavaScript</span></span>](#tab/javascript)

[!INCLUDE [sample-code](../includes/snippets/javascript/get-classes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6a176-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6a176-138">Objective-C</span></span>](#tab/objc)

[!INCLUDE [sample-code](../includes/snippets/objc/get-classes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6a176-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a176-139">Response</span></span>

<span data-ttu-id="6a176-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6a176-140">The following is an example of the response.</span></span>

> <span data-ttu-id="6a176-141">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="6a176-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="6a176-142">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="6a176-142">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 277

{
  "value": [
    {
      "id": "11019",
      "description": "Health Level 1",
      "classCode": "Health 501",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "displayName": "Health 1",
      "externalId": "11019",
      "externalName": "Health Level 1",
      "externalSource": "sis",
      "mailNickname": "fineartschool.net"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List classes",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
