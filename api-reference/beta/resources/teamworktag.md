---
title: Tipo de recurso teamworkTag
description: Representa uma marca associada a uma equipe.
author: anniecolonna
localization_priority: Normal
ms.prod: teamwork
doc_type: resourcePageType
ms.openlocfilehash: fc732ce340f8ab8a3460c16900c4aff2d381744e
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/22/2021
ms.locfileid: "53059874"
---
# <a name="teamworktag-resource-type"></a><span data-ttu-id="b53b5-103">Tipo de recurso teamworkTag</span><span class="sxs-lookup"><span data-stu-id="b53b5-103">teamworkTag resource type</span></span>

<span data-ttu-id="b53b5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b53b5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b53b5-105">Representa uma marca associada a uma equipe.</span><span class="sxs-lookup"><span data-stu-id="b53b5-105">Represents a tag associated with a team.</span></span> 

<span data-ttu-id="b53b5-106">As marcas fornecem uma maneira flexível para os clientes classificarem usuários ou grupos com base em um atributo comum dentro de uma equipe.</span><span class="sxs-lookup"><span data-stu-id="b53b5-106">Tags provide a flexible way for customers to classify users or groups based on a common attribute within a team.</span></span> <span data-ttu-id="b53b5-107">Por exemplo, uma marca Desempresa, Gerente ou Designer permitirá que os usuários alcancem grupos de pessoas no Teams sem precisar digitar cada nome.</span><span class="sxs-lookup"><span data-stu-id="b53b5-107">For example, a Nurse or Manager or Designer tag will enable users to reach groups of people in Teams without having to type every single name.</span></span>

<span data-ttu-id="b53b5-108">Quando uma marca é adicionada, os usuários podem @mention-la em um canal.</span><span class="sxs-lookup"><span data-stu-id="b53b5-108">When a tag is added, users can @mention it in a channel.</span></span> <span data-ttu-id="b53b5-109">Todos os que receberam essa marca receberão uma notificação da mesma forma que receberiam se fossem @mentioned individualmente.</span><span class="sxs-lookup"><span data-stu-id="b53b5-109">Everyone who has been assigned that tag will receive a notification just as they would if they were @mentioned individually.</span></span> <span data-ttu-id="b53b5-110">Os usuários também podem usar uma marca para iniciar um novo chat com os membros dessa marca.</span><span class="sxs-lookup"><span data-stu-id="b53b5-110">Users can also use a tag is to start a new chat with the members of that tag.</span></span>

