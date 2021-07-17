---
title: Tipo de recurso externalGroup
description: Representa um grupo externo usado para definir permissões em externalItems adicionados a uma conexão Graph Microsoft.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 3f0c6adbd47d1823b82e19d3fb9a352e26391da9
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467570"
---
# <a name="externalgroup-resource-type"></a><span data-ttu-id="cf6ea-103">Tipo de recurso externalGroup</span><span class="sxs-lookup"><span data-stu-id="cf6ea-103">externalGroup resource type</span></span>

<span data-ttu-id="cf6ea-104">Namespace: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="cf6ea-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf6ea-105">Representa um grupo externo.</span><span class="sxs-lookup"><span data-stu-id="cf6ea-105">Represents an external group.</span></span> <span data-ttu-id="cf6ea-106">Grupos externos (juntamente com Azure Active Directory e grupos) são usados para definir permissões em **externalItems adicionados** a uma conexão microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="cf6ea-106">External groups (along with Azure Active Directory users and groups) are used to set permissions on **externalItems** added to a Microsoft Graph connection.</span></span> <span data-ttu-id="cf6ea-107">Use **externalGroups** para representar grupos não Azure Active Directory ou construções do tipo grupo (como unidades de negócios, Teams e filho on) que determinam a permissão sobre o conteúdo em sua fonte de dados externa.</span><span class="sxs-lookup"><span data-stu-id="cf6ea-107">Use **externalGroups** to represent non-Azure Active Directory groups or group-like constructs (such as Business units, Teams, and son on) that determine permission over the content in your external data source.</span></span>

## <a name="methods"></a><span data-ttu-id="cf6ea-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="cf6ea-108">Methods</span></span>

|<span data-ttu-id="cf6ea-109">Método</span><span class="sxs-lookup"><span data-stu-id="cf6ea-109">Method</span></span>|<span data-ttu-id="cf6ea-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="cf6ea-110">Return type</span></span>|<span data-ttu-id="cf6ea-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf6ea-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cf6ea-112">Criar externalGroup</span><span class="sxs-lookup"><span data-stu-id="cf6ea-112">Create externalGroup</span></span>](../api/externalconnectors-externalconnection-post-groups.md)|[<span data-ttu-id="cf6ea-113">microsoft.graph.externalConnectors.externalGroup</span><span class="sxs-lookup"><span data-stu-id="cf6ea-113">microsoft.graph.externalConnectors.externalGroup</span></span>](../resources/externalconnectors-externalgroup.md)|<span data-ttu-id="cf6ea-114">Crie um novo **objeto externalGroup.**</span><span class="sxs-lookup"><span data-stu-id="cf6ea-114">Create a new **externalGroup** object.</span></span>|
|[<span data-ttu-id="cf6ea-115">Excluir externalGroup</span><span class="sxs-lookup"><span data-stu-id="cf6ea-115">Delete externalGroup</span></span>](../api/externalconnectors-externalgroup-delete.md)|<span data-ttu-id="cf6ea-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cf6ea-116">None</span></span>|<span data-ttu-id="cf6ea-117">**Exclua um objeto externalGroup.**</span><span class="sxs-lookup"><span data-stu-id="cf6ea-117">Delete an **externalGroup** object.</span></span>|
|[<span data-ttu-id="cf6ea-118">Criar membros</span><span class="sxs-lookup"><span data-stu-id="cf6ea-118">Create members</span></span>](../api/externalconnectors-externalgroup-post-members.md)|[<span data-ttu-id="cf6ea-119">microsoft.graph.externalConnectors.externalGroupMember</span><span class="sxs-lookup"><span data-stu-id="cf6ea-119">microsoft.graph.externalConnectors.externalGroupMember</span></span>](../resources/externalconnectors-externalgroupmember.md)|<span data-ttu-id="cf6ea-120">Crie um novo **objeto externalGroupMember.**</span><span class="sxs-lookup"><span data-stu-id="cf6ea-120">Create a new **externalGroupMember** object.</span></span>|

## <a name="properties"></a><span data-ttu-id="cf6ea-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cf6ea-121">Properties</span></span>

