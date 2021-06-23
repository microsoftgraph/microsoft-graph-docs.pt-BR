---
title: Tipo de recurso teamworkTagMember
description: Representa um usuário em uma equipe que tem uma marca aplicada a ele.
author: anniecolonna
localization_priority: Normal
ms.prod: teamwork
doc_type: resourcePageType
ms.openlocfilehash: 73666dd19720e6d8882bb16fd90c612097e41d10
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/22/2021
ms.locfileid: "53059870"
---
# <a name="teamworktagmember-resource-type"></a><span data-ttu-id="d03de-103">Tipo de recurso teamworkTagMember</span><span class="sxs-lookup"><span data-stu-id="d03de-103">teamworkTagMember resource type</span></span>

<span data-ttu-id="d03de-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d03de-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d03de-105">Representa um usuário em uma equipe à qual uma marca é aplicada.</span><span class="sxs-lookup"><span data-stu-id="d03de-105">Represents a user in a team to whom a tag is applied.</span></span>

## <a name="methods"></a><span data-ttu-id="d03de-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="d03de-106">Methods</span></span>
|<span data-ttu-id="d03de-107">Método</span><span class="sxs-lookup"><span data-stu-id="d03de-107">Method</span></span>|<span data-ttu-id="d03de-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d03de-108">Return type</span></span>|<span data-ttu-id="d03de-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d03de-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d03de-110">Listar o trabalho em equipeTagMembers</span><span class="sxs-lookup"><span data-stu-id="d03de-110">List teamworkTagMembers</span></span>](../api/teamworktagmember-list.md)|<span data-ttu-id="d03de-111">**coleção teamworkTagMember**</span><span class="sxs-lookup"><span data-stu-id="d03de-111">**teamworkTagMember** collection</span></span>|<span data-ttu-id="d03de-112">Obter uma lista dos membros de uma marca padrão em uma equipe e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="d03de-112">Get a list of the members of a standard tag in a team and their properties.</span></span>|
|[<span data-ttu-id="d03de-113">Obter trabalho em equipeTagMember</span><span class="sxs-lookup"><span data-stu-id="d03de-113">Get teamworkTagMember</span></span>](../api/teamworktagmember-get.md)|<span data-ttu-id="d03de-114">**teamworkTagMember**</span><span class="sxs-lookup"><span data-stu-id="d03de-114">**teamworkTagMember**</span></span>|<span data-ttu-id="d03de-115">Obter as propriedades e as relações de um membro de uma marca padrão em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="d03de-115">Get the properties and relationships of a member of a standard tag in a team.</span></span>|
|[<span data-ttu-id="d03de-116">Excluir o trabalho em equipeTagMember</span><span class="sxs-lookup"><span data-stu-id="d03de-116">Delete teamworkTagMember</span></span>](../api/teamworktagmember-delete.md)|<span data-ttu-id="d03de-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d03de-117">None</span></span>|<span data-ttu-id="d03de-118">Exclua um membro de uma marca padrão na equipe.</span><span class="sxs-lookup"><span data-stu-id="d03de-118">Delete a member from a standard tag in the team.</span></span>|

## <a name="properties"></a><span data-ttu-id="d03de-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d03de-119">Properties</span></span>
|<span data-ttu-id="d03de-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d03de-120">Property</span></span>|<span data-ttu-id="d03de-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="d03de-121">Type</span></span>|<span data-ttu-id="d03de-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d03de-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d03de-123">displayName</span><span class="sxs-lookup"><span data-stu-id="d03de-123">displayName</span></span>|<span data-ttu-id="d03de-124">String</span><span class="sxs-lookup"><span data-stu-id="d03de-124">String</span></span>|<span data-ttu-id="d03de-125">O nome de exibição do membro.</span><span class="sxs-lookup"><span data-stu-id="d03de-125">The member's display name.</span></span>|
|<span data-ttu-id="d03de-126">ID</span><span class="sxs-lookup"><span data-stu-id="d03de-126">ID</span></span>|<span data-ttu-id="d03de-127">String</span><span class="sxs-lookup"><span data-stu-id="d03de-127">String</span></span>|<span data-ttu-id="d03de-128">ID do membro.</span><span class="sxs-lookup"><span data-stu-id="d03de-128">ID of the member.</span></span>|
|<span data-ttu-id="d03de-129">tenantID</span><span class="sxs-lookup"><span data-stu-id="d03de-129">tenantID</span></span>|<span data-ttu-id="d03de-130">String</span><span class="sxs-lookup"><span data-stu-id="d03de-130">String</span></span>|<span data-ttu-id="d03de-131">A ID do locatário do que o membro da marca faz parte.</span><span class="sxs-lookup"><span data-stu-id="d03de-131">The ID of the tenant that the tag member is a part of.</span></span>|
|<span data-ttu-id="d03de-132">userID</span><span class="sxs-lookup"><span data-stu-id="d03de-132">userID</span></span>|<span data-ttu-id="d03de-133">String</span><span class="sxs-lookup"><span data-stu-id="d03de-133">String</span></span>|<span data-ttu-id="d03de-134">A ID do usuário do membro.</span><span class="sxs-lookup"><span data-stu-id="d03de-134">The user ID of the member.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d03de-135">Relações</span><span class="sxs-lookup"><span data-stu-id="d03de-135">Relationships</span></span>
<span data-ttu-id="d03de-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d03de-136">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d03de-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d03de-137">JSON representation</span></span>
<span data-ttu-id="d03de-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d03de-138">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "ID",
  "@odata.type": "microsoft.graph.teamworkTagMember",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkTagMember",
  "ID": "String (Identifier)",
  "displayName": "String",
  "tenantID": "String",
  "userID": "String"
}
```