## <a name="methods"></a><span data-ttu-id="b53b5-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="b53b5-111">Methods</span></span>
|<span data-ttu-id="b53b5-112">Método</span><span class="sxs-lookup"><span data-stu-id="b53b5-112">Method</span></span>|<span data-ttu-id="b53b5-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b53b5-113">Return type</span></span>|<span data-ttu-id="b53b5-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="b53b5-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b53b5-115">Listar teamworkTags</span><span class="sxs-lookup"><span data-stu-id="b53b5-115">List teamworkTags</span></span>](../api/teamworktag-list.md)|<span data-ttu-id="b53b5-116">**coleção teamworkTag**</span><span class="sxs-lookup"><span data-stu-id="b53b5-116">**teamworkTag** collection</span></span>|<span data-ttu-id="b53b5-117">Obter uma lista dos objetos **teamworkTag** e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="b53b5-117">Get a list of the **teamworkTag** objects and their properties.</span></span>|
|[<span data-ttu-id="b53b5-118">Criar teamworkTag</span><span class="sxs-lookup"><span data-stu-id="b53b5-118">Create teamworkTag</span></span>](../api/teamworktag-post.md)|<span data-ttu-id="b53b5-119">**teamworkTag**</span><span class="sxs-lookup"><span data-stu-id="b53b5-119">**teamworkTag**</span></span>|<span data-ttu-id="b53b5-120">Crie um novo **objeto teamworkTag.**</span><span class="sxs-lookup"><span data-stu-id="b53b5-120">Create a new **teamworkTag** object.</span></span>|
|[<span data-ttu-id="b53b5-121">Obter teamworkTag</span><span class="sxs-lookup"><span data-stu-id="b53b5-121">Get teamworkTag</span></span>](../api/teamworktag-get.md)|<span data-ttu-id="b53b5-122">**teamworkTag**</span><span class="sxs-lookup"><span data-stu-id="b53b5-122">**teamworkTag**</span></span>|<span data-ttu-id="b53b5-123">Leia as propriedades e as relações de um **objeto teamworkTag.**</span><span class="sxs-lookup"><span data-stu-id="b53b5-123">Read the properties and relationships of a **teamworkTag** object.</span></span>|
|[<span data-ttu-id="b53b5-124">Atualizar o teamworkTag</span><span class="sxs-lookup"><span data-stu-id="b53b5-124">Update teamworkTag</span></span>](../api/teamworktag-update.md)|<span data-ttu-id="b53b5-125">**teamworkTag**</span><span class="sxs-lookup"><span data-stu-id="b53b5-125">**teamworkTag**</span></span>|<span data-ttu-id="b53b5-126">Atualize as propriedades de um **objeto teamworkTag.**</span><span class="sxs-lookup"><span data-stu-id="b53b5-126">Update the properties of a **teamworkTag** object.</span></span>|
|[<span data-ttu-id="b53b5-127">Excluir teamworkTag</span><span class="sxs-lookup"><span data-stu-id="b53b5-127">Delete teamworkTag</span></span>](../api/teamworktag-delete.md)|<span data-ttu-id="b53b5-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b53b5-128">None</span></span>|<span data-ttu-id="b53b5-129">Excluir um **objeto teamworkTag.**</span><span class="sxs-lookup"><span data-stu-id="b53b5-129">Delete a **teamworkTag** object.</span></span>|
|[<span data-ttu-id="b53b5-130">Listar o trabalho em equipeTagMembers</span><span class="sxs-lookup"><span data-stu-id="b53b5-130">List teamworkTagMembers</span></span>](../api/teamworktagmember-list.md)|<span data-ttu-id="b53b5-131">**coleção teamworkTagMember**</span><span class="sxs-lookup"><span data-stu-id="b53b5-131">**teamworkTagMember** collection</span></span>|<span data-ttu-id="b53b5-132">Obter uma lista dos membros de uma marca padrão em uma equipe e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="b53b5-132">Get a list of the members of a standard tag in a team and their properties.</span></span>|
|[<span data-ttu-id="b53b5-133">Obter trabalho em equipeTagMember</span><span class="sxs-lookup"><span data-stu-id="b53b5-133">Get teamworkTagMember</span></span>](../api/teamworktagmember-get.md)|<span data-ttu-id="b53b5-134">**teamworkTagMember**</span><span class="sxs-lookup"><span data-stu-id="b53b5-134">**teamworkTagMember**</span></span>|<span data-ttu-id="b53b5-135">Obter as propriedades e as relações de um membro de uma marca padrão em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="b53b5-135">Get the properties and relationships of a member of a standard tag in a team.</span></span>|
|[<span data-ttu-id="b53b5-136">Excluir o trabalho em equipeTagMember</span><span class="sxs-lookup"><span data-stu-id="b53b5-136">Delete teamworkTagMember</span></span>](../api/teamworktagmember-delete.md)|<span data-ttu-id="b53b5-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b53b5-137">None</span></span>|<span data-ttu-id="b53b5-138">Exclua um membro de uma marca padrão na equipe.</span><span class="sxs-lookup"><span data-stu-id="b53b5-138">Delete a member from a standard tag in the team.</span></span>|

