---
title: Listar scopedAdministratorOf
description: Recupere uma lista de scopedRoleMembership para o usuário.
author: jpettere
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 1de486edef0764b528491ed63bd5fd01d2e94895
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721492"
---
# <a name="list-scopedadministratorof"></a><span data-ttu-id="d1797-103">Listar scopedAdministratorOf</span><span class="sxs-lookup"><span data-stu-id="d1797-103">List scopedAdministratorOf</span></span>

<span data-ttu-id="d1797-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1797-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1797-105">Recupere uma lista de [scopedRoleMembership](../resources/scopedrolemembership.md) para o usuário.</span><span class="sxs-lookup"><span data-stu-id="d1797-105">Retrieve a list of [scopedRoleMembership](../resources/scopedrolemembership.md) for the user.</span></span>
## <a name="permissions"></a><span data-ttu-id="d1797-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d1797-106">Permissions</span></span>
<span data-ttu-id="d1797-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1797-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d1797-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d1797-109">Permission type</span></span>      | <span data-ttu-id="d1797-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d1797-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d1797-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d1797-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d1797-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d1797-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d1797-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d1797-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1797-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d1797-114">Not supported.</span></span>    |
|<span data-ttu-id="d1797-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d1797-115">Application</span></span> | <span data-ttu-id="d1797-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1797-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d1797-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d1797-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/scopedRoleMemberOf 
GET /users/{id}/scopedRoleMemberOf

```
## <a name="optional-query-parameters"></a><span data-ttu-id="d1797-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d1797-118">Optional query parameters</span></span>
<span data-ttu-id="d1797-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d1797-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d1797-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d1797-120">Request headers</span></span>
| <span data-ttu-id="d1797-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d1797-121">Header</span></span>       | <span data-ttu-id="d1797-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d1797-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d1797-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d1797-123">Authorization</span></span>  | <span data-ttu-id="d1797-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d1797-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d1797-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d1797-126">Request body</span></span>
<span data-ttu-id="d1797-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d1797-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1797-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1797-128">Response</span></span>

<span data-ttu-id="d1797-129">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos scopedRoleMembership](../resources/scopedrolemembership.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d1797-129">If successful, this method returns a `200 OK` response code and collection of [scopedRoleMembership](../resources/scopedrolemembership.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d1797-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d1797-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d1797-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d1797-131">Request</span></span>
<span data-ttu-id="d1797-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d1797-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d1797-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d1797-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_scopedadministratorof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/scopedRoleMemberOf
```
# <a name="c"></a>[<span data-ttu-id="d1797-134">C#</span><span class="sxs-lookup"><span data-stu-id="d1797-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-scopedadministratorof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d1797-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d1797-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-scopedadministratorof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d1797-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d1797-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-scopedadministratorof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d1797-137">Java</span><span class="sxs-lookup"><span data-stu-id="d1797-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-scopedadministratorof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d1797-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1797-138">Response</span></span>
<span data-ttu-id="d1797-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d1797-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
