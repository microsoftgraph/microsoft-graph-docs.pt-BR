---
title: Adicionar um scopedRoleMember
description: 'Adicione um novo scopedRoleMembership. Observação: Somente as funções de *administrador da conta de usuário* e o *administrador de assistência técnica* são suportadas atualmente para as associações de função com escopo.'
ms.openlocfilehash: bab8b1ba5d9093617f1aafb48d84f41badef2566
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034072"
---
# <a name="add-a-scopedrolemember"></a><span data-ttu-id="f38e0-104">Adicionar um scopedRoleMember</span><span class="sxs-lookup"><span data-stu-id="f38e0-104">Add a scopedRoleMember</span></span>

> <span data-ttu-id="f38e0-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f38e0-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f38e0-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f38e0-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f38e0-107">Adicione um novo [scopedRoleMembership](../resources/scopedrolemembership.md).</span><span class="sxs-lookup"><span data-stu-id="f38e0-107">Add a new [scopedRoleMembership](../resources/scopedrolemembership.md).</span></span> <span data-ttu-id="f38e0-108">Observação: Somente as funções de *administrador da conta de usuário* e o *administrador de assistência técnica* são suportadas atualmente para as associações de função com escopo.</span><span class="sxs-lookup"><span data-stu-id="f38e0-108">NOTE: Only the *User account administrator* and *Helpdesk administrator* roles are currently supported for scoped-role memberships.</span></span>

## <a name="permissions"></a><span data-ttu-id="f38e0-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="f38e0-109">Permissions</span></span>
<span data-ttu-id="f38e0-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f38e0-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f38e0-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f38e0-112">Permission type</span></span>      | <span data-ttu-id="f38e0-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f38e0-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f38e0-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f38e0-114">Delegated (work or school account)</span></span> | <span data-ttu-id="f38e0-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f38e0-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f38e0-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f38e0-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f38e0-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f38e0-117">Not supported.</span></span>    |
|<span data-ttu-id="f38e0-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f38e0-118">Application</span></span> | <span data-ttu-id="f38e0-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f38e0-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f38e0-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f38e0-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits/{id}/scopedRoleMembers
```
## <a name="request-headers"></a><span data-ttu-id="f38e0-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f38e0-121">Request headers</span></span>
| <span data-ttu-id="f38e0-122">Nome</span><span class="sxs-lookup"><span data-stu-id="f38e0-122">Name</span></span>      |<span data-ttu-id="f38e0-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f38e0-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f38e0-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f38e0-124">Authorization</span></span>  | <span data-ttu-id="f38e0-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f38e0-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f38e0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f38e0-127">Request body</span></span>
<span data-ttu-id="f38e0-128">No corpo da solicitação, fornece uma representação JSON do objeto [scopedRoleMembership](../resources/scopedrolemembership.md) .</span><span class="sxs-lookup"><span data-stu-id="f38e0-128">In the request body, supply a JSON representation of [scopedRoleMembership](../resources/scopedrolemembership.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f38e0-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f38e0-129">Response</span></span>

<span data-ttu-id="f38e0-130">Se tiver êxito, este método retornará `201 Created` objeto response de código e [scopedRoleMembership](../resources/scopedrolemembership.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f38e0-130">If successful, this method returns `201 Created` response code and [scopedRoleMembership](../resources/scopedrolemembership.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f38e0-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f38e0-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f38e0-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f38e0-132">Request</span></span>
<span data-ttu-id="f38e0-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f38e0-133">Here is an example of the request.</span></span>
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
<span data-ttu-id="f38e0-134">No corpo da solicitação, fornece uma representação JSON do objeto [scopedRoleMembership](../resources/scopedrolemembership.md) .</span><span class="sxs-lookup"><span data-stu-id="f38e0-134">In the request body, supply a JSON representation of [scopedRoleMembership](../resources/scopedrolemembership.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="f38e0-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f38e0-135">Response</span></span>
<span data-ttu-id="f38e0-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f38e0-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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