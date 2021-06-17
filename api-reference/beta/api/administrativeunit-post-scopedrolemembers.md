---
title: Adicionar um scopedRoleMember
description: 'Adicione um novo scopedRoleMembership. OBSERVAÇÃO: No momento, apenas as *funções* de administrador de conta de usuário e *helpdesk* são suportadas para associações de função com escopo.'
localization_priority: Normal
author: DougKirschner
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 2eb0f3e687e86d9634c28ba4958e895718718625
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52991917"
---
# <a name="add-a-scopedrolemember"></a><span data-ttu-id="e76b4-104">Adicionar um scopedRoleMember</span><span class="sxs-lookup"><span data-stu-id="e76b4-104">Add a scopedRoleMember</span></span>

<span data-ttu-id="e76b4-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e76b4-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e76b4-106">Adicione um novo [scopedRoleMembership](../resources/scopedrolemembership.md).</span><span class="sxs-lookup"><span data-stu-id="e76b4-106">Add a new [scopedRoleMembership](../resources/scopedrolemembership.md).</span></span> <span data-ttu-id="e76b4-107">OBSERVAÇÃO: No momento, apenas as *funções* de administrador de conta de usuário e *helpdesk* são suportadas para associações de função com escopo.</span><span class="sxs-lookup"><span data-stu-id="e76b4-107">NOTE: Only the *User account administrator* and *Helpdesk administrator* roles are currently supported for scoped-role memberships.</span></span>

## <a name="permissions"></a><span data-ttu-id="e76b4-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="e76b4-108">Permissions</span></span>
<span data-ttu-id="e76b4-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e76b4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e76b4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e76b4-111">Permission type</span></span>      | <span data-ttu-id="e76b4-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e76b4-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e76b4-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e76b4-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e76b4-114">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e76b4-114">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e76b4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e76b4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e76b4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e76b4-116">Not supported.</span></span>    |
|<span data-ttu-id="e76b4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e76b4-117">Application</span></span> | <span data-ttu-id="e76b4-118">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="e76b4-118">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="e76b4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e76b4-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits/{id}/scopedRoleMembers
```
## <a name="request-headers"></a><span data-ttu-id="e76b4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e76b4-120">Request headers</span></span>
| <span data-ttu-id="e76b4-121">Nome</span><span class="sxs-lookup"><span data-stu-id="e76b4-121">Name</span></span>      |<span data-ttu-id="e76b4-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e76b4-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e76b4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e76b4-123">Authorization</span></span>  | <span data-ttu-id="e76b4-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e76b4-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e76b4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e76b4-126">Request body</span></span>
<span data-ttu-id="e76b4-127">No corpo da solicitação, fornece uma representação JSON do [objeto scopedRoleMembership.](../resources/scopedrolemembership.md)</span><span class="sxs-lookup"><span data-stu-id="e76b4-127">In the request body, supply a JSON representation of [scopedRoleMembership](../resources/scopedrolemembership.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e76b4-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e76b4-128">Response</span></span>

<span data-ttu-id="e76b4-129">Se tiver êxito, este método retornará `201 Created` o código de resposta e o objeto [scopedRoleMembership](../resources/scopedrolemembership.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e76b4-129">If successful, this method returns `201 Created` response code and [scopedRoleMembership](../resources/scopedrolemembership.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e76b4-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e76b4-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e76b4-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e76b4-131">Request</span></span>
<span data-ttu-id="e76b4-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e76b4-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e76b4-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="e76b4-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_scopedrolemembership_from_administrativeunit"
}-->
```http
POST https://graph.microsoft.com/beta/administrativeUnits/{id}/scopedRoleMembers
Content-type: application/json
Content-length: 272

{
  "roleId": "roleId-value",
  "roleMemberInfo": {
    "id": "id-value"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="e76b4-134">C#</span><span class="sxs-lookup"><span data-stu-id="e76b4-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-scopedrolemembership-from-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e76b4-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e76b4-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-scopedrolemembership-from-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e76b4-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e76b4-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-scopedrolemembership-from-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e76b4-137">Java</span><span class="sxs-lookup"><span data-stu-id="e76b4-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-scopedrolemembership-from-administrativeunit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="e76b4-138">No corpo da solicitação, fornece uma representação JSON do [objeto scopedRoleMembership.](../resources/scopedrolemembership.md)</span><span class="sxs-lookup"><span data-stu-id="e76b4-138">In the request body, supply a JSON representation of [scopedRoleMembership](../resources/scopedrolemembership.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="e76b4-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="e76b4-139">Response</span></span>
<span data-ttu-id="e76b4-p105">Aqui está um exemplo da resposta. Observação: o objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="e76b4-p105">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scopedRoleMembership"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 294

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#scopedRoleMemberships/$entity",
  "administrativeUnitId": "administrativeUnitId-value",
  "roleId": "roleId-value",
  "roleMemberInfo": {
    "id": "id-value",
    "displayName": "displayName-value",
    "userPrincipalName": "userPrincipalName-value"
  },
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create scopedRoleMembership",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