| <span data-ttu-id="cf6ea-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cf6ea-122">Property</span></span>    | <span data-ttu-id="cf6ea-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="cf6ea-123">Type</span></span>   | <span data-ttu-id="cf6ea-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf6ea-124">Description</span></span>                                                                                                              |
|:------------|:-------|:-------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="cf6ea-125">id</span><span class="sxs-lookup"><span data-stu-id="cf6ea-125">id</span></span>          | <span data-ttu-id="cf6ea-126">String</span><span class="sxs-lookup"><span data-stu-id="cf6ea-126">String</span></span> | <span data-ttu-id="cf6ea-127">A ID exclusiva do grupo externo dentro de uma conexão.</span><span class="sxs-lookup"><span data-stu-id="cf6ea-127">The unique ID of the external group within a connection.</span></span> <span data-ttu-id="cf6ea-128">Ele deve ser alfanumérico e pode ter até 128 caracteres.</span><span class="sxs-lookup"><span data-stu-id="cf6ea-128">It must be alphanumeric and can be up to 128 characters long.</span></span> |
| <span data-ttu-id="cf6ea-129">displayName</span><span class="sxs-lookup"><span data-stu-id="cf6ea-129">displayName</span></span> | <span data-ttu-id="cf6ea-130">String</span><span class="sxs-lookup"><span data-stu-id="cf6ea-130">String</span></span> | <span data-ttu-id="cf6ea-131">O nome amigável do grupo externo.</span><span class="sxs-lookup"><span data-stu-id="cf6ea-131">The friendly name of the external group.</span></span> <span data-ttu-id="cf6ea-132">Opcional.</span><span class="sxs-lookup"><span data-stu-id="cf6ea-132">Optional.</span></span>                                                                       |
| <span data-ttu-id="cf6ea-133">description</span><span class="sxs-lookup"><span data-stu-id="cf6ea-133">description</span></span> | <span data-ttu-id="cf6ea-134">String</span><span class="sxs-lookup"><span data-stu-id="cf6ea-134">String</span></span> | <span data-ttu-id="cf6ea-135">A descrição do grupo externo.</span><span class="sxs-lookup"><span data-stu-id="cf6ea-135">The description of the external group.</span></span> <span data-ttu-id="cf6ea-136">Opcional.</span><span class="sxs-lookup"><span data-stu-id="cf6ea-136">Optional.</span></span>                                                                         

## <a name="relationships"></a><span data-ttu-id="cf6ea-137">Relações</span><span class="sxs-lookup"><span data-stu-id="cf6ea-137">Relationships</span></span>

| <span data-ttu-id="cf6ea-138">Relação</span><span class="sxs-lookup"><span data-stu-id="cf6ea-138">Relationship</span></span> | <span data-ttu-id="cf6ea-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="cf6ea-139">Type</span></span>                                                                  | <span data-ttu-id="cf6ea-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf6ea-140">Description</span></span>                                               |
|:-------------|:----------------------------------------------------------------------|:----------------------------------------------------------|
| <span data-ttu-id="cf6ea-141">membros</span><span class="sxs-lookup"><span data-stu-id="cf6ea-141">members</span></span>      | <span data-ttu-id="cf6ea-142">[Coleção microsoft.graph.externalConnectors.externalGroupMember](../resources/externalconnectors-externalgroupmember.md)</span><span class="sxs-lookup"><span data-stu-id="cf6ea-142">[microsoft.graph.externalConnectors.externalGroupMember](../resources/externalconnectors-externalgroupmember.md) collection</span></span> | <span data-ttu-id="cf6ea-143">Um membro adicionado a **um externalGroup**.</span><span class="sxs-lookup"><span data-stu-id="cf6ea-143">A member added to an **externalGroup**.</span></span> <span data-ttu-id="cf6ea-144">Você pode adicionar Azure Active Directory usuários, Azure Active Directory grupos ou outros **externalGroups** como membros.</span><span class="sxs-lookup"><span data-stu-id="cf6ea-144">You can add Azure Active Directory users, Azure Active Directory groups, or other **externalGroups** as members.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="cf6ea-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cf6ea-145">JSON representation</span></span>

<span data-ttu-id="cf6ea-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cf6ea-146">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalConnectors.externalGroup",
  "openType": false
}
-->

``` json
{
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```
