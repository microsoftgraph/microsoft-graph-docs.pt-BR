---
title: Listar groupLifecyclePolicies
description: Recupera uma lista de objetos groupLifecyclePolicy à qual um grupo pertence.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 23ac6af1f01f24613f91a3a8f00d922f9f5741ec
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36014881"
---
# <a name="list-grouplifecyclepolicies"></a><span data-ttu-id="754da-103">Listar groupLifecyclePolicies</span><span class="sxs-lookup"><span data-stu-id="754da-103">List groupLifecyclePolicies</span></span>

<span data-ttu-id="754da-104">Recupera uma lista de objetos [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) à qual um grupo pertence.</span><span class="sxs-lookup"><span data-stu-id="754da-104">Retrieves a list of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects to which a group belongs.</span></span>

## <a name="permissions"></a><span data-ttu-id="754da-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="754da-105">Permissions</span></span>

<span data-ttu-id="754da-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="754da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="754da-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="754da-108">Permission type</span></span>      | <span data-ttu-id="754da-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="754da-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="754da-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="754da-110">Delegated (work or school account)</span></span> | <span data-ttu-id="754da-111">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="754da-111">Directory.Read.All, Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="754da-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="754da-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="754da-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="754da-113">Not supported.</span></span>    |
|<span data-ttu-id="754da-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="754da-114">Application</span></span> | <span data-ttu-id="754da-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="754da-115">Directory.Read.All, Directory.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="754da-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="754da-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/groupLifecyclePolicies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="754da-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="754da-117">Optional query parameters</span></span>
<span data-ttu-id="754da-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="754da-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="754da-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="754da-119">Request headers</span></span>
| <span data-ttu-id="754da-120">Nome</span><span class="sxs-lookup"><span data-stu-id="754da-120">Name</span></span> | <span data-ttu-id="754da-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="754da-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="754da-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="754da-122">Authorization</span></span> | <span data-ttu-id="754da-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="754da-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="754da-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="754da-125">Request body</span></span>
<span data-ttu-id="754da-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="754da-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="754da-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="754da-127">Response</span></span>
<span data-ttu-id="754da-128">Quando é bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="754da-128">If successful, this method returns a `200 OK` response code and collection of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="754da-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="754da-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="754da-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="754da-130">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="754da-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="754da-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicies"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/groupLifecyclePolicies
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="754da-132">C#</span><span class="sxs-lookup"><span data-stu-id="754da-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-grouplifecyclepolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="754da-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="754da-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-grouplifecyclepolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="754da-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="754da-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-grouplifecyclepolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="754da-135">Java</span><span class="sxs-lookup"><span data-stu-id="754da-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-grouplifecyclepolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="754da-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="754da-136">Response</span></span>

<span data-ttu-id="754da-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="754da-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 222

{
  "value": [
    {
      "id": "ffffffff-ffff-ffff-ffff-ffffffffffff",
      "groupLifetimeInDays": 90,
      "managedGroupTypes": "Selected",
      "alternateNotificationEmails": "admin@contoso.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groupLifecyclePolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
