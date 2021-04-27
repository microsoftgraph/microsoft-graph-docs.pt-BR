---
title: Obter um scopedRoleMember
description: Recupere um recurso scopedRoleMembership específico.
author: anandyadavMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 606f76952aedea22a9eb240f4a620ac930b15ad2
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048264"
---
# <a name="get-a-scopedrolemember"></a><span data-ttu-id="03332-103">Obter um scopedRoleMember</span><span class="sxs-lookup"><span data-stu-id="03332-103">Get a scopedRoleMember</span></span>

<span data-ttu-id="03332-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03332-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03332-105">Recupere um recurso [scopedRoleMembership](../resources/scopedrolemembership.md) específico.</span><span class="sxs-lookup"><span data-stu-id="03332-105">Retrieve a specific [scopedRoleMembership](../resources/scopedrolemembership.md) resource.</span></span>
## <a name="permissions"></a><span data-ttu-id="03332-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="03332-106">Permissions</span></span>
<span data-ttu-id="03332-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03332-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="03332-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="03332-109">Permission type</span></span>      | <span data-ttu-id="03332-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="03332-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="03332-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="03332-111">Delegated (work or school account)</span></span> | <span data-ttu-id="03332-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="03332-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="03332-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="03332-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03332-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="03332-114">Not supported.</span></span>    |
|<span data-ttu-id="03332-115">Application</span><span class="sxs-lookup"><span data-stu-id="03332-115">Application</span></span> | <span data-ttu-id="03332-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03332-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="03332-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="03332-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits/{id}/scopedRoleMembers/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="03332-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="03332-118">Optional query parameters</span></span>
<span data-ttu-id="03332-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="03332-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="03332-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="03332-120">Request headers</span></span>
| <span data-ttu-id="03332-121">Nome</span><span class="sxs-lookup"><span data-stu-id="03332-121">Name</span></span>      |<span data-ttu-id="03332-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="03332-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="03332-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="03332-123">Authorization</span></span>  | <span data-ttu-id="03332-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="03332-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="03332-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="03332-126">Request body</span></span>
<span data-ttu-id="03332-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="03332-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="03332-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="03332-128">Response</span></span>

<span data-ttu-id="03332-129">Se tiver êxito, este método retornará um código de `200 OK` resposta e o objeto [scopedRoleMembership](../resources/scopedrolemembership.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="03332-129">If successful, this method returns a `200 OK` response code and the requested [scopedRoleMembership](../resources/scopedrolemembership.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="03332-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="03332-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="03332-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="03332-131">Request</span></span>
<span data-ttu-id="03332-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="03332-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="03332-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="03332-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_scopedrolemember_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/scopedRoleMembers/{id}
```
# <a name="c"></a>[<span data-ttu-id="03332-134">C#</span><span class="sxs-lookup"><span data-stu-id="03332-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-scopedrolemember-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="03332-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="03332-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-scopedrolemember-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="03332-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="03332-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-scopedrolemember-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="03332-137">Java</span><span class="sxs-lookup"><span data-stu-id="03332-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-scopedrolemember-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="03332-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="03332-138">Response</span></span>
<span data-ttu-id="03332-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="03332-139">Here is an example of the response.</span></span> <span data-ttu-id="03332-140">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="03332-140">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scopedRoleMembership"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 307

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
