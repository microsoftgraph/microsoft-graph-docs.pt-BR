---
title: tipo de recurso scopedRoleMembership
description: Uma associação de função com escopo descreve a associação de um usuário de uma função de diretório, que tem mais escopo para uma unidade administrativa (AU).  Isso fornece um mecanismo para permitir que uma empresa de todo o locatário adminsistrator delegar privilégios administrativos a um usuário para gerenciar usuários e grupos em um subconjunto da organização (o subconjunto que está definido por uma AU).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 2580555bf3d10454aad9052f694ff1a62bf4b9b1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965278"
---
# <a name="scopedrolemembership-resource-type"></a><span data-ttu-id="ad1b8-104">tipo de recurso scopedRoleMembership</span><span class="sxs-lookup"><span data-stu-id="ad1b8-104">scopedRoleMembership resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad1b8-105">Uma associação de função com escopo descreve a associação de um usuário de uma função de diretório, que tem mais escopo para uma unidade administrativa (AU).</span><span class="sxs-lookup"><span data-stu-id="ad1b8-105">A scoped-role membership describes a user's membership of a directory role, that is further scoped to an Administrative Unit (AU).</span></span>  <span data-ttu-id="ad1b8-106">Isso fornece um mecanismo para permitir que uma empresa de todo o locatário adminsistrator delegar privilégios administrativos a um usuário para gerenciar usuários e grupos em um subconjunto da organização (o subconjunto que está definido por uma AU).</span><span class="sxs-lookup"><span data-stu-id="ad1b8-106">This provides a mechanism to allow a tenant-wide company adminsistrator to delegate administrative privileges to a user to manage users and groups in a subset of the organization (the subset being defined by an AU).</span></span>

## <a name="methods"></a><span data-ttu-id="ad1b8-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="ad1b8-107">Methods</span></span>
<span data-ttu-id="ad1b8-108">Não há suporte para consultas diretas a esse recurso.</span><span class="sxs-lookup"><span data-stu-id="ad1b8-108">Direct queries to this resource are not supported.</span></span>  <span data-ttu-id="ad1b8-109">Confira o tópico [unidades administrativas](administrativeunit.md) para ver informações sobre como consultar as associações com escopo de função, bem como adicionar e remover associações com escopo de função.</span><span class="sxs-lookup"><span data-stu-id="ad1b8-109">Please see the [adminstrative units](administrativeunit.md) topic to see information on how to query for scoped-role memberships, as well as adding and removing scoped-role memberships.</span></span> 

## <a name="properties"></a><span data-ttu-id="ad1b8-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ad1b8-110">Properties</span></span>
| <span data-ttu-id="ad1b8-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ad1b8-111">Property</span></span>   | <span data-ttu-id="ad1b8-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="ad1b8-112">Type</span></span> | <span data-ttu-id="ad1b8-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="ad1b8-113">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="ad1b8-114">administrativeUnitId</span><span class="sxs-lookup"><span data-stu-id="ad1b8-114">administrativeUnitId</span></span>|<span data-ttu-id="ad1b8-115">string</span><span class="sxs-lookup"><span data-stu-id="ad1b8-115">string</span></span>|<span data-ttu-id="ad1b8-116">Identificador exclusivo da unidade administrativa à qual a função de diretório tem escopo</span><span class="sxs-lookup"><span data-stu-id="ad1b8-116">Unique identifier for the administrative unit that the directory role is scoped to</span></span>|
|<span data-ttu-id="ad1b8-117">id</span><span class="sxs-lookup"><span data-stu-id="ad1b8-117">id</span></span>|<span data-ttu-id="ad1b8-118">string</span><span class="sxs-lookup"><span data-stu-id="ad1b8-118">string</span></span>| <span data-ttu-id="ad1b8-119">Identificador exclusivo da associação com escopo de função.</span><span class="sxs-lookup"><span data-stu-id="ad1b8-119">Unique identifier for the scoped-role membership.</span></span> <span data-ttu-id="ad1b8-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ad1b8-120">Read-only.</span></span>|
|<span data-ttu-id="ad1b8-121">roleId</span><span class="sxs-lookup"><span data-stu-id="ad1b8-121">roleId</span></span>|<span data-ttu-id="ad1b8-122">string</span><span class="sxs-lookup"><span data-stu-id="ad1b8-122">string</span></span>| <span data-ttu-id="ad1b8-123">Identificador exclusivo da função de diretório em que o membro está.</span><span class="sxs-lookup"><span data-stu-id="ad1b8-123">Unique identifier for the directory role that the member is in.</span></span>|
|<span data-ttu-id="ad1b8-124">roleMemberInfo</span><span class="sxs-lookup"><span data-stu-id="ad1b8-124">roleMemberInfo</span></span>|[<span data-ttu-id="ad1b8-125">identity</span><span class="sxs-lookup"><span data-stu-id="ad1b8-125">identity</span></span>](identity.md)| <span data-ttu-id="ad1b8-126">Informações de identidade de membro da função.</span><span class="sxs-lookup"><span data-stu-id="ad1b8-126">Role member identity information.</span></span> <span data-ttu-id="ad1b8-127">Representa o usuário que é um membro desse escopo-Role.</span><span class="sxs-lookup"><span data-stu-id="ad1b8-127">Represents the user that is a member of this scoped-role.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ad1b8-128">Relações</span><span class="sxs-lookup"><span data-stu-id="ad1b8-128">Relationships</span></span>
<span data-ttu-id="ad1b8-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ad1b8-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="ad1b8-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ad1b8-130">JSON representation</span></span>

<span data-ttu-id="ad1b8-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ad1b8-131">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scopedRoleMembership"
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
  "suppressions": []
}
-->
