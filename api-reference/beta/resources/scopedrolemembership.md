---
title: tipo de recurso scopedRoleMembership
description: Uma associação de função com escopo descreve a associação de um usuário de uma função de diretório, que tem mais escopo para uma unidade administrativa (AU).  Isso fornece um mecanismo para permitir que uma empresa de todo o locatário adminsistrator delegar privilégios administrativos a um usuário para gerenciar usuários e grupos em um subconjunto da organização (o subconjunto que está definido por uma AU).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: abhijeetsinha
ms.openlocfilehash: 27eae463ab0f5fe0718a6d97602e366d32b11b86
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812432"
---
# <a name="scopedrolemembership-resource-type"></a><span data-ttu-id="0691a-104">tipo de recurso scopedRoleMembership</span><span class="sxs-lookup"><span data-stu-id="0691a-104">scopedRoleMembership resource type</span></span>

<span data-ttu-id="0691a-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0691a-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0691a-106">Uma associação de função com escopo descreve a associação de um usuário de uma função de diretório, que tem mais escopo para uma unidade administrativa (AU).</span><span class="sxs-lookup"><span data-stu-id="0691a-106">A scoped-role membership describes a user's membership of a directory role, that is further scoped to an Administrative Unit (AU).</span></span>  <span data-ttu-id="0691a-107">Isso fornece um mecanismo para permitir que um administrador da empresa de todo o locatário delegue privilégios administrativos a um usuário para gerenciar usuários e grupos em um subconjunto da organização (o subconjunto que está sendo definido por uma AU).</span><span class="sxs-lookup"><span data-stu-id="0691a-107">This provides a mechanism to allow a tenant-wide company administrator to delegate administrative privileges to a user to manage users and groups in a subset of the organization (the subset being defined by an AU).</span></span>

## <a name="methods"></a><span data-ttu-id="0691a-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="0691a-108">Methods</span></span>
<span data-ttu-id="0691a-109">Não há suporte para consultas diretas a esse recurso.</span><span class="sxs-lookup"><span data-stu-id="0691a-109">Direct queries to this resource are not supported.</span></span>  <span data-ttu-id="0691a-110">Confira o tópico [unidades administrativas](administrativeunit.md) para ver informações sobre como consultar as associações com escopo de função, bem como adicionar e remover associações com escopo de função.</span><span class="sxs-lookup"><span data-stu-id="0691a-110">Please see the [administrative units](administrativeunit.md) topic to see information on how to query for scoped-role memberships, as well as adding and removing scoped-role memberships.</span></span>

## <a name="properties"></a><span data-ttu-id="0691a-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0691a-111">Properties</span></span>
| <span data-ttu-id="0691a-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0691a-112">Property</span></span>   | <span data-ttu-id="0691a-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="0691a-113">Type</span></span> | <span data-ttu-id="0691a-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="0691a-114">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="0691a-115">administrativeUnitId</span><span class="sxs-lookup"><span data-stu-id="0691a-115">administrativeUnitId</span></span>|<span data-ttu-id="0691a-116">string</span><span class="sxs-lookup"><span data-stu-id="0691a-116">string</span></span>|<span data-ttu-id="0691a-117">Identificador exclusivo da unidade administrativa à qual a função de diretório tem escopo</span><span class="sxs-lookup"><span data-stu-id="0691a-117">Unique identifier for the administrative unit that the directory role is scoped to</span></span>|
|<span data-ttu-id="0691a-118">id</span><span class="sxs-lookup"><span data-stu-id="0691a-118">id</span></span>|<span data-ttu-id="0691a-119">string</span><span class="sxs-lookup"><span data-stu-id="0691a-119">string</span></span>| <span data-ttu-id="0691a-120">Identificador exclusivo da associação com escopo de função.</span><span class="sxs-lookup"><span data-stu-id="0691a-120">Unique identifier for the scoped-role membership.</span></span> <span data-ttu-id="0691a-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0691a-121">Read-only.</span></span>|
|<span data-ttu-id="0691a-122">roleId</span><span class="sxs-lookup"><span data-stu-id="0691a-122">roleId</span></span>|<span data-ttu-id="0691a-123">string</span><span class="sxs-lookup"><span data-stu-id="0691a-123">string</span></span>| <span data-ttu-id="0691a-124">Identificador exclusivo da função de diretório em que o membro está.</span><span class="sxs-lookup"><span data-stu-id="0691a-124">Unique identifier for the directory role that the member is in.</span></span>|
|<span data-ttu-id="0691a-125">roleMemberInfo</span><span class="sxs-lookup"><span data-stu-id="0691a-125">roleMemberInfo</span></span>|[<span data-ttu-id="0691a-126">identity</span><span class="sxs-lookup"><span data-stu-id="0691a-126">identity</span></span>](identity.md)| <span data-ttu-id="0691a-127">Informações de identidade de membro da função.</span><span class="sxs-lookup"><span data-stu-id="0691a-127">Role member identity information.</span></span> <span data-ttu-id="0691a-128">Representa o usuário que é um membro desse escopo-Role.</span><span class="sxs-lookup"><span data-stu-id="0691a-128">Represents the user that is a member of this scoped-role.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0691a-129">Relações</span><span class="sxs-lookup"><span data-stu-id="0691a-129">Relationships</span></span>
<span data-ttu-id="0691a-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0691a-130">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="0691a-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0691a-131">JSON representation</span></span>

<span data-ttu-id="0691a-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0691a-132">Here is a JSON representation of the resource.</span></span>

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
