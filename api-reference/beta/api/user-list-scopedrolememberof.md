---
title: Listar scopedAdministratorOf
description: Recupere uma lista de scopedRoleMembership para o usuário.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0303425884d3ae7b622c5e20a7ed1909feb99850
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451767"
---
# <a name="list-scopedadministratorof"></a><span data-ttu-id="d87d3-103">Listar scopedAdministratorOf</span><span class="sxs-lookup"><span data-stu-id="d87d3-103">List scopedAdministratorOf</span></span>

<span data-ttu-id="d87d3-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d87d3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d87d3-105">Recupere uma lista de [scopedRoleMembership](../resources/scopedrolemembership.md) para o usuário.</span><span class="sxs-lookup"><span data-stu-id="d87d3-105">Retrieve a list of [scopedRoleMembership](../resources/scopedrolemembership.md) for the user.</span></span>
## <a name="permissions"></a><span data-ttu-id="d87d3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d87d3-106">Permissions</span></span>
<span data-ttu-id="d87d3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d87d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d87d3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d87d3-109">Permission type</span></span>      | <span data-ttu-id="d87d3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d87d3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d87d3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d87d3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d87d3-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d87d3-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d87d3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d87d3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d87d3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d87d3-114">Not supported.</span></span>    |
|<span data-ttu-id="d87d3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d87d3-115">Application</span></span> | <span data-ttu-id="d87d3-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d87d3-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d87d3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d87d3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/scopedAdministratorOf
GET /users/{id}/scopedAdministratorOf

```
## <a name="optional-query-parameters"></a><span data-ttu-id="d87d3-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d87d3-118">Optional query parameters</span></span>
<span data-ttu-id="d87d3-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d87d3-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d87d3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d87d3-120">Request headers</span></span>
| <span data-ttu-id="d87d3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d87d3-121">Header</span></span>       | <span data-ttu-id="d87d3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d87d3-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d87d3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d87d3-123">Authorization</span></span>  | <span data-ttu-id="d87d3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d87d3-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d87d3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d87d3-126">Request body</span></span>
<span data-ttu-id="d87d3-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d87d3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d87d3-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d87d3-128">Response</span></span>

<span data-ttu-id="d87d3-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [scopedRoleMembership](../resources/scopedrolemembership.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d87d3-129">If successful, this method returns a `200 OK` response code and collection of [scopedRoleMembership](../resources/scopedrolemembership.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d87d3-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d87d3-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d87d3-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d87d3-131">Request</span></span>
<span data-ttu-id="d87d3-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d87d3-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d87d3-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d87d3-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_scopedadministratorof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/scopedAdministratorOf
```
# <a name="c"></a>[<span data-ttu-id="d87d3-134">C#</span><span class="sxs-lookup"><span data-stu-id="d87d3-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-scopedadministratorof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d87d3-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d87d3-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-scopedadministratorof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d87d3-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d87d3-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-scopedadministratorof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d87d3-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="d87d3-137">Response</span></span>
<span data-ttu-id="d87d3-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d87d3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
