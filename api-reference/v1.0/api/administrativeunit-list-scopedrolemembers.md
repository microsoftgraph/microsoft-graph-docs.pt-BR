---
title: Listar scopedRoleMembers
description: Recupere uma lista de recursos scopedRoleMembership.
author: anandyadavMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: ea7e032f89ef4c2a04db1d8c4beab15ef757d117
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050630"
---
# <a name="list-scopedrolemembers"></a><span data-ttu-id="31fa1-103">Listar scopedRoleMembers</span><span class="sxs-lookup"><span data-stu-id="31fa1-103">List scopedRoleMembers</span></span>

<span data-ttu-id="31fa1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31fa1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="31fa1-105">Recupere uma lista de [recursos scopedRoleMembership.](../resources/scopedrolemembership.md)</span><span class="sxs-lookup"><span data-stu-id="31fa1-105">Retrieve a list of [scopedRoleMembership](../resources/scopedrolemembership.md) resources.</span></span>
## <a name="permissions"></a><span data-ttu-id="31fa1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="31fa1-106">Permissions</span></span>
<span data-ttu-id="31fa1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31fa1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="31fa1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="31fa1-109">Permission type</span></span>      | <span data-ttu-id="31fa1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="31fa1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="31fa1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="31fa1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="31fa1-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="31fa1-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="31fa1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="31fa1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31fa1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="31fa1-114">Not supported.</span></span>    |
|<span data-ttu-id="31fa1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="31fa1-115">Application</span></span> | <span data-ttu-id="31fa1-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31fa1-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="31fa1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="31fa1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directory/administrativeUnits/{id}/scopedRoleMembers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="31fa1-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="31fa1-118">Optional query parameters</span></span>
<span data-ttu-id="31fa1-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="31fa1-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="31fa1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="31fa1-120">Request headers</span></span>
| <span data-ttu-id="31fa1-121">Nome</span><span class="sxs-lookup"><span data-stu-id="31fa1-121">Name</span></span>      |<span data-ttu-id="31fa1-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="31fa1-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="31fa1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="31fa1-123">Authorization</span></span>  | <span data-ttu-id="31fa1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="31fa1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="31fa1-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="31fa1-126">Request body</span></span>
<span data-ttu-id="31fa1-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="31fa1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="31fa1-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="31fa1-128">Response</span></span>

<span data-ttu-id="31fa1-129">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos scopedRoleMembership](../resources/scopedrolemembership.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="31fa1-129">If successful, this method returns a `200 OK` response code and collection of [scopedRoleMembership](../resources/scopedrolemembership.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="31fa1-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="31fa1-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="31fa1-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="31fa1-131">Request</span></span>
<span data-ttu-id="31fa1-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="31fa1-132">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="31fa1-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="31fa1-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_scopedrolemember_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directory/administrativeUnits/{id}/scopedRoleMembers
```
# <a name="c"></a>[<span data-ttu-id="31fa1-134">C#</span><span class="sxs-lookup"><span data-stu-id="31fa1-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-scopedrolemember-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="31fa1-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="31fa1-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-scopedrolemember-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="31fa1-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="31fa1-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-scopedrolemember-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="31fa1-137">Java</span><span class="sxs-lookup"><span data-stu-id="31fa1-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-scopedrolemember-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

##### <a name="response"></a><span data-ttu-id="31fa1-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="31fa1-138">Response</span></span>
<span data-ttu-id="31fa1-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="31fa1-139">Here is an example of the response.</span></span> <span data-ttu-id="31fa1-140">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="31fa1-140">Note: The response object shown here might be shortened for readability.</span></span>
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
      "id": "id-value",
      "roleId": "roleId-value",
      "administrativeUnitId": "administrativeUnitId-value",
      "roleMemberInfo": {
        "id": "id-value",
        "displayName": "displayName-value",
        "userPrincipalName": "userPrincipalName-value"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List scopedRoleMembers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
