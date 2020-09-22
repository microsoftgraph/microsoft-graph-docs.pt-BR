---
title: tipo de recurso de interexternal
description: Representa um grupo externo usado para definir permissões no externalItems adicionado a uma conexão do Microsoft Graph.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: c258df9e6f20cf7a19e291fd298ad66345a72949
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193811"
---
# <a name="externalgroup-resource-type"></a><span data-ttu-id="170fb-103">tipo de recurso de interexternal</span><span class="sxs-lookup"><span data-stu-id="170fb-103">externalGroup resource type</span></span>

<span data-ttu-id="170fb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="170fb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="170fb-105">Representa um grupo externo.</span><span class="sxs-lookup"><span data-stu-id="170fb-105">Represents an external group.</span></span> <span data-ttu-id="170fb-106">Grupos externos (juntamente com usuários e grupos do Azure Active Directory) são usados para definir permissões no **externalItems** adicionado a uma conexão do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="170fb-106">External groups (along with Azure Active Directory users and groups) are used to set permissions on **externalItems** added to a Microsoft Graph connection.</span></span> <span data-ttu-id="170fb-107">Use o **externalGroups** para representar grupos do Active Directory do Azure ou construções do tipo grupo (como unidades de negócios, equipes e filho) que determinam a permissão sobre o conteúdo da sua fonte de dados externa.</span><span class="sxs-lookup"><span data-stu-id="170fb-107">Use **externalGroups** to represent non-Azure Active Directory groups or group-like constructs (such as Business units, Teams, and son on) that determine permission over the content in your external data source.</span></span>

## <a name="methods"></a><span data-ttu-id="170fb-108">Methods</span><span class="sxs-lookup"><span data-stu-id="170fb-108">Methods</span></span>

|<span data-ttu-id="170fb-109">Método</span><span class="sxs-lookup"><span data-stu-id="170fb-109">Method</span></span>|<span data-ttu-id="170fb-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="170fb-110">Return type</span></span>|<span data-ttu-id="170fb-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="170fb-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="170fb-112">Criar um</span><span class="sxs-lookup"><span data-stu-id="170fb-112">Create externalGroup</span></span>](../api/externalconnection-post-groups.md)|[<span data-ttu-id="170fb-113">externa</span><span class="sxs-lookup"><span data-stu-id="170fb-113">externalGroup</span></span>](../resources/externalgroup.md)|<span data-ttu-id="170fb-114">Criar um novo objeto de objeto **externo** .</span><span class="sxs-lookup"><span data-stu-id="170fb-114">Create a new **externalGroup** object.</span></span>|
|[<span data-ttu-id="170fb-115">Excluir o external</span><span class="sxs-lookup"><span data-stu-id="170fb-115">Delete externalGroup</span></span>](../api/externalgroup-delete.md)|<span data-ttu-id="170fb-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="170fb-116">None</span></span>|<span data-ttu-id="170fb-117">Excluir um **objeto** de um.</span><span class="sxs-lookup"><span data-stu-id="170fb-117">Delete an **externalGroup** object.</span></span>|
|[<span data-ttu-id="170fb-118">Criar membros</span><span class="sxs-lookup"><span data-stu-id="170fb-118">Create members</span></span>](../api/externalgroup-post-members.md)|[<span data-ttu-id="170fb-119">externalGroupMember</span><span class="sxs-lookup"><span data-stu-id="170fb-119">externalGroupMember</span></span>](../resources/externalgroupmember.md)|<span data-ttu-id="170fb-120">Criar um novo objeto **externalGroupMember** .</span><span class="sxs-lookup"><span data-stu-id="170fb-120">Create a new **externalGroupMember** object.</span></span>|

## <a name="properties"></a><span data-ttu-id="170fb-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="170fb-121">Properties</span></span>

| <span data-ttu-id="170fb-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="170fb-122">Property</span></span>    | <span data-ttu-id="170fb-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="170fb-123">Type</span></span>   | <span data-ttu-id="170fb-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="170fb-124">Description</span></span>                                                                                                              |
|:------------|:-------|:-------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="170fb-125">id</span><span class="sxs-lookup"><span data-stu-id="170fb-125">id</span></span>          | <span data-ttu-id="170fb-126">String</span><span class="sxs-lookup"><span data-stu-id="170fb-126">String</span></span> | <span data-ttu-id="170fb-127">A identificação exclusiva do grupo externo em uma conexão.</span><span class="sxs-lookup"><span data-stu-id="170fb-127">The unique ID of the external group within a connection.</span></span> <span data-ttu-id="170fb-128">Ele deve ser alfanumérico e até 128 caracteres de comprimento.</span><span class="sxs-lookup"><span data-stu-id="170fb-128">It must be alphanumeric and can be up to 128 characters long.</span></span> |
| <span data-ttu-id="170fb-129">displayName</span><span class="sxs-lookup"><span data-stu-id="170fb-129">displayName</span></span> | <span data-ttu-id="170fb-130">String</span><span class="sxs-lookup"><span data-stu-id="170fb-130">String</span></span> | <span data-ttu-id="170fb-131">O nome amigável do grupo externo.</span><span class="sxs-lookup"><span data-stu-id="170fb-131">The friendly name of the external group.</span></span> <span data-ttu-id="170fb-132">Opcional.</span><span class="sxs-lookup"><span data-stu-id="170fb-132">Optional.</span></span>                                                                       |
| <span data-ttu-id="170fb-133">description</span><span class="sxs-lookup"><span data-stu-id="170fb-133">description</span></span> | <span data-ttu-id="170fb-134">String</span><span class="sxs-lookup"><span data-stu-id="170fb-134">String</span></span> | <span data-ttu-id="170fb-135">A descrição do grupo externo.</span><span class="sxs-lookup"><span data-stu-id="170fb-135">The description of the external group.</span></span> <span data-ttu-id="170fb-136">Opcional.</span><span class="sxs-lookup"><span data-stu-id="170fb-136">Optional.</span></span>                                                                         

## <a name="relationships"></a><span data-ttu-id="170fb-137">Relações</span><span class="sxs-lookup"><span data-stu-id="170fb-137">Relationships</span></span>

| <span data-ttu-id="170fb-138">Relação</span><span class="sxs-lookup"><span data-stu-id="170fb-138">Relationship</span></span> | <span data-ttu-id="170fb-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="170fb-139">Type</span></span>                                                                  | <span data-ttu-id="170fb-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="170fb-140">Description</span></span>                                               |
|:-------------|:----------------------------------------------------------------------|:----------------------------------------------------------|
| <span data-ttu-id="170fb-141">membros</span><span class="sxs-lookup"><span data-stu-id="170fb-141">members</span></span>      | <span data-ttu-id="170fb-142">coleção [externalGroupMember](../resources/externalgroupmember.md)</span><span class="sxs-lookup"><span data-stu-id="170fb-142">[externalGroupMember](../resources/externalgroupmember.md) collection</span></span> | <span data-ttu-id="170fb-143">Um membro adicionado a uma **myexterna**.</span><span class="sxs-lookup"><span data-stu-id="170fb-143">A member added to an **externalGroup**.</span></span> <span data-ttu-id="170fb-144">Você pode adicionar usuários do Azure Active Directory, grupos do Azure Active Directory ou outros **externalGroups** como membros.</span><span class="sxs-lookup"><span data-stu-id="170fb-144">You can add Azure Active Directory users, Azure Active Directory groups, or other **externalGroups** as members.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="170fb-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="170fb-145">JSON representation</span></span>

<span data-ttu-id="170fb-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="170fb-146">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalGroup",
  "baseType": "",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.externalGroup",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```
