---
title: Tipo de recurso externalGroup
description: Representa um grupo externo usado para definir permissões em externalItems adicionados a uma conexão do Microsoft Graph.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 2e9d8e3a605f1c3df39b13607f82e7541d59e62e
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161697"
---
# <a name="externalgroup-resource-type"></a><span data-ttu-id="c5d19-103">Tipo de recurso externalGroup</span><span class="sxs-lookup"><span data-stu-id="c5d19-103">externalGroup resource type</span></span>

<span data-ttu-id="c5d19-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5d19-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5d19-105">Representa um grupo externo.</span><span class="sxs-lookup"><span data-stu-id="c5d19-105">Represents an external group.</span></span> <span data-ttu-id="c5d19-106">Grupos externos (juntamente com usuários e grupos do Azure Active Directory) são usados para definir permissões em **externalItems adicionados** a uma conexão do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c5d19-106">External groups (along with Azure Active Directory users and groups) are used to set permissions on **externalItems** added to a Microsoft Graph connection.</span></span> <span data-ttu-id="c5d19-107">Use **externalGroups** para representar grupos do Active Directory não Azure ou construções do tipo grupo (como unidades de negócios, Teams e es) que determinam a permissão sobre o conteúdo em sua fonte de dados externa.</span><span class="sxs-lookup"><span data-stu-id="c5d19-107">Use **externalGroups** to represent non-Azure Active Directory groups or group-like constructs (such as Business units, Teams, and son on) that determine permission over the content in your external data source.</span></span>

## <a name="methods"></a><span data-ttu-id="c5d19-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="c5d19-108">Methods</span></span>

|<span data-ttu-id="c5d19-109">Método</span><span class="sxs-lookup"><span data-stu-id="c5d19-109">Method</span></span>|<span data-ttu-id="c5d19-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c5d19-110">Return type</span></span>|<span data-ttu-id="c5d19-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5d19-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c5d19-112">Criar externalGroup</span><span class="sxs-lookup"><span data-stu-id="c5d19-112">Create externalGroup</span></span>](../api/externalconnection-post-groups.md)|[<span data-ttu-id="c5d19-113">externalGroup</span><span class="sxs-lookup"><span data-stu-id="c5d19-113">externalGroup</span></span>](../resources/externalgroup.md)|<span data-ttu-id="c5d19-114">Criar um novo **objeto externalGroup.**</span><span class="sxs-lookup"><span data-stu-id="c5d19-114">Create a new **externalGroup** object.</span></span>|
|[<span data-ttu-id="c5d19-115">Excluir externalGroup</span><span class="sxs-lookup"><span data-stu-id="c5d19-115">Delete externalGroup</span></span>](../api/externalgroup-delete.md)|<span data-ttu-id="c5d19-116">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="c5d19-116">None</span></span>|<span data-ttu-id="c5d19-117">**Exclua um objeto externalGroup.**</span><span class="sxs-lookup"><span data-stu-id="c5d19-117">Delete an **externalGroup** object.</span></span>|
|[<span data-ttu-id="c5d19-118">Criar membros</span><span class="sxs-lookup"><span data-stu-id="c5d19-118">Create members</span></span>](../api/externalgroup-post-members.md)|[<span data-ttu-id="c5d19-119">externalGroupMember</span><span class="sxs-lookup"><span data-stu-id="c5d19-119">externalGroupMember</span></span>](../resources/externalgroupmember.md)|<span data-ttu-id="c5d19-120">Criar um novo **objeto externalGroupMember.**</span><span class="sxs-lookup"><span data-stu-id="c5d19-120">Create a new **externalGroupMember** object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c5d19-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c5d19-121">Properties</span></span>

| <span data-ttu-id="c5d19-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c5d19-122">Property</span></span>    | <span data-ttu-id="c5d19-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="c5d19-123">Type</span></span>   | <span data-ttu-id="c5d19-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5d19-124">Description</span></span>                                                                                                              |
|:------------|:-------|:-------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="c5d19-125">id</span><span class="sxs-lookup"><span data-stu-id="c5d19-125">id</span></span>          | <span data-ttu-id="c5d19-126">String</span><span class="sxs-lookup"><span data-stu-id="c5d19-126">String</span></span> | <span data-ttu-id="c5d19-127">A ID exclusiva do grupo externo dentro de uma conexão.</span><span class="sxs-lookup"><span data-stu-id="c5d19-127">The unique ID of the external group within a connection.</span></span> <span data-ttu-id="c5d19-128">Ele deve ser alfanumérico e ter até 128 caracteres.</span><span class="sxs-lookup"><span data-stu-id="c5d19-128">It must be alphanumeric and can be up to 128 characters long.</span></span> |
| <span data-ttu-id="c5d19-129">displayName</span><span class="sxs-lookup"><span data-stu-id="c5d19-129">displayName</span></span> | <span data-ttu-id="c5d19-130">String</span><span class="sxs-lookup"><span data-stu-id="c5d19-130">String</span></span> | <span data-ttu-id="c5d19-131">O nome amigável do grupo externo.</span><span class="sxs-lookup"><span data-stu-id="c5d19-131">The friendly name of the external group.</span></span> <span data-ttu-id="c5d19-132">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c5d19-132">Optional.</span></span>                                                                       |
| <span data-ttu-id="c5d19-133">description</span><span class="sxs-lookup"><span data-stu-id="c5d19-133">description</span></span> | <span data-ttu-id="c5d19-134">String</span><span class="sxs-lookup"><span data-stu-id="c5d19-134">String</span></span> | <span data-ttu-id="c5d19-135">A descrição do grupo externo.</span><span class="sxs-lookup"><span data-stu-id="c5d19-135">The description of the external group.</span></span> <span data-ttu-id="c5d19-136">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c5d19-136">Optional.</span></span>                                                                         

## <a name="relationships"></a><span data-ttu-id="c5d19-137">Relações</span><span class="sxs-lookup"><span data-stu-id="c5d19-137">Relationships</span></span>

| <span data-ttu-id="c5d19-138">Relação</span><span class="sxs-lookup"><span data-stu-id="c5d19-138">Relationship</span></span> | <span data-ttu-id="c5d19-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="c5d19-139">Type</span></span>                                                                  | <span data-ttu-id="c5d19-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5d19-140">Description</span></span>                                               |
|:-------------|:----------------------------------------------------------------------|:----------------------------------------------------------|
| <span data-ttu-id="c5d19-141">membros</span><span class="sxs-lookup"><span data-stu-id="c5d19-141">members</span></span>      | <span data-ttu-id="c5d19-142">[Coleção externalGroupMember](../resources/externalgroupmember.md)</span><span class="sxs-lookup"><span data-stu-id="c5d19-142">[externalGroupMember](../resources/externalgroupmember.md) collection</span></span> | <span data-ttu-id="c5d19-143">Um membro adicionado a um **externalGroup**.</span><span class="sxs-lookup"><span data-stu-id="c5d19-143">A member added to an **externalGroup**.</span></span> <span data-ttu-id="c5d19-144">Você pode adicionar usuários do Azure Active Directory, grupos do Azure Active Directory ou outros **grupos externos como** membros.</span><span class="sxs-lookup"><span data-stu-id="c5d19-144">You can add Azure Active Directory users, Azure Active Directory groups, or other **externalGroups** as members.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c5d19-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c5d19-145">JSON representation</span></span>

<span data-ttu-id="c5d19-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c5d19-146">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalGroup",
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
