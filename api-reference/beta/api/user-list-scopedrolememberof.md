---
title: Listar scopedAdministratorOf
description: Recupere uma lista de scopedRoleMembership para o usuário.
author: jpettere
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 0686e0a6b8ac6bec26a2f30d8e52e59b52f3a192
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051701"
---
# <a name="list-scopedadministratorof"></a><span data-ttu-id="2f211-103">Listar scopedAdministratorOf</span><span class="sxs-lookup"><span data-stu-id="2f211-103">List scopedAdministratorOf</span></span>

<span data-ttu-id="2f211-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f211-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f211-105">Recupere uma lista de [scopedRoleMembership](../resources/scopedrolemembership.md) para o usuário.</span><span class="sxs-lookup"><span data-stu-id="2f211-105">Retrieve a list of [scopedRoleMembership](../resources/scopedrolemembership.md) for the user.</span></span>
## <a name="permissions"></a><span data-ttu-id="2f211-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2f211-106">Permissions</span></span>
<span data-ttu-id="2f211-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f211-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2f211-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2f211-109">Permission type</span></span>      | <span data-ttu-id="2f211-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2f211-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2f211-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2f211-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2f211-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2f211-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2f211-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2f211-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f211-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f211-114">Not supported.</span></span>    |
|<span data-ttu-id="2f211-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2f211-115">Application</span></span> | <span data-ttu-id="2f211-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f211-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2f211-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2f211-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/scopedRoleMemberOf 
GET /users/{id}/scopedRoleMemberOf

```
## <a name="optional-query-parameters"></a><span data-ttu-id="2f211-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2f211-118">Optional query parameters</span></span>
<span data-ttu-id="2f211-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2f211-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2f211-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2f211-120">Request headers</span></span>
| <span data-ttu-id="2f211-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2f211-121">Header</span></span>       | <span data-ttu-id="2f211-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2f211-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2f211-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2f211-123">Authorization</span></span>  | <span data-ttu-id="2f211-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2f211-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2f211-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2f211-126">Request body</span></span>
<span data-ttu-id="2f211-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2f211-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2f211-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f211-128">Response</span></span>

<span data-ttu-id="2f211-129">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos scopedRoleMembership](../resources/scopedrolemembership.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2f211-129">If successful, this method returns a `200 OK` response code and collection of [scopedRoleMembership](../resources/scopedrolemembership.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2f211-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2f211-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2f211-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f211-131">Request</span></span>
<span data-ttu-id="2f211-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f211-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2f211-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="2f211-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_scopedadministratorof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/scopedRoleMemberOf
```
# <a name="c"></a>[<span data-ttu-id="2f211-134">C#</span><span class="sxs-lookup"><span data-stu-id="2f211-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-scopedadministratorof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2f211-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2f211-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-scopedadministratorof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2f211-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2f211-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-scopedadministratorof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2f211-137">Java</span><span class="sxs-lookup"><span data-stu-id="2f211-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-scopedadministratorof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2f211-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f211-138">Response</span></span>
<span data-ttu-id="2f211-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2f211-139">Here is an example of the response.</span></span> <span data-ttu-id="2f211-140">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2f211-140">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scopedRoleMembership",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 307

{
  "value": [
    {
      "roleId": "roleId-value",
      "administrativeUnitId": "administrativeUnitId-value",
      "roleMemberInfo": {
        "id": "id-value",
        "displayName": "displayName-value",
        "userPrincipalName": "userPrincipalName-value"
      },
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List scopedAdministratorOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
