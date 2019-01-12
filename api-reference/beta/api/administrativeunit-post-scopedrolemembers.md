---
title: Adicionar um scopedRoleMember
description: 'Adicione um novo scopedRoleMembership. Observação: Somente as funções de *administrador da conta de usuário* e o *administrador de assistência técnica* são suportadas atualmente para as associações de função com escopo.'
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6dce85d891c9d124d1d57d14a8a7309fb766b895
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27936680"
---
# <a name="add-a-scopedrolemember"></a><span data-ttu-id="5983d-104">Adicionar um scopedRoleMember</span><span class="sxs-lookup"><span data-stu-id="5983d-104">Add a scopedRoleMember</span></span>

> <span data-ttu-id="5983d-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5983d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5983d-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5983d-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5983d-107">Adicione um novo [scopedRoleMembership](../resources/scopedrolemembership.md).</span><span class="sxs-lookup"><span data-stu-id="5983d-107">Add a new [scopedRoleMembership](../resources/scopedrolemembership.md).</span></span> <span data-ttu-id="5983d-108">Observação: Somente as funções de *administrador da conta de usuário* e o *administrador de assistência técnica* são suportadas atualmente para as associações de função com escopo.</span><span class="sxs-lookup"><span data-stu-id="5983d-108">NOTE: Only the *User account administrator* and *Helpdesk administrator* roles are currently supported for scoped-role memberships.</span></span>

## <a name="permissions"></a><span data-ttu-id="5983d-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="5983d-109">Permissions</span></span>
<span data-ttu-id="5983d-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5983d-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5983d-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5983d-112">Permission type</span></span>      | <span data-ttu-id="5983d-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5983d-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5983d-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5983d-114">Delegated (work or school account)</span></span> | <span data-ttu-id="5983d-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5983d-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5983d-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5983d-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5983d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5983d-117">Not supported.</span></span>    |
|<span data-ttu-id="5983d-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5983d-118">Application</span></span> | <span data-ttu-id="5983d-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5983d-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5983d-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5983d-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits/{id}/scopedRoleMembers
```
## <a name="request-headers"></a><span data-ttu-id="5983d-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5983d-121">Request headers</span></span>
| <span data-ttu-id="5983d-122">Nome</span><span class="sxs-lookup"><span data-stu-id="5983d-122">Name</span></span>      |<span data-ttu-id="5983d-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="5983d-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5983d-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="5983d-124">Authorization</span></span>  | <span data-ttu-id="5983d-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5983d-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5983d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5983d-127">Request body</span></span>
<span data-ttu-id="5983d-128">No corpo da solicitação, fornece uma representação JSON do objeto [scopedRoleMembership](../resources/scopedrolemembership.md) .</span><span class="sxs-lookup"><span data-stu-id="5983d-128">In the request body, supply a JSON representation of [scopedRoleMembership](../resources/scopedrolemembership.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="5983d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="5983d-129">Response</span></span>

<span data-ttu-id="5983d-130">Se tiver êxito, este método retornará `201 Created` objeto response de código e [scopedRoleMembership](../resources/scopedrolemembership.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5983d-130">If successful, this method returns `201 Created` response code and [scopedRoleMembership](../resources/scopedrolemembership.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5983d-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5983d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5983d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5983d-132">Request</span></span>
<span data-ttu-id="5983d-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5983d-133">Here is an example of the request.</span></span>
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
<span data-ttu-id="5983d-134">No corpo da solicitação, fornece uma representação JSON do objeto [scopedRoleMembership](../resources/scopedrolemembership.md) .</span><span class="sxs-lookup"><span data-stu-id="5983d-134">In the request body, supply a JSON representation of [scopedRoleMembership](../resources/scopedrolemembership.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="5983d-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="5983d-135">Response</span></span>
<span data-ttu-id="5983d-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5983d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scopedrolemembership"
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
<!-- {
  "type": "#page.annotation",
  "description": "Create scopedRoleMembership",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
