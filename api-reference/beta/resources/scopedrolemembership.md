---
title: tipo de recurso de scopedRoleMembership
description: Uma associação de função com escopo descreve a associação de um usuário de uma função de diretório, que ainda mais destinada para uma unidade administrativa (AU).  Isso oferece um mecanismo para permitir que um adminsistrator locatário toda empresa delegar privilégios administrativos para um usuário gerencie usuários e grupos em um subconjunto da organização (o subconjunto está sendo definido por um AU).
ms.openlocfilehash: bd635a5b1b06b98657ba24c397e2f67afb76fa8f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036460"
---
# <a name="scopedrolemembership-resource-type"></a><span data-ttu-id="141cd-104">tipo de recurso de scopedRoleMembership</span><span class="sxs-lookup"><span data-stu-id="141cd-104">scopedRoleMembership resource type</span></span>

> <span data-ttu-id="141cd-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="141cd-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="141cd-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="141cd-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="141cd-107">Uma associação de função com escopo descreve a associação de um usuário de uma função de diretório, que ainda mais destinada para uma unidade administrativa (AU).</span><span class="sxs-lookup"><span data-stu-id="141cd-107">A scoped-role membership describes a user's membership of a directory role, that is further scoped to an Administrative Unit (AU).</span></span>  <span data-ttu-id="141cd-108">Isso oferece um mecanismo para permitir que um adminsistrator locatário toda empresa delegar privilégios administrativos para um usuário gerencie usuários e grupos em um subconjunto da organização (o subconjunto está sendo definido por um AU).</span><span class="sxs-lookup"><span data-stu-id="141cd-108">This provides a mechanism to allow a tenant-wide company adminsistrator to delegate administrative privileges to a user to manage users and groups in a subset of the organization (the subset being defined by an AU).</span></span>

## <a name="methods"></a><span data-ttu-id="141cd-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="141cd-109">Methods</span></span>
<span data-ttu-id="141cd-110">Consultas diretas para este recurso não são suportadas.</span><span class="sxs-lookup"><span data-stu-id="141cd-110">Direct queries to this resource are not supported.</span></span>  <span data-ttu-id="141cd-111">Por favor, consulte o tópico de [unidades administrativas](administrativeunit.md) para ver informações sobre como consultar as associações de função com escopo, bem como adicionando e removendo associações de função com escopo.</span><span class="sxs-lookup"><span data-stu-id="141cd-111">Please see the [adminstrative units](administrativeunit.md) topic to see information on how to query for scoped-role memberships, as well as adding and removing scoped-role memberships.</span></span> 

## <a name="properties"></a><span data-ttu-id="141cd-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="141cd-112">Properties</span></span>
| <span data-ttu-id="141cd-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="141cd-113">Property</span></span>   | <span data-ttu-id="141cd-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="141cd-114">Type</span></span> | <span data-ttu-id="141cd-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="141cd-115">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="141cd-116">administrativeUnitId</span><span class="sxs-lookup"><span data-stu-id="141cd-116">administrativeUnitId</span></span>|<span data-ttu-id="141cd-117">string</span><span class="sxs-lookup"><span data-stu-id="141cd-117">string</span></span>|<span data-ttu-id="141cd-118">Identificador exclusivo para a unidade administrativa que a função directory destinada a</span><span class="sxs-lookup"><span data-stu-id="141cd-118">Unique identifier for the administrative unit that the directory role is scoped to</span></span>|
|<span data-ttu-id="141cd-119">id</span><span class="sxs-lookup"><span data-stu-id="141cd-119">id</span></span>|<span data-ttu-id="141cd-120">string</span><span class="sxs-lookup"><span data-stu-id="141cd-120">string</span></span>| <span data-ttu-id="141cd-121">Identificador exclusivo para a associação da função com escopo.</span><span class="sxs-lookup"><span data-stu-id="141cd-121">Unique identifier for the scoped-role membership.</span></span> <span data-ttu-id="141cd-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="141cd-122">Read-only.</span></span>|
|<span data-ttu-id="141cd-123">roleId</span><span class="sxs-lookup"><span data-stu-id="141cd-123">roleId</span></span>|<span data-ttu-id="141cd-124">string</span><span class="sxs-lookup"><span data-stu-id="141cd-124">string</span></span>| <span data-ttu-id="141cd-125">Identificador exclusivo para a função de diretório que o membro é no.</span><span class="sxs-lookup"><span data-stu-id="141cd-125">Unique identifier for the directory role that the member is in.</span></span>|
|<span data-ttu-id="141cd-126">roleMemberInfo</span><span class="sxs-lookup"><span data-stu-id="141cd-126">roleMemberInfo</span></span>|[<span data-ttu-id="141cd-127">identity</span><span class="sxs-lookup"><span data-stu-id="141cd-127">identity</span></span>](identity.md)| <span data-ttu-id="141cd-128">Informações de identidade do membro de função.</span><span class="sxs-lookup"><span data-stu-id="141cd-128">Role member identity information.</span></span> <span data-ttu-id="141cd-129">Representa o usuário que seja membro desta função com escopo.</span><span class="sxs-lookup"><span data-stu-id="141cd-129">Represents the user that is a member of this scoped-role.</span></span>|

## <a name="relationships"></a><span data-ttu-id="141cd-130">Relações</span><span class="sxs-lookup"><span data-stu-id="141cd-130">Relationships</span></span>
<span data-ttu-id="141cd-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="141cd-131">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="141cd-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="141cd-132">JSON representation</span></span>

<span data-ttu-id="141cd-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="141cd-133">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scopedrolemembership"
}-->

```json
{
  "administrativeUnitId": "string",
  "id": "string (identifier)",
  "roleId": "string",
  "roleMemberInfo": {"@odata.type": "microsoft.graph.identity"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "scopedRoleMembership resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->