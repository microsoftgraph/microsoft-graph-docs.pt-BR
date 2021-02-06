---
title: Tipo de recurso scopedRoleMembership
description: Uma associação de função com escopo descreve a associação de um usuário a uma função de diretório, que tem como escopo uma Unidade Administrativa (AU).  Isso fornece um mecanismo para permitir que um administrador de empresa em todo o locatário delegar privilégios administrativos a um usuário para gerenciar usuários e grupos em um subconjunto da organização (o subconjunto sendo definido por uma AU).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: abhijeetsinha
ms.openlocfilehash: ffd1e616d94ccf959b8535f46f79a2c7c57e00c2
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134695"
---
# <a name="scopedrolemembership-resource-type"></a><span data-ttu-id="b8d41-104">Tipo de recurso scopedRoleMembership</span><span class="sxs-lookup"><span data-stu-id="b8d41-104">scopedRoleMembership resource type</span></span>

<span data-ttu-id="b8d41-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8d41-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8d41-106">Uma associação de função com escopo descreve a associação de um usuário a uma função de diretório, que tem como escopo uma Unidade Administrativa (AU).</span><span class="sxs-lookup"><span data-stu-id="b8d41-106">A scoped-role membership describes a user's membership of a directory role, that is further scoped to an Administrative Unit (AU).</span></span>  <span data-ttu-id="b8d41-107">Isso fornece um mecanismo para permitir que um administrador de empresa de todo o locatário delegar privilégios administrativos a um usuário para gerenciar usuários e grupos em um subconjunto da organização (o subconjunto definido por uma AU).</span><span class="sxs-lookup"><span data-stu-id="b8d41-107">This provides a mechanism to allow a tenant-wide company administrator to delegate administrative privileges to a user to manage users and groups in a subset of the organization (the subset being defined by an AU).</span></span>

## <a name="methods"></a><span data-ttu-id="b8d41-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="b8d41-108">Methods</span></span>
<span data-ttu-id="b8d41-109">Não há suporte para consultas diretas a esse recurso.</span><span class="sxs-lookup"><span data-stu-id="b8d41-109">Direct queries to this resource are not supported.</span></span>  <span data-ttu-id="b8d41-110">Consulte o tópico [de](administrativeunit.md) unidades administrativas para ver informações sobre como consultar associações de função com escopo, bem como adicionar e remover associações de função com escopo.</span><span class="sxs-lookup"><span data-stu-id="b8d41-110">Please see the [administrative units](administrativeunit.md) topic to see information on how to query for scoped-role memberships, as well as adding and removing scoped-role memberships.</span></span>

## <a name="properties"></a><span data-ttu-id="b8d41-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b8d41-111">Properties</span></span>
| <span data-ttu-id="b8d41-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b8d41-112">Property</span></span>   | <span data-ttu-id="b8d41-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="b8d41-113">Type</span></span> | <span data-ttu-id="b8d41-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8d41-114">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="b8d41-115">administrativeUnitId</span><span class="sxs-lookup"><span data-stu-id="b8d41-115">administrativeUnitId</span></span>|<span data-ttu-id="b8d41-116">string</span><span class="sxs-lookup"><span data-stu-id="b8d41-116">string</span></span>|<span data-ttu-id="b8d41-117">Identificador exclusivo da unidade administrativa para a qual a função de diretório tem escopo</span><span class="sxs-lookup"><span data-stu-id="b8d41-117">Unique identifier for the administrative unit that the directory role is scoped to</span></span>|
|<span data-ttu-id="b8d41-118">id</span><span class="sxs-lookup"><span data-stu-id="b8d41-118">id</span></span>|<span data-ttu-id="b8d41-119">string</span><span class="sxs-lookup"><span data-stu-id="b8d41-119">string</span></span>| <span data-ttu-id="b8d41-120">Identificador exclusivo da associação de função com escopo.</span><span class="sxs-lookup"><span data-stu-id="b8d41-120">Unique identifier for the scoped-role membership.</span></span> <span data-ttu-id="b8d41-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b8d41-121">Read-only.</span></span>|
|<span data-ttu-id="b8d41-122">roleId</span><span class="sxs-lookup"><span data-stu-id="b8d41-122">roleId</span></span>|<span data-ttu-id="b8d41-123">string</span><span class="sxs-lookup"><span data-stu-id="b8d41-123">string</span></span>| <span data-ttu-id="b8d41-124">Identificador exclusivo da função de diretório na qual o membro está.</span><span class="sxs-lookup"><span data-stu-id="b8d41-124">Unique identifier for the directory role that the member is in.</span></span>|
|<span data-ttu-id="b8d41-125">roleMemberInfo</span><span class="sxs-lookup"><span data-stu-id="b8d41-125">roleMemberInfo</span></span>|[<span data-ttu-id="b8d41-126">identity</span><span class="sxs-lookup"><span data-stu-id="b8d41-126">identity</span></span>](identity.md)| <span data-ttu-id="b8d41-127">Informações de identidade do membro da função.</span><span class="sxs-lookup"><span data-stu-id="b8d41-127">Role member identity information.</span></span> <span data-ttu-id="b8d41-128">Representa o usuário que é membro dessa função com escopo.</span><span class="sxs-lookup"><span data-stu-id="b8d41-128">Represents the user that is a member of this scoped-role.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8d41-129">Relações</span><span class="sxs-lookup"><span data-stu-id="b8d41-129">Relationships</span></span>
<span data-ttu-id="b8d41-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b8d41-130">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="b8d41-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b8d41-131">JSON representation</span></span>

<span data-ttu-id="b8d41-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b8d41-132">Here is a JSON representation of the resource.</span></span>

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


