---
title: Adicionar um scopedRoleMember
description: 'Adicione um novo scopedRoleMembership. Observação: somente as funções de administrador de *conta de usuário* e *administrador de helpdesk* têm suporte para associações com escopo de função.'
localization_priority: Normal
author: anandyadavMSFT
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2888e50142a77d5f669e9090aecf6b50aeaeb02e
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2020
ms.locfileid: "43123325"
---
# <a name="add-a-scopedrolemember"></a><span data-ttu-id="c189e-104">Adicionar um scopedRoleMember</span><span class="sxs-lookup"><span data-stu-id="c189e-104">Add a scopedRoleMember</span></span>

<span data-ttu-id="c189e-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c189e-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c189e-106">Adicione um novo [scopedRoleMembership](../resources/scopedrolemembership.md).</span><span class="sxs-lookup"><span data-stu-id="c189e-106">Add a new [scopedRoleMembership](../resources/scopedrolemembership.md).</span></span> <span data-ttu-id="c189e-107">Observação: somente as funções de administrador de *conta de usuário* e *administrador de helpdesk* têm suporte para associações com escopo de função.</span><span class="sxs-lookup"><span data-stu-id="c189e-107">NOTE: Only the *User account administrator* and *Helpdesk administrator* roles are currently supported for scoped-role memberships.</span></span>

## <a name="permissions"></a><span data-ttu-id="c189e-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="c189e-108">Permissions</span></span>
<span data-ttu-id="c189e-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c189e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c189e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c189e-111">Permission type</span></span>      | <span data-ttu-id="c189e-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c189e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c189e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c189e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c189e-114">RoleManagement. ReadWrite. Directory, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="c189e-114">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c189e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c189e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c189e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c189e-116">Not supported.</span></span>    |
|<span data-ttu-id="c189e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c189e-117">Application</span></span> | <span data-ttu-id="c189e-118">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="c189e-118">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="c189e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c189e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits/{id}/scopedRoleMembers
```
## <a name="request-headers"></a><span data-ttu-id="c189e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c189e-120">Request headers</span></span>
| <span data-ttu-id="c189e-121">Nome</span><span class="sxs-lookup"><span data-stu-id="c189e-121">Name</span></span>      |<span data-ttu-id="c189e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c189e-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c189e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c189e-123">Authorization</span></span>  | <span data-ttu-id="c189e-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c189e-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c189e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c189e-126">Request body</span></span>
<span data-ttu-id="c189e-127">No corpo da solicitação, forneça uma representação JSON do objeto [scopedRoleMembership](../resources/scopedrolemembership.md) .</span><span class="sxs-lookup"><span data-stu-id="c189e-127">In the request body, supply a JSON representation of [scopedRoleMembership](../resources/scopedrolemembership.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c189e-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c189e-128">Response</span></span>

<span data-ttu-id="c189e-129">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [scopedRoleMembership](../resources/scopedrolemembership.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c189e-129">If successful, this method returns `201 Created` response code and [scopedRoleMembership](../resources/scopedrolemembership.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c189e-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c189e-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c189e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c189e-131">Request</span></span>
<span data-ttu-id="c189e-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c189e-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c189e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c189e-133">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c189e-134">C#</span><span class="sxs-lookup"><span data-stu-id="c189e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-scopedrolemembership-from-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c189e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c189e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-scopedrolemembership-from-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c189e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c189e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-scopedrolemembership-from-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="c189e-137">No corpo da solicitação, forneça uma representação JSON do objeto [scopedRoleMembership](../resources/scopedrolemembership.md) .</span><span class="sxs-lookup"><span data-stu-id="c189e-137">In the request body, supply a JSON representation of [scopedRoleMembership](../resources/scopedrolemembership.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="c189e-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="c189e-138">Response</span></span>
<span data-ttu-id="c189e-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c189e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
