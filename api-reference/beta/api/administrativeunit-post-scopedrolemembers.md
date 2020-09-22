---
title: Adicionar um scopedRoleMember
description: 'Adicione um novo scopedRoleMembership. Observação: somente as funções de administrador de *conta de usuário* e *administrador de helpdesk* têm suporte para associações com escopo de função.'
localization_priority: Normal
author: anandyadavMSFT
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 426612052396fa5beb533d6fe680345436e38690
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997181"
---
# <a name="add-a-scopedrolemember"></a><span data-ttu-id="5b7da-104">Adicionar um scopedRoleMember</span><span class="sxs-lookup"><span data-stu-id="5b7da-104">Add a scopedRoleMember</span></span>

<span data-ttu-id="5b7da-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b7da-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b7da-106">Adicione um novo [scopedRoleMembership](../resources/scopedrolemembership.md).</span><span class="sxs-lookup"><span data-stu-id="5b7da-106">Add a new [scopedRoleMembership](../resources/scopedrolemembership.md).</span></span> <span data-ttu-id="5b7da-107">Observação: somente as funções de administrador de *conta de usuário* e *administrador de helpdesk* têm suporte para associações com escopo de função.</span><span class="sxs-lookup"><span data-stu-id="5b7da-107">NOTE: Only the *User account administrator* and *Helpdesk administrator* roles are currently supported for scoped-role memberships.</span></span>

## <a name="permissions"></a><span data-ttu-id="5b7da-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="5b7da-108">Permissions</span></span>
<span data-ttu-id="5b7da-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b7da-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5b7da-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5b7da-111">Permission type</span></span>      | <span data-ttu-id="5b7da-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5b7da-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5b7da-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5b7da-113">Delegated (work or school account)</span></span> | <span data-ttu-id="5b7da-114">RoleManagement. ReadWrite. Directory, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="5b7da-114">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5b7da-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5b7da-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b7da-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5b7da-116">Not supported.</span></span>    |
|<span data-ttu-id="5b7da-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5b7da-117">Application</span></span> | <span data-ttu-id="5b7da-118">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="5b7da-118">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="5b7da-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5b7da-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits/{id}/scopedRoleMembers
```
## <a name="request-headers"></a><span data-ttu-id="5b7da-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5b7da-120">Request headers</span></span>
| <span data-ttu-id="5b7da-121">Nome</span><span class="sxs-lookup"><span data-stu-id="5b7da-121">Name</span></span>      |<span data-ttu-id="5b7da-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b7da-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5b7da-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5b7da-123">Authorization</span></span>  | <span data-ttu-id="5b7da-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5b7da-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b7da-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5b7da-126">Request body</span></span>
<span data-ttu-id="5b7da-127">No corpo da solicitação, forneça uma representação JSON do objeto [scopedRoleMembership](../resources/scopedrolemembership.md) .</span><span class="sxs-lookup"><span data-stu-id="5b7da-127">In the request body, supply a JSON representation of [scopedRoleMembership](../resources/scopedrolemembership.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="5b7da-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b7da-128">Response</span></span>

<span data-ttu-id="5b7da-129">Se bem-sucedido, este método retorna o `201 Created` código de resposta e o objeto [scopedRoleMembership](../resources/scopedrolemembership.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5b7da-129">If successful, this method returns `201 Created` response code and [scopedRoleMembership](../resources/scopedrolemembership.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b7da-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5b7da-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5b7da-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5b7da-131">Request</span></span>
<span data-ttu-id="5b7da-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5b7da-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5b7da-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="5b7da-133">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5b7da-134">C#</span><span class="sxs-lookup"><span data-stu-id="5b7da-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-scopedrolemembership-from-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5b7da-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5b7da-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-scopedrolemembership-from-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5b7da-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5b7da-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-scopedrolemembership-from-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="5b7da-137">No corpo da solicitação, forneça uma representação JSON do objeto [scopedRoleMembership](../resources/scopedrolemembership.md) .</span><span class="sxs-lookup"><span data-stu-id="5b7da-137">In the request body, supply a JSON representation of [scopedRoleMembership](../resources/scopedrolemembership.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="5b7da-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b7da-138">Response</span></span>
<span data-ttu-id="5b7da-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5b7da-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