## <a name="properties"></a><span data-ttu-id="b53b5-139">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b53b5-139">Properties</span></span>
|<span data-ttu-id="b53b5-140">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b53b5-140">Property</span></span>|<span data-ttu-id="b53b5-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="b53b5-141">Type</span></span>|<span data-ttu-id="b53b5-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="b53b5-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b53b5-143">description</span><span class="sxs-lookup"><span data-stu-id="b53b5-143">description</span></span>|<span data-ttu-id="b53b5-144">String</span><span class="sxs-lookup"><span data-stu-id="b53b5-144">String</span></span>|<span data-ttu-id="b53b5-145">Descrição da marca como ela aparecerá para o usuário em Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="b53b5-145">Tag description as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="b53b5-146">displayName</span><span class="sxs-lookup"><span data-stu-id="b53b5-146">displayName</span></span>|<span data-ttu-id="b53b5-147">String</span><span class="sxs-lookup"><span data-stu-id="b53b5-147">String</span></span>|<span data-ttu-id="b53b5-148">Nome da marca como ele aparecerá para o usuário em Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="b53b5-148">Tag name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="b53b5-149">id</span><span class="sxs-lookup"><span data-stu-id="b53b5-149">id</span></span>|<span data-ttu-id="b53b5-150">String</span><span class="sxs-lookup"><span data-stu-id="b53b5-150">String</span></span>|<span data-ttu-id="b53b5-151">ID da marca.</span><span class="sxs-lookup"><span data-stu-id="b53b5-151">ID of the tag.</span></span>|
|<span data-ttu-id="b53b5-152">memberCount</span><span class="sxs-lookup"><span data-stu-id="b53b5-152">memberCount</span></span>|<span data-ttu-id="b53b5-153">Int32</span><span class="sxs-lookup"><span data-stu-id="b53b5-153">Int32</span></span>|<span data-ttu-id="b53b5-154">O número de usuários atribuídos à marca.</span><span class="sxs-lookup"><span data-stu-id="b53b5-154">The number of users assigned to the tag.</span></span>|
|<span data-ttu-id="b53b5-155">tagType</span><span class="sxs-lookup"><span data-stu-id="b53b5-155">tagType</span></span>|<span data-ttu-id="b53b5-156">teamworkTagType</span><span class="sxs-lookup"><span data-stu-id="b53b5-156">teamworkTagType</span></span>|<span data-ttu-id="b53b5-157">O tipo de marca.</span><span class="sxs-lookup"><span data-stu-id="b53b5-157">The type of tag.</span></span> <span data-ttu-id="b53b5-158">O padrão é padrão.</span><span class="sxs-lookup"><span data-stu-id="b53b5-158">Default is standard.</span></span>|
|<span data-ttu-id="b53b5-159">teamId</span><span class="sxs-lookup"><span data-stu-id="b53b5-159">teamId</span></span>|<span data-ttu-id="b53b5-160">String</span><span class="sxs-lookup"><span data-stu-id="b53b5-160">String</span></span>|<span data-ttu-id="b53b5-161">ID da equipe na qual a marca é definida.</span><span class="sxs-lookup"><span data-stu-id="b53b5-161">ID of the team in which the tag is defined.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b53b5-162">Relações</span><span class="sxs-lookup"><span data-stu-id="b53b5-162">Relationships</span></span>
|<span data-ttu-id="b53b5-163">Relação</span><span class="sxs-lookup"><span data-stu-id="b53b5-163">Relationship</span></span>|<span data-ttu-id="b53b5-164">Tipo</span><span class="sxs-lookup"><span data-stu-id="b53b5-164">Type</span></span>|<span data-ttu-id="b53b5-165">Descrição</span><span class="sxs-lookup"><span data-stu-id="b53b5-165">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b53b5-166">membros</span><span class="sxs-lookup"><span data-stu-id="b53b5-166">members</span></span>|<span data-ttu-id="b53b5-167">[coleção teamworkTagMember](../resources/teamworktagmember.md)</span><span class="sxs-lookup"><span data-stu-id="b53b5-167">[teamworkTagMember](../resources/teamworktagmember.md) collection</span></span>|<span data-ttu-id="b53b5-168">Usuários atribuídos à marca.</span><span class="sxs-lookup"><span data-stu-id="b53b5-168">Users assigned to the tag.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b53b5-169">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b53b5-169">JSON representation</span></span>
<span data-ttu-id="b53b5-170">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b53b5-170">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamworkTag",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkTag",
  "id": "String (identifier)",
  "teamId": "String",
  "displayName": "String",
  "memberCount": "Integer",
  "tagType": "String"
}
```

