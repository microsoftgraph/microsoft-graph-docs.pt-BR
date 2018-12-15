---
title: tipo de recurso de teamsTab
description: 'Um teamsTab é uma guia que tem fixados (anexado) a um canal de uma equipe. '
ms.openlocfilehash: 102d4c0b766d8a0d9bdf22cb2ed76f5e06d87ad5
ms.sourcegitcommit: f3d479edf03935d0edbbc7668a65f7cde2a56c92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2018
ms.locfileid: "27283616"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="96bbb-103">tipo de recurso de teamsTab</span><span class="sxs-lookup"><span data-stu-id="96bbb-103">teamsTab resource type</span></span>

> <span data-ttu-id="96bbb-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="96bbb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="96bbb-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="96bbb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="96bbb-106">Um teamsTab é uma [guia](../resources/teamstab.md) que tem fixados (anexado) a um [canal](channel.md) de dentro de uma [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="96bbb-106">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="96bbb-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="96bbb-107">Methods</span></span>

| <span data-ttu-id="96bbb-108">Método</span><span class="sxs-lookup"><span data-stu-id="96bbb-108">Method</span></span>       | <span data-ttu-id="96bbb-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="96bbb-109">Return Type</span></span>  |<span data-ttu-id="96bbb-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="96bbb-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="96bbb-111">Guias de lista</span><span class="sxs-lookup"><span data-stu-id="96bbb-111">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="96bbb-112">teamsTab</span><span class="sxs-lookup"><span data-stu-id="96bbb-112">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="96bbb-113">Guias de listas fixados em um canal.</span><span class="sxs-lookup"><span data-stu-id="96bbb-113">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="96bbb-114">Obtenha o guia</span><span class="sxs-lookup"><span data-stu-id="96bbb-114">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="96bbb-115">teamsTab</span><span class="sxs-lookup"><span data-stu-id="96bbb-115">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="96bbb-116">Lê uma guia fixada em um canal.</span><span class="sxs-lookup"><span data-stu-id="96bbb-116">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="96bbb-117">Adicionar guia</span><span class="sxs-lookup"><span data-stu-id="96bbb-117">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="96bbb-118">teamsTab</span><span class="sxs-lookup"><span data-stu-id="96bbb-118">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="96bbb-119">Adiciona (pins) uma guia em um canal.</span><span class="sxs-lookup"><span data-stu-id="96bbb-119">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="96bbb-120">Remover guia</span><span class="sxs-lookup"><span data-stu-id="96bbb-120">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="96bbb-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="96bbb-121">None</span></span> | <span data-ttu-id="96bbb-122">Remove (unpin) uma guia de um canal.</span><span class="sxs-lookup"><span data-stu-id="96bbb-122">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="96bbb-123">Guia de atualização</span><span class="sxs-lookup"><span data-stu-id="96bbb-123">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="96bbb-124">teamsTab</span><span class="sxs-lookup"><span data-stu-id="96bbb-124">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="96bbb-125">Atualiza as propriedades da guia.</span><span class="sxs-lookup"><span data-stu-id="96bbb-125">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="96bbb-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="96bbb-126">Properties</span></span>

|<span data-ttu-id="96bbb-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="96bbb-127">Property</span></span>|<span data-ttu-id="96bbb-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="96bbb-128">Type</span></span>|<span data-ttu-id="96bbb-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="96bbb-129">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="96bbb-130">id</span><span class="sxs-lookup"><span data-stu-id="96bbb-130">id</span></span>              |   <span data-ttu-id="96bbb-131">string</span><span class="sxs-lookup"><span data-stu-id="96bbb-131">string</span></span>                  |  <span data-ttu-id="96bbb-132">Identificador que identifica exclusivamente uma instância específica de um canal na guia leitura apenas.</span><span class="sxs-lookup"><span data-stu-id="96bbb-132">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="96bbb-133">displayName</span><span class="sxs-lookup"><span data-stu-id="96bbb-133">displayName</span></span>            |   <span data-ttu-id="96bbb-134">string</span><span class="sxs-lookup"><span data-stu-id="96bbb-134">string</span></span>                  |  <span data-ttu-id="96bbb-135">Nome da guia.</span><span class="sxs-lookup"><span data-stu-id="96bbb-135">Name of the tab.</span></span>     |
|  <span data-ttu-id="96bbb-136">name</span><span class="sxs-lookup"><span data-stu-id="96bbb-136">name</span></span>            |   <span data-ttu-id="96bbb-137">string</span><span class="sxs-lookup"><span data-stu-id="96bbb-137">string</span></span>                  |  <span data-ttu-id="96bbb-138">(Obsoleto) Nome da guia.</span><span class="sxs-lookup"><span data-stu-id="96bbb-138">(Deprecated) Name of the tab.</span></span>     |
|  <span data-ttu-id="96bbb-139">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="96bbb-139">teamsAppId</span></span>           |   <span data-ttu-id="96bbb-140">string</span><span class="sxs-lookup"><span data-stu-id="96bbb-140">string</span></span>             |  <span data-ttu-id="96bbb-141">Identificador de definição de aplicativo da guia. Este valor não pode ser alterado após a criação da guia.</span><span class="sxs-lookup"><span data-stu-id="96bbb-141">App definition identifier of the tab. This value cannot be changed after tab creation.</span></span>     |
|  <span data-ttu-id="96bbb-142">sortOrderIndex</span><span class="sxs-lookup"><span data-stu-id="96bbb-142">sortOrderIndex</span></span>  |   <span data-ttu-id="96bbb-143">inteiro</span><span class="sxs-lookup"><span data-stu-id="96bbb-143">int</span></span>                     |  <span data-ttu-id="96bbb-144">Índice da ordem usada para classificar as guias.</span><span class="sxs-lookup"><span data-stu-id="96bbb-144">Index of the order used for sorting tabs.</span></span>     |
|  <span data-ttu-id="96bbb-145">webUrl</span><span class="sxs-lookup"><span data-stu-id="96bbb-145">webUrl</span></span>          |   <span data-ttu-id="96bbb-146">string</span><span class="sxs-lookup"><span data-stu-id="96bbb-146">string</span></span>                  |  <span data-ttu-id="96bbb-147">Link profundo url da instância do guia.</span><span class="sxs-lookup"><span data-stu-id="96bbb-147">Deep link url of the tab instance.</span></span> <span data-ttu-id="96bbb-148">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="96bbb-148">Read only.</span></span>     |
|  <span data-ttu-id="96bbb-149">configuration</span><span class="sxs-lookup"><span data-stu-id="96bbb-149">configuration</span></span>        |   [<span data-ttu-id="96bbb-150">teamsTabConfiguration</span><span class="sxs-lookup"><span data-stu-id="96bbb-150">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="96bbb-151">Contêiner de configurações personalizadas aplicadas a uma guia. Na guia é considerada configurado somente depois que essa propriedade for definida.</span><span class="sxs-lookup"><span data-stu-id="96bbb-151">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="96bbb-152">Relações</span><span class="sxs-lookup"><span data-stu-id="96bbb-152">Relationships</span></span>

| <span data-ttu-id="96bbb-153">Relação</span><span class="sxs-lookup"><span data-stu-id="96bbb-153">Relationship</span></span> | <span data-ttu-id="96bbb-154">Tipo</span><span class="sxs-lookup"><span data-stu-id="96bbb-154">Type</span></span>   | <span data-ttu-id="96bbb-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="96bbb-155">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="96bbb-156">teamsApp</span><span class="sxs-lookup"><span data-stu-id="96bbb-156">teamsApp</span></span>|[<span data-ttu-id="96bbb-157">teamsApp</span><span class="sxs-lookup"><span data-stu-id="96bbb-157">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="96bbb-158">O aplicativo que está vinculado à guia.</span><span class="sxs-lookup"><span data-stu-id="96bbb-158">The application that is linked to the tab.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="96bbb-159">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="96bbb-159">JSON representation</span></span>

<span data-ttu-id="96bbb-160">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="96bbb-160">The following is a JSON representation of the resource.</span></span>


<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.teamsTab"
}-->

```json
{  
  "id": "string",
  "displayName": "string",
  "teamsAppId": "string",
  "sortOrderIndex": "string",
  "webUrl": "string",
  "configuration" : "teamsTabConfiguration"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsTab resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

## <a name="see-also"></a><span data-ttu-id="96bbb-161">Confira também</span><span class="sxs-lookup"><span data-stu-id="96bbb-161">See also</span></span>

[<span data-ttu-id="96bbb-162">Configurando os tipos de guia interna</span><span class="sxs-lookup"><span data-stu-id="96bbb-162">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
