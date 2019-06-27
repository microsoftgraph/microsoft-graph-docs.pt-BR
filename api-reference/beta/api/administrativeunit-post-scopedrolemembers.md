---
title: Adicionar um scopedRoleMember
description: 'Adicione um novo scopedRoleMembership. Observação: somente as funções de administrador de *conta de usuário* e *administrador de helpdesk* têm suporte para associações com escopo de função.'
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e933158e2510f26048b7f770aa43dfcd67b6cae9
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258678"
---
# <a name="add-a-scopedrolemember"></a><span data-ttu-id="a3a4d-104">Adicionar um scopedRoleMember</span><span class="sxs-lookup"><span data-stu-id="a3a4d-104">Add a scopedRoleMember</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3a4d-105">Adicione um novo [scopedRoleMembership](../resources/scopedrolemembership.md).</span><span class="sxs-lookup"><span data-stu-id="a3a4d-105">Add a new [scopedRoleMembership](../resources/scopedrolemembership.md).</span></span> <span data-ttu-id="a3a4d-106">Observação: somente as funções de administrador de *conta de usuário* e *administrador de helpdesk* têm suporte para associações com escopo de função.</span><span class="sxs-lookup"><span data-stu-id="a3a4d-106">NOTE: Only the *User account administrator* and *Helpdesk administrator* roles are currently supported for scoped-role memberships.</span></span>

## <a name="permissions"></a><span data-ttu-id="a3a4d-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a3a4d-107">Permissions</span></span>
<span data-ttu-id="a3a4d-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3a4d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a3a4d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a3a4d-110">Permission type</span></span>      | <span data-ttu-id="a3a4d-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a3a4d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a3a4d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a3a4d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a3a4d-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a3a4d-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a3a4d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a3a4d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3a4d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a3a4d-115">Not supported.</span></span>    |
|<span data-ttu-id="a3a4d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a3a4d-116">Application</span></span> | <span data-ttu-id="a3a4d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a3a4d-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a3a4d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a3a4d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits/{id}/scopedRoleMembers
```
## <a name="request-headers"></a><span data-ttu-id="a3a4d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a3a4d-119">Request headers</span></span>
| <span data-ttu-id="a3a4d-120">Nome</span><span class="sxs-lookup"><span data-stu-id="a3a4d-120">Name</span></span>      |<span data-ttu-id="a3a4d-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3a4d-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a3a4d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a3a4d-122">Authorization</span></span>  | <span data-ttu-id="a3a4d-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a3a4d-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3a4d-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a3a4d-125">Request body</span></span>
<span data-ttu-id="a3a4d-126">No corpo da solicitação, forneça uma representação JSON do objeto [scopedRoleMembership](../resources/scopedrolemembership.md) .</span><span class="sxs-lookup"><span data-stu-id="a3a4d-126">In the request body, supply a JSON representation of [scopedRoleMembership](../resources/scopedrolemembership.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a3a4d-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3a4d-127">Response</span></span>

<span data-ttu-id="a3a4d-128">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [scopedRoleMembership](../resources/scopedrolemembership.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a3a4d-128">If successful, this method returns `201 Created` response code and [scopedRoleMembership](../resources/scopedrolemembership.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3a4d-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a3a4d-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a3a4d-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a3a4d-130">Request</span></span>
<span data-ttu-id="a3a4d-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a3a4d-131">Here is an example of the request.</span></span>
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
<span data-ttu-id="a3a4d-132">No corpo da solicitação, forneça uma representação JSON do objeto [scopedRoleMembership](../resources/scopedrolemembership.md) .</span><span class="sxs-lookup"><span data-stu-id="a3a4d-132">In the request body, supply a JSON representation of [scopedRoleMembership](../resources/scopedrolemembership.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="a3a4d-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3a4d-133">Response</span></span>
<span data-ttu-id="a3a4d-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a3a4d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="a3a4d-137">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="a3a4d-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a3a4d-138">C#</span><span class="sxs-lookup"><span data-stu-id="a3a4d-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_scopedrolemembership_from_administrativeunit-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a3a4d-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="a3a4d-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_scopedrolemembership_from_administrativeunit-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="a3a4d-140">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a3a4d-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_scopedrolemembership_from_administrativeunit-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/administrativeunit-post-scopedrolemembers.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/administrativeunit-post-scopedrolemembers.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/administrativeunit-post-scopedrolemembers.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
