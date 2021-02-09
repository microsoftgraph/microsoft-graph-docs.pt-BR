---
title: Tipo de recurso externalGroupMember
description: Representa um membro de um externalGroup usado para definir permissões em conteúdo externo adicionado ao Microsoft Graph.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 1e86fb275b941b7a3033999fedd4c71aa3ac1de1
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161688"
---
# <a name="externalgroupmember-resource-type"></a><span data-ttu-id="828eb-103">Tipo de recurso externalGroupMember</span><span class="sxs-lookup"><span data-stu-id="828eb-103">externalGroupMember resource type</span></span>

<span data-ttu-id="828eb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="828eb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="828eb-105">Representa um membro de um [externalGroup](externalgroup.md) usado para definir permissões em conteúdo externo adicionado ao Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="828eb-105">Represents a member of an [externalGroup](externalgroup.md) used to set permissions on external content added to Microsoft Graph.</span></span>

## <a name="methods"></a><span data-ttu-id="828eb-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="828eb-106">Methods</span></span>

| <span data-ttu-id="828eb-107">Método</span><span class="sxs-lookup"><span data-stu-id="828eb-107">Method</span></span>                                                              | <span data-ttu-id="828eb-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="828eb-108">Return type</span></span>         | <span data-ttu-id="828eb-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="828eb-109">Description</span></span>                              |
|:--------------------------------------------------------------------|:--------------------|:-----------------------------------------|
| [<span data-ttu-id="828eb-110">Criar externalGroupMember</span><span class="sxs-lookup"><span data-stu-id="828eb-110">Create externalGroupMember</span></span>](../api/externalgroup-post-members.md) | <span data-ttu-id="828eb-111">externalGroupMember</span><span class="sxs-lookup"><span data-stu-id="828eb-111">externalGroupMember</span></span> | <span data-ttu-id="828eb-112">Criar um novo **objeto externalGroupMember.**</span><span class="sxs-lookup"><span data-stu-id="828eb-112">Create a new **externalGroupMember** object.</span></span> |
| [<span data-ttu-id="828eb-113">Excluir externalGroupMember</span><span class="sxs-lookup"><span data-stu-id="828eb-113">Delete externalGroupMember</span></span>](../api/externalgroupmember-delete.md)  | <span data-ttu-id="828eb-114">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="828eb-114">None</span></span>                | <span data-ttu-id="828eb-115">**Exclua um objeto externalGroupMember.**</span><span class="sxs-lookup"><span data-stu-id="828eb-115">Delete an **externalGroupMember** object.</span></span>   |

## <a name="properties"></a><span data-ttu-id="828eb-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="828eb-116">Properties</span></span>

| <span data-ttu-id="828eb-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="828eb-117">Property</span></span>       | <span data-ttu-id="828eb-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="828eb-118">Type</span></span>                    | <span data-ttu-id="828eb-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="828eb-119">Description</span></span>                                                          |
|:---------------|:------------------------|:---------------------------------------------------------------------|
| <span data-ttu-id="828eb-120">id</span><span class="sxs-lookup"><span data-stu-id="828eb-120">id</span></span>             | <span data-ttu-id="828eb-121">String</span><span class="sxs-lookup"><span data-stu-id="828eb-121">String</span></span>                  | <span data-ttu-id="828eb-122">A ID exclusiva do membro.</span><span class="sxs-lookup"><span data-stu-id="828eb-122">The unique ID of the member.</span></span> <span data-ttu-id="828eb-123">Seria o objectId no caso de usuários ou grupos do Azure Active Directory e a propriedade **de id** do **externalGroup** no caso de grupos externos.</span><span class="sxs-lookup"><span data-stu-id="828eb-123">It would be the objectId in case of Azure Active Directory users or groups and the **id** property of the **externalGroup** in case of external groups.</span></span>                                    |
| <span data-ttu-id="828eb-124">type</span><span class="sxs-lookup"><span data-stu-id="828eb-124">type</span></span>           | <span data-ttu-id="828eb-125">externalGroupMemberType</span><span class="sxs-lookup"><span data-stu-id="828eb-125">externalGroupMemberType</span></span> | <span data-ttu-id="828eb-126">O tipo de membro adicionado ao grupo externo.</span><span class="sxs-lookup"><span data-stu-id="828eb-126">The type of member added to the external group.</span></span> <span data-ttu-id="828eb-127">Os valores `user` possíveis são: `group` ou quando **identitySource** é `azureActiveDirectory` e apenas quando `group` **identitySource** é `external` .</span><span class="sxs-lookup"><span data-stu-id="828eb-127">Possible values are: `user` or `group` when the **identitySource** is `azureActiveDirectory` and just `group` when the **identitySource** is `external`.</span></span> |
| <span data-ttu-id="828eb-128">identitySource</span><span class="sxs-lookup"><span data-stu-id="828eb-128">identitySource</span></span> | <span data-ttu-id="828eb-129">identitySourceType</span><span class="sxs-lookup"><span data-stu-id="828eb-129">identitySourceType</span></span>      | <span data-ttu-id="828eb-130">A fonte de identidade à que o membro pertence.</span><span class="sxs-lookup"><span data-stu-id="828eb-130">The identity source that the member belongs to.</span></span> <span data-ttu-id="828eb-131">Os valores possíveis são: `azureActiveDirectory`, `external`.</span><span class="sxs-lookup"><span data-stu-id="828eb-131">Possible values are: `azureActiveDirectory`, `external`.</span></span>                                                                                         |

## <a name="relationships"></a><span data-ttu-id="828eb-132">Relações</span><span class="sxs-lookup"><span data-stu-id="828eb-132">Relationships</span></span>

<span data-ttu-id="828eb-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="828eb-133">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="828eb-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="828eb-134">JSON representation</span></span>

<span data-ttu-id="828eb-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="828eb-135">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalGroupMember",
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
