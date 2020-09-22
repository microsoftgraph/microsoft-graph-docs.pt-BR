---
title: tipo de recurso externalGroupMember
description: Representa um membro de um grupo externo usado para definir permissões no conteúdo externo adicionado ao Microsoft Graph.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 19b5c5094501215cc3ffd3e852ba6ca427807988
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193810"
---
# <a name="externalgroupmember-resource-type"></a><span data-ttu-id="83d53-103">tipo de recurso externalGroupMember</span><span class="sxs-lookup"><span data-stu-id="83d53-103">externalGroupMember resource type</span></span>

<span data-ttu-id="83d53-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83d53-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83d53-105">Representa um membro de um grupo [externo](externalgroup.md) usado para definir permissões no conteúdo externo adicionado ao Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="83d53-105">Represents a member of an [externalGroup](externalgroup.md) used to set permissions on external content added to Microsoft Graph.</span></span>

## <a name="methods"></a><span data-ttu-id="83d53-106">Methods</span><span class="sxs-lookup"><span data-stu-id="83d53-106">Methods</span></span>

| <span data-ttu-id="83d53-107">Método</span><span class="sxs-lookup"><span data-stu-id="83d53-107">Method</span></span>                                                              | <span data-ttu-id="83d53-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="83d53-108">Return type</span></span>         | <span data-ttu-id="83d53-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="83d53-109">Description</span></span>                              |
|:--------------------------------------------------------------------|:--------------------|:-----------------------------------------|
| [<span data-ttu-id="83d53-110">Criar externalGroupMember</span><span class="sxs-lookup"><span data-stu-id="83d53-110">Create externalGroupMember</span></span>](../api/externalgroup-post-members.md) | <span data-ttu-id="83d53-111">externalGroupMember</span><span class="sxs-lookup"><span data-stu-id="83d53-111">externalGroupMember</span></span> | <span data-ttu-id="83d53-112">Criar um novo objeto **externalGroupMember** .</span><span class="sxs-lookup"><span data-stu-id="83d53-112">Create a new **externalGroupMember** object.</span></span> |
| [<span data-ttu-id="83d53-113">Excluir externalGroupMember</span><span class="sxs-lookup"><span data-stu-id="83d53-113">Delete externalGroupMember</span></span>](../api/externalgroupmember-delete.md)  | <span data-ttu-id="83d53-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="83d53-114">None</span></span>                | <span data-ttu-id="83d53-115">Excluir um objeto **externalGroupMember** .</span><span class="sxs-lookup"><span data-stu-id="83d53-115">Delete an **externalGroupMember** object.</span></span>   |

## <a name="properties"></a><span data-ttu-id="83d53-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="83d53-116">Properties</span></span>

| <span data-ttu-id="83d53-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="83d53-117">Property</span></span>       | <span data-ttu-id="83d53-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="83d53-118">Type</span></span>                    | <span data-ttu-id="83d53-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="83d53-119">Description</span></span>                                                          |
|:---------------|:------------------------|:---------------------------------------------------------------------|
| <span data-ttu-id="83d53-120">id</span><span class="sxs-lookup"><span data-stu-id="83d53-120">id</span></span>             | <span data-ttu-id="83d53-121">String</span><span class="sxs-lookup"><span data-stu-id="83d53-121">String</span></span>                  | <span data-ttu-id="83d53-122">A identificação exclusiva do membro.</span><span class="sxs-lookup"><span data-stu-id="83d53-122">The unique ID of the member.</span></span> <span data-ttu-id="83d53-123">Seria o objectId em caso de usuários ou grupos do Active Directory do Azure e a propriedade **ID** do grupo **externo** no caso de grupos externos.</span><span class="sxs-lookup"><span data-stu-id="83d53-123">It would be the objectId in case of Azure Active Directory users or groups and the **id** property of the **externalGroup** in case of external groups.</span></span>                                    |
| <span data-ttu-id="83d53-124">tipo</span><span class="sxs-lookup"><span data-stu-id="83d53-124">type</span></span>           | <span data-ttu-id="83d53-125">externalGroupMemberType</span><span class="sxs-lookup"><span data-stu-id="83d53-125">externalGroupMemberType</span></span> | <span data-ttu-id="83d53-126">O tipo de membro adicionado ao grupo externo.</span><span class="sxs-lookup"><span data-stu-id="83d53-126">The type of member added to the external group.</span></span> <span data-ttu-id="83d53-127">Os valores possíveis são: `user` ou `group` quando **IdentityName** é `azureActiveDirectory` e apenas `group` quando **IdentityName** é `external` .</span><span class="sxs-lookup"><span data-stu-id="83d53-127">Possible values are: `user` or `group` when the **identitySource** is `azureActiveDirectory` and just `group` when the **identitySource** is `external`.</span></span> |
| <span data-ttu-id="83d53-128">identificação da identidade</span><span class="sxs-lookup"><span data-stu-id="83d53-128">identitySource</span></span> | <span data-ttu-id="83d53-129">identitySourceType</span><span class="sxs-lookup"><span data-stu-id="83d53-129">identitySourceType</span></span>      | <span data-ttu-id="83d53-130">A origem de identidade à qual o membro pertence.</span><span class="sxs-lookup"><span data-stu-id="83d53-130">The identity source that the member belongs to.</span></span> <span data-ttu-id="83d53-131">Os valores possíveis são: `azureActiveDirectory`, `external`.</span><span class="sxs-lookup"><span data-stu-id="83d53-131">Possible values are: `azureActiveDirectory`, `external`.</span></span>                                                                                         |

## <a name="relationships"></a><span data-ttu-id="83d53-132">Relações</span><span class="sxs-lookup"><span data-stu-id="83d53-132">Relationships</span></span>

<span data-ttu-id="83d53-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="83d53-133">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="83d53-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="83d53-134">JSON representation</span></span>

<span data-ttu-id="83d53-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="83d53-135">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalGroupMember",
  "baseType": "",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.externalGroupMember",
  "id": "String (identifier)",
  "type": "String",
  "identitySource": "String"
}
```
