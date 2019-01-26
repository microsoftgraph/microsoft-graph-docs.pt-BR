---
title: Adicionar um scopedRoleMember
description: 'Adicione um novo scopedRoleMembership. Observação: Somente as funções de *administrador da conta de usuário* e o *administrador de assistência técnica* são suportadas atualmente para as associações de função com escopo.'
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e93dc3bc245b323e3c40fdd5678f4bfba495eafd
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571825"
---
# <a name="add-a-scopedrolemember"></a><span data-ttu-id="94a4c-104">Adicionar um scopedRoleMember</span><span class="sxs-lookup"><span data-stu-id="94a4c-104">Add a scopedRoleMember</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94a4c-105">Adicione um novo [scopedRoleMembership](../resources/scopedrolemembership.md).</span><span class="sxs-lookup"><span data-stu-id="94a4c-105">Add a new [scopedRoleMembership](../resources/scopedrolemembership.md).</span></span> <span data-ttu-id="94a4c-106">Observação: Somente as funções de *administrador da conta de usuário* e o *administrador de assistência técnica* são suportadas atualmente para as associações de função com escopo.</span><span class="sxs-lookup"><span data-stu-id="94a4c-106">NOTE: Only the *User account administrator* and *Helpdesk administrator* roles are currently supported for scoped-role memberships.</span></span>

## <a name="permissions"></a><span data-ttu-id="94a4c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="94a4c-107">Permissions</span></span>
<span data-ttu-id="94a4c-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94a4c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="94a4c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="94a4c-110">Permission type</span></span>      | <span data-ttu-id="94a4c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="94a4c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94a4c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="94a4c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="94a4c-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="94a4c-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="94a4c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="94a4c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94a4c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94a4c-115">Not supported.</span></span>    |
|<span data-ttu-id="94a4c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="94a4c-116">Application</span></span> | <span data-ttu-id="94a4c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94a4c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="94a4c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="94a4c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits/{id}/scopedRoleMembers
```
## <a name="request-headers"></a><span data-ttu-id="94a4c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="94a4c-119">Request headers</span></span>
| <span data-ttu-id="94a4c-120">Nome</span><span class="sxs-lookup"><span data-stu-id="94a4c-120">Name</span></span>      |<span data-ttu-id="94a4c-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="94a4c-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="94a4c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="94a4c-122">Authorization</span></span>  | <span data-ttu-id="94a4c-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94a4c-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="94a4c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="94a4c-125">Request body</span></span>
<span data-ttu-id="94a4c-126">No corpo da solicitação, fornece uma representação JSON do objeto [scopedRoleMembership](../resources/scopedrolemembership.md) .</span><span class="sxs-lookup"><span data-stu-id="94a4c-126">In the request body, supply a JSON representation of [scopedRoleMembership](../resources/scopedrolemembership.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="94a4c-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="94a4c-127">Response</span></span>

<span data-ttu-id="94a4c-128">Se tiver êxito, este método retornará `201 Created` objeto response de código e [scopedRoleMembership](../resources/scopedrolemembership.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94a4c-128">If successful, this method returns `201 Created` response code and [scopedRoleMembership](../resources/scopedrolemembership.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94a4c-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="94a4c-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="94a4c-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="94a4c-130">Request</span></span>
<span data-ttu-id="94a4c-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="94a4c-131">Here is an example of the request.</span></span>
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
<span data-ttu-id="94a4c-132">No corpo da solicitação, fornece uma representação JSON do objeto [scopedRoleMembership](../resources/scopedrolemembership.md) .</span><span class="sxs-lookup"><span data-stu-id="94a4c-132">In the request body, supply a JSON representation of [scopedRoleMembership](../resources/scopedrolemembership.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="94a4c-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="94a4c-133">Response</span></span>
<span data-ttu-id="94a4c-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="94a4c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/administrativeunit-post-scopedrolemembers.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
