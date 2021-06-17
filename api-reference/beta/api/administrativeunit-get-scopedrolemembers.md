---
title: Obter um scopedRoleMember
description: Recupere um recurso scopedRoleMembership específico.
author: DougKirschner
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: c2673dfae71faff2b484221b427f2841e36f1dbe
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992006"
---
# <a name="get-a-scopedrolemember"></a><span data-ttu-id="b9dac-103">Obter um scopedRoleMember</span><span class="sxs-lookup"><span data-stu-id="b9dac-103">Get a scopedRoleMember</span></span>

<span data-ttu-id="b9dac-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9dac-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9dac-105">Recupere um recurso [scopedRoleMembership](../resources/scopedrolemembership.md) específico.</span><span class="sxs-lookup"><span data-stu-id="b9dac-105">Retrieve a specific [scopedRoleMembership](../resources/scopedrolemembership.md) resource.</span></span>
## <a name="permissions"></a><span data-ttu-id="b9dac-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="b9dac-106">Permissions</span></span>
<span data-ttu-id="b9dac-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9dac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b9dac-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b9dac-109">Permission type</span></span>      | <span data-ttu-id="b9dac-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b9dac-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9dac-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b9dac-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b9dac-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b9dac-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b9dac-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b9dac-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9dac-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9dac-114">Not supported.</span></span>    |
|<span data-ttu-id="b9dac-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b9dac-115">Application</span></span> | <span data-ttu-id="b9dac-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9dac-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9dac-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b9dac-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits/{id}/scopedRoleMembers/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b9dac-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b9dac-118">Optional query parameters</span></span>
<span data-ttu-id="b9dac-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b9dac-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b9dac-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b9dac-120">Request headers</span></span>
| <span data-ttu-id="b9dac-121">Nome</span><span class="sxs-lookup"><span data-stu-id="b9dac-121">Name</span></span>      |<span data-ttu-id="b9dac-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9dac-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b9dac-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b9dac-123">Authorization</span></span>  | <span data-ttu-id="b9dac-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b9dac-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b9dac-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b9dac-126">Request body</span></span>
<span data-ttu-id="b9dac-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b9dac-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9dac-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9dac-128">Response</span></span>

<span data-ttu-id="b9dac-129">Se tiver êxito, este método retornará um código de `200 OK` resposta e o objeto [scopedRoleMembership](../resources/scopedrolemembership.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b9dac-129">If successful, this method returns a `200 OK` response code and the requested [scopedRoleMembership](../resources/scopedrolemembership.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b9dac-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b9dac-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b9dac-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b9dac-131">Request</span></span>
<span data-ttu-id="b9dac-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b9dac-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b9dac-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="b9dac-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_scopedrolemember_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/scopedRoleMembers/{id}
```
# <a name="c"></a>[<span data-ttu-id="b9dac-134">C#</span><span class="sxs-lookup"><span data-stu-id="b9dac-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-scopedrolemember-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b9dac-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b9dac-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-scopedrolemember-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b9dac-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b9dac-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-scopedrolemember-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b9dac-137">Java</span><span class="sxs-lookup"><span data-stu-id="b9dac-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-scopedrolemember-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b9dac-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9dac-138">Response</span></span>
<span data-ttu-id="b9dac-p103">Aqui está um exemplo da resposta. Observação: o objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="b9dac-p103">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
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
