---
title: Listar groupLifecyclePolicies
description: Recupera uma lista de objetos groupLifecyclePolicy à qual um grupo pertence.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 9b538b2b47a41e2d17b83253939f9f31c52b3712
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48459638"
---
# <a name="list-grouplifecyclepolicies"></a><span data-ttu-id="0282d-103">Listar groupLifecyclePolicies</span><span class="sxs-lookup"><span data-stu-id="0282d-103">List groupLifecyclePolicies</span></span>

<span data-ttu-id="0282d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0282d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0282d-105">Recupera uma lista de objetos [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) à qual um grupo pertence.</span><span class="sxs-lookup"><span data-stu-id="0282d-105">Retrieves a list of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects to which a group belongs.</span></span>

## <a name="permissions"></a><span data-ttu-id="0282d-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="0282d-106">Permissions</span></span>

<span data-ttu-id="0282d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0282d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0282d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0282d-109">Permission type</span></span>      | <span data-ttu-id="0282d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0282d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0282d-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0282d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0282d-112">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0282d-112">Directory.Read.All, Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="0282d-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0282d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0282d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0282d-114">Not supported.</span></span>    |
|<span data-ttu-id="0282d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0282d-115">Application</span></span> | <span data-ttu-id="0282d-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0282d-116">Directory.Read.All, Directory.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0282d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0282d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/groupLifecyclePolicies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0282d-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0282d-118">Optional query parameters</span></span>
<span data-ttu-id="0282d-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0282d-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0282d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0282d-120">Request headers</span></span>
| <span data-ttu-id="0282d-121">Nome</span><span class="sxs-lookup"><span data-stu-id="0282d-121">Name</span></span> | <span data-ttu-id="0282d-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="0282d-122">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="0282d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0282d-123">Authorization</span></span> | <span data-ttu-id="0282d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0282d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0282d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0282d-126">Request body</span></span>
<span data-ttu-id="0282d-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0282d-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="0282d-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="0282d-128">Response</span></span>
<span data-ttu-id="0282d-129">Quando é bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0282d-129">If successful, this method returns a `200 OK` response code and collection of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0282d-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0282d-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0282d-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0282d-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="0282d-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="0282d-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicies"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/groupLifecyclePolicies
```
# <a name="c"></a>[<span data-ttu-id="0282d-133">C#</span><span class="sxs-lookup"><span data-stu-id="0282d-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-grouplifecyclepolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0282d-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0282d-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-grouplifecyclepolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0282d-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0282d-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-grouplifecyclepolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0282d-136">Java</span><span class="sxs-lookup"><span data-stu-id="0282d-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-grouplifecyclepolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0282d-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="0282d-137">Response</span></span>

<span data-ttu-id="0282d-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0282d-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
