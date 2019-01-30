---
title: tipo de recurso de scopedRoleMembership
description: Uma associação de função com escopo descreve a associação de um usuário de uma função de diretório, que ainda mais destinada para uma unidade administrativa (AU).  Isso oferece um mecanismo para permitir que um adminsistrator locatário toda empresa delegar privilégios administrativos para um usuário gerencie usuários e grupos em um subconjunto da organização (o subconjunto está sendo definido por um AU).
localization_priority: Normal
ms.openlocfilehash: 2d51ad696487e7daafb9b0f4fcef0934e4f6d6e2
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640788"
---
# <a name="scopedrolemembership-resource-type"></a><span data-ttu-id="8361c-104">tipo de recurso de scopedRoleMembership</span><span class="sxs-lookup"><span data-stu-id="8361c-104">scopedRoleMembership resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8361c-105">Uma associação de função com escopo descreve a associação de um usuário de uma função de diretório, que ainda mais destinada para uma unidade administrativa (AU).</span><span class="sxs-lookup"><span data-stu-id="8361c-105">A scoped-role membership describes a user's membership of a directory role, that is further scoped to an Administrative Unit (AU).</span></span>  <span data-ttu-id="8361c-106">Isso oferece um mecanismo para permitir que um adminsistrator locatário toda empresa delegar privilégios administrativos para um usuário gerencie usuários e grupos em um subconjunto da organização (o subconjunto está sendo definido por um AU).</span><span class="sxs-lookup"><span data-stu-id="8361c-106">This provides a mechanism to allow a tenant-wide company adminsistrator to delegate administrative privileges to a user to manage users and groups in a subset of the organization (the subset being defined by an AU).</span></span>

## <a name="methods"></a><span data-ttu-id="8361c-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="8361c-107">Methods</span></span>
<span data-ttu-id="8361c-108">Consultas diretas para este recurso não são suportadas.</span><span class="sxs-lookup"><span data-stu-id="8361c-108">Direct queries to this resource are not supported.</span></span>  <span data-ttu-id="8361c-109">Por favor, consulte o tópico de [unidades administrativas](administrativeunit.md) para ver informações sobre como consultar as associações de função com escopo, bem como adicionando e removendo associações de função com escopo.</span><span class="sxs-lookup"><span data-stu-id="8361c-109">Please see the [adminstrative units](administrativeunit.md) topic to see information on how to query for scoped-role memberships, as well as adding and removing scoped-role memberships.</span></span> 

## <a name="properties"></a><span data-ttu-id="8361c-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8361c-110">Properties</span></span>
| <span data-ttu-id="8361c-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8361c-111">Property</span></span>   | <span data-ttu-id="8361c-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="8361c-112">Type</span></span> | <span data-ttu-id="8361c-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="8361c-113">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="8361c-114">administrativeUnitId</span><span class="sxs-lookup"><span data-stu-id="8361c-114">administrativeUnitId</span></span>|<span data-ttu-id="8361c-115">string</span><span class="sxs-lookup"><span data-stu-id="8361c-115">string</span></span>|<span data-ttu-id="8361c-116">Identificador exclusivo para a unidade administrativa que a função directory destinada a</span><span class="sxs-lookup"><span data-stu-id="8361c-116">Unique identifier for the administrative unit that the directory role is scoped to</span></span>|
|<span data-ttu-id="8361c-117">id</span><span class="sxs-lookup"><span data-stu-id="8361c-117">id</span></span>|<span data-ttu-id="8361c-118">string</span><span class="sxs-lookup"><span data-stu-id="8361c-118">string</span></span>| <span data-ttu-id="8361c-119">Identificador exclusivo para a associação da função com escopo.</span><span class="sxs-lookup"><span data-stu-id="8361c-119">Unique identifier for the scoped-role membership.</span></span> <span data-ttu-id="8361c-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8361c-120">Read-only.</span></span>|
|<span data-ttu-id="8361c-121">roleId</span><span class="sxs-lookup"><span data-stu-id="8361c-121">roleId</span></span>|<span data-ttu-id="8361c-122">string</span><span class="sxs-lookup"><span data-stu-id="8361c-122">string</span></span>| <span data-ttu-id="8361c-123">Identificador exclusivo para a função de diretório que o membro é no.</span><span class="sxs-lookup"><span data-stu-id="8361c-123">Unique identifier for the directory role that the member is in.</span></span>|
|<span data-ttu-id="8361c-124">roleMemberInfo</span><span class="sxs-lookup"><span data-stu-id="8361c-124">roleMemberInfo</span></span>|[<span data-ttu-id="8361c-125">identity</span><span class="sxs-lookup"><span data-stu-id="8361c-125">identity</span></span>](identity.md)| <span data-ttu-id="8361c-126">Informações de identidade do membro de função.</span><span class="sxs-lookup"><span data-stu-id="8361c-126">Role member identity information.</span></span> <span data-ttu-id="8361c-127">Representa o usuário que seja membro desta função com escopo.</span><span class="sxs-lookup"><span data-stu-id="8361c-127">Represents the user that is a member of this scoped-role.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8361c-128">Relações</span><span class="sxs-lookup"><span data-stu-id="8361c-128">Relationships</span></span>
<span data-ttu-id="8361c-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8361c-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="8361c-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8361c-130">JSON representation</span></span>

<span data-ttu-id="8361c-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8361c-131">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "scopedRoleMembership resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/scopedrolemembership.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
