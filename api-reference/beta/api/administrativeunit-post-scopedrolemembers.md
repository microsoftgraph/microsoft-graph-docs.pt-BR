---
title: Adicionar um scopedRoleMember
description: 'Adicione um novo scopedRoleMembership. Observação: somente as funções de administrador de *conta de usuário* e *administrador de helpdesk* têm suporte para associações com escopo de função.'
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6fe72ec5158eb055b6f4309089aa8dc0327571a7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441701"
---
# <a name="add-a-scopedrolemember"></a><span data-ttu-id="21454-104">Adicionar um scopedRoleMember</span><span class="sxs-lookup"><span data-stu-id="21454-104">Add a scopedRoleMember</span></span>

<span data-ttu-id="21454-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="21454-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21454-106">Adicione um novo [scopedRoleMembership](../resources/scopedrolemembership.md).</span><span class="sxs-lookup"><span data-stu-id="21454-106">Add a new [scopedRoleMembership](../resources/scopedrolemembership.md).</span></span> <span data-ttu-id="21454-107">Observação: somente as funções de administrador de *conta de usuário* e *administrador de helpdesk* têm suporte para associações com escopo de função.</span><span class="sxs-lookup"><span data-stu-id="21454-107">NOTE: Only the *User account administrator* and *Helpdesk administrator* roles are currently supported for scoped-role memberships.</span></span>

## <a name="permissions"></a><span data-ttu-id="21454-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="21454-108">Permissions</span></span>
<span data-ttu-id="21454-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21454-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="21454-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="21454-111">Permission type</span></span>      | <span data-ttu-id="21454-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="21454-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="21454-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="21454-113">Delegated (work or school account)</span></span> | <span data-ttu-id="21454-114">RoleManagement. ReadWrite. Directory, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="21454-114">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="21454-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="21454-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="21454-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="21454-116">Not supported.</span></span>    |
|<span data-ttu-id="21454-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="21454-117">Application</span></span> | <span data-ttu-id="21454-118">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="21454-118">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="21454-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="21454-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits/{id}/scopedRoleMembers
```
## <a name="request-headers"></a><span data-ttu-id="21454-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="21454-120">Request headers</span></span>
| <span data-ttu-id="21454-121">Nome</span><span class="sxs-lookup"><span data-stu-id="21454-121">Name</span></span>      |<span data-ttu-id="21454-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="21454-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="21454-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="21454-123">Authorization</span></span>  | <span data-ttu-id="21454-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="21454-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="21454-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="21454-126">Request body</span></span>
<span data-ttu-id="21454-127">No corpo da solicitação, forneça uma representação JSON do objeto [scopedRoleMembership](../resources/scopedrolemembership.md) .</span><span class="sxs-lookup"><span data-stu-id="21454-127">In the request body, supply a JSON representation of [scopedRoleMembership](../resources/scopedrolemembership.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="21454-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="21454-128">Response</span></span>

<span data-ttu-id="21454-129">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [scopedRoleMembership](../resources/scopedrolemembership.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="21454-129">If successful, this method returns `201 Created` response code and [scopedRoleMembership](../resources/scopedrolemembership.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21454-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="21454-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="21454-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="21454-131">Request</span></span>
<span data-ttu-id="21454-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="21454-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="21454-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="21454-133">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="21454-134">C#</span><span class="sxs-lookup"><span data-stu-id="21454-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-scopedrolemembership-from-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="21454-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="21454-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-scopedrolemembership-from-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="21454-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="21454-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-scopedrolemembership-from-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="21454-137">No corpo da solicitação, forneça uma representação JSON do objeto [scopedRoleMembership](../resources/scopedrolemembership.md) .</span><span class="sxs-lookup"><span data-stu-id="21454-137">In the request body, supply a JSON representation of [scopedRoleMembership](../resources/scopedrolemembership.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="21454-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="21454-138">Response</span></span>
<span data-ttu-id="21454-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="21454-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
