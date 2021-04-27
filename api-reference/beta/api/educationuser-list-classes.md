---
title: Listar classes
description: 'Recupere uma lista de objetos de classe. Se o token delegado for usado, os membros só poderão ver informações sobre suas próprias aulas. '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: ec0bcde1e53e3dfe801a4cdafbf49572b4c812b8
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52042829"
---
# <a name="list-classes"></a><span data-ttu-id="dca5c-104">Listar classes</span><span class="sxs-lookup"><span data-stu-id="dca5c-104">List classes</span></span>

<span data-ttu-id="dca5c-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dca5c-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dca5c-106">Recupere uma coleção de recursos educationClass.</span><span class="sxs-lookup"><span data-stu-id="dca5c-106">Retrieve a collection of educationClass resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="dca5c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="dca5c-107">Permissions</span></span>

<span data-ttu-id="dca5c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dca5c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dca5c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dca5c-110">Permission type</span></span>                        | <span data-ttu-id="dca5c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dca5c-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="dca5c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dca5c-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="dca5c-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="dca5c-113">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="dca5c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dca5c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dca5c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dca5c-115">Not supported.</span></span>                              |
| <span data-ttu-id="dca5c-116">Application</span><span class="sxs-lookup"><span data-stu-id="dca5c-116">Application</span></span>                            | <span data-ttu-id="dca5c-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dca5c-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="dca5c-118">Quando as permissões delegadas são usadas, somente os recursos educationClass que o usuário de autenticação é membro serão retornados.</span><span class="sxs-lookup"><span data-stu-id="dca5c-118">When delegated permissions are used, only educationClass resources that the authentication user is a member will be returned.</span></span>

## <a name="http-request"></a><span data-ttu-id="dca5c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dca5c-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/me/classes
GET /education/users/{id}/classes
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dca5c-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="dca5c-120">Optional query parameters</span></span>

<span data-ttu-id="dca5c-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="dca5c-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dca5c-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dca5c-122">Request headers</span></span>

| <span data-ttu-id="dca5c-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dca5c-123">Header</span></span>        | <span data-ttu-id="dca5c-124">Valor</span><span class="sxs-lookup"><span data-stu-id="dca5c-124">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="dca5c-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="dca5c-125">Authorization</span></span> | <span data-ttu-id="dca5c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dca5c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dca5c-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dca5c-128">Request body</span></span>

<span data-ttu-id="dca5c-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dca5c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dca5c-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="dca5c-130">Response</span></span>

<span data-ttu-id="dca5c-131">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dca5c-131">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dca5c-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dca5c-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="dca5c-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dca5c-133">Request</span></span>

<span data-ttu-id="dca5c-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dca5c-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dca5c-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="dca5c-135">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_classes_3"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/me/classes
```

# <a name="c"></a>[<span data-ttu-id="dca5c-136">C#</span><span class="sxs-lookup"><span data-stu-id="dca5c-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-classes-3-csharp-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/csharp/get-classes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dca5c-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dca5c-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-classes-3-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/get-classes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dca5c-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dca5c-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-classes-3-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/get-classes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dca5c-139">Java</span><span class="sxs-lookup"><span data-stu-id="dca5c-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-classes-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="dca5c-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="dca5c-140">Response</span></span>

<span data-ttu-id="dca5c-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dca5c-141">The following is an example of the response.</span></span>

> <span data-ttu-id="dca5c-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="dca5c-142">**Note:** The response object shown here might be shortened for readability.</span></span>

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
