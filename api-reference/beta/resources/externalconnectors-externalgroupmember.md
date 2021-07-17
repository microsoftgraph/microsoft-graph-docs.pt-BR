---
title: Tipo de recurso externalGroupMember
description: Representa um membro de um externalGroup usado para definir permissões no conteúdo externo adicionado à Microsoft Graph.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: e3626c718360982bf79cb9757a13e4b4c01669cd
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467568"
---
# <a name="externalgroupmember-resource-type"></a><span data-ttu-id="d33e0-103">Tipo de recurso externalGroupMember</span><span class="sxs-lookup"><span data-stu-id="d33e0-103">externalGroupMember resource type</span></span>

<span data-ttu-id="d33e0-104">Namespace: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="d33e0-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d33e0-105">Representa um membro de [um externalGroup](externalconnectors-externalgroup.md) usado para definir permissões no conteúdo externo adicionado à Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d33e0-105">Represents a member of an [externalGroup](externalconnectors-externalgroup.md) used to set permissions on external content added to Microsoft Graph.</span></span>

## <a name="methods"></a><span data-ttu-id="d33e0-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="d33e0-106">Methods</span></span>

| <span data-ttu-id="d33e0-107">Método</span><span class="sxs-lookup"><span data-stu-id="d33e0-107">Method</span></span>                                                              | <span data-ttu-id="d33e0-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d33e0-108">Return type</span></span>         | <span data-ttu-id="d33e0-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d33e0-109">Description</span></span>                              |
|:--------------------------------------------------------------------|:--------------------|:-----------------------------------------|
| [<span data-ttu-id="d33e0-110">Criar externalGroupMember</span><span class="sxs-lookup"><span data-stu-id="d33e0-110">Create externalGroupMember</span></span>](../api/externalconnectors-externalgroup-post-members.md) | [<span data-ttu-id="d33e0-111">externalGroupMember</span><span class="sxs-lookup"><span data-stu-id="d33e0-111">externalGroupMember</span></span>](../resources/externalconnectors-externalgroupmember.md) | <span data-ttu-id="d33e0-112">Crie um novo **objeto externalGroupMember.**</span><span class="sxs-lookup"><span data-stu-id="d33e0-112">Create a new **externalGroupMember** object.</span></span> |
| [<span data-ttu-id="d33e0-113">Excluir externalGroupMember</span><span class="sxs-lookup"><span data-stu-id="d33e0-113">Delete externalGroupMember</span></span>](../api/externalconnectors-externalgroupmember-delete.md)  | <span data-ttu-id="d33e0-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d33e0-114">None</span></span>                | <span data-ttu-id="d33e0-115">**Exclua um objeto externalGroupMember.**</span><span class="sxs-lookup"><span data-stu-id="d33e0-115">Delete an **externalGroupMember** object.</span></span>   |

## <a name="properties"></a><span data-ttu-id="d33e0-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d33e0-116">Properties</span></span>

| <span data-ttu-id="d33e0-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d33e0-117">Property</span></span>       | <span data-ttu-id="d33e0-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="d33e0-118">Type</span></span>                    | <span data-ttu-id="d33e0-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="d33e0-119">Description</span></span>                                                          |
|:---------------|:------------------------|:---------------------------------------------------------------------|
| <span data-ttu-id="d33e0-120">id</span><span class="sxs-lookup"><span data-stu-id="d33e0-120">id</span></span>             | <span data-ttu-id="d33e0-121">String</span><span class="sxs-lookup"><span data-stu-id="d33e0-121">String</span></span>                  | <span data-ttu-id="d33e0-122">A ID exclusiva do membro.</span><span class="sxs-lookup"><span data-stu-id="d33e0-122">The unique ID of the member.</span></span> <span data-ttu-id="d33e0-123">Seria objectId no caso de Azure Active Directory ou grupos e a propriedade **id** do **externalGroup** no caso de grupos externos.</span><span class="sxs-lookup"><span data-stu-id="d33e0-123">It would be the objectId in case of Azure Active Directory users or groups and the **id** property of the **externalGroup** in case of external groups.</span></span>                                    |
| <span data-ttu-id="d33e0-124">tipo</span><span class="sxs-lookup"><span data-stu-id="d33e0-124">type</span></span>           | <span data-ttu-id="d33e0-125">microsoft.graph.externalConnectors.externalGroupMemberType</span><span class="sxs-lookup"><span data-stu-id="d33e0-125">microsoft.graph.externalConnectors.externalGroupMemberType</span></span> | <span data-ttu-id="d33e0-126">O tipo de membro adicionado ao grupo externo.</span><span class="sxs-lookup"><span data-stu-id="d33e0-126">The type of member added to the external group.</span></span> <span data-ttu-id="d33e0-127">Os valores possíveis são: `user` `group` ou quando **identitySource** é `azureActiveDirectory` e apenas quando `group` **identitySource** é `external` .</span><span class="sxs-lookup"><span data-stu-id="d33e0-127">Possible values are: `user` or `group` when the **identitySource** is `azureActiveDirectory` and just `group` when the **identitySource** is `external`.</span></span> |
| <span data-ttu-id="d33e0-128">identitySource</span><span class="sxs-lookup"><span data-stu-id="d33e0-128">identitySource</span></span> | <span data-ttu-id="d33e0-129">microsoft.graph.externalConnectors.identitySourceType</span><span class="sxs-lookup"><span data-stu-id="d33e0-129">microsoft.graph.externalConnectors.identitySourceType</span></span>      | <span data-ttu-id="d33e0-130">A fonte de identidade à que o membro pertence.</span><span class="sxs-lookup"><span data-stu-id="d33e0-130">The identity source that the member belongs to.</span></span> <span data-ttu-id="d33e0-131">Os valores possíveis são: `azureActiveDirectory`, `external`.</span><span class="sxs-lookup"><span data-stu-id="d33e0-131">Possible values are: `azureActiveDirectory`, `external`.</span></span>                                                                                         |

## <a name="relationships"></a><span data-ttu-id="d33e0-132">Relações</span><span class="sxs-lookup"><span data-stu-id="d33e0-132">Relationships</span></span>

<span data-ttu-id="d33e0-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d33e0-133">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d33e0-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d33e0-134">JSON representation</span></span>

<span data-ttu-id="d33e0-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d33e0-135">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalConnectors.externalGroupMember",
  "openType": false
}
-->

``` json
{
  "id": "String (identifier)",
  "type": "String",
  "identitySource": "String"
}
```
