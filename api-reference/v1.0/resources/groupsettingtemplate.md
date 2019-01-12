---
title: tipo de recurso groupSettingTemplate
description: Os modelos de configuração de grupo representam configurações definidas pelo sistema disponíveis para o locatário. As configurações de grupo podem ser criadas com base no **groupSettingTemplates** disponível e valores alterados de seus padrões predefinidos. Os modelos de configuração de grupo não podem ser criados, atualizados ou excluídos. Essas configurações podem representar configurações de nível de locatário ou configurações de grupo específico. Atualmente, os únicos modelos disponíveis se aplicam aos grupos do Office 365 e incluem as configurações, como se os usuários podem criar grupos ou convidar pessoas de fora da organização a se tornarem membros de um grupo.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2b9b95303b72bc111f045010e71459f541e9a9b8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27919334"
---
# <a name="groupsettingtemplate-resource-type"></a><span data-ttu-id="a7f8e-107">tipo de recurso groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="a7f8e-107">groupSettingTemplate resource type</span></span>

<span data-ttu-id="a7f8e-p102">Os modelos de configuração de grupo representam configurações definidas pelo sistema disponíveis para o locatário. As [configurações de grupo](groupsetting.md) podem ser criadas com base no **groupSettingTemplates** disponível e valores alterados de seus padrões predefinidos. Os modelos de configuração de grupo não podem ser criados, atualizados ou excluídos. Essas configurações podem representar configurações de nível de locatário ou configurações de grupo específico. Atualmente, os únicos modelos disponíveis se aplicam aos grupos do Office 365 e incluem as configurações, como se os usuários podem criar grupos ou convidar pessoas de fora da organização a se tornarem membros de um grupo.</span><span class="sxs-lookup"><span data-stu-id="a7f8e-p102">Group setting templates represent system-defined settings available to the tenant. [Group settings](groupsetting.md) can be created based on the available **groupSettingTemplates**, and values changed from their preset defaults. Group setting templates cannot be created, updated or deleted. These settings can represent tenant-wide settings, or can represent specific group settings. Currently, the only templates available apply to Office 365 groups, and include settings such as whether users can create groups or invite guests from outside the organization to become members of a group.</span></span>

## <a name="methods"></a><span data-ttu-id="a7f8e-113">Métodos</span><span class="sxs-lookup"><span data-stu-id="a7f8e-113">Methods</span></span>

| <span data-ttu-id="a7f8e-114">Método</span><span class="sxs-lookup"><span data-stu-id="a7f8e-114">Method</span></span> | <span data-ttu-id="a7f8e-115">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a7f8e-115">Return Type</span></span> | <span data-ttu-id="a7f8e-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="a7f8e-116">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="a7f8e-117">Obter groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="a7f8e-117">Get groupSettingTemplate</span></span>](../api/groupsettingtemplate-get.md) | [<span data-ttu-id="a7f8e-118">groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="a7f8e-118">groupSettingTemplate</span></span>](groupsettingtemplate.md) | <span data-ttu-id="a7f8e-119">Leia as propriedades específicas de um dos objetos groupSettingTemplate definidos pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="a7f8e-119">Read the specific properties of one of the system defined groupSettingTemplate objects.</span></span> |
|[<span data-ttu-id="a7f8e-120">Lista groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="a7f8e-120">List groupSettingTemplate</span></span>](../api/groupsettingtemplate-list.md) | [<span data-ttu-id="a7f8e-121">Coleção de groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="a7f8e-121">Collection of groupSettingTemplate</span></span>](groupsettingtemplate.md) |<span data-ttu-id="a7f8e-122">Lista todos os objetos de groupSettingTemplate definidos pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="a7f8e-122">List all of the system defined groupSettingTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="a7f8e-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a7f8e-123">Properties</span></span>

| <span data-ttu-id="a7f8e-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a7f8e-124">Property</span></span> | <span data-ttu-id="a7f8e-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="a7f8e-125">Type</span></span> | <span data-ttu-id="a7f8e-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="a7f8e-126">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a7f8e-127">description</span><span class="sxs-lookup"><span data-stu-id="a7f8e-127">description</span></span>|<span data-ttu-id="a7f8e-128">String</span><span class="sxs-lookup"><span data-stu-id="a7f8e-128">String</span></span>| <span data-ttu-id="a7f8e-129">Descrição do modelo.</span><span class="sxs-lookup"><span data-stu-id="a7f8e-129">Description of the template.</span></span> |
|<span data-ttu-id="a7f8e-130">displayName</span><span class="sxs-lookup"><span data-stu-id="a7f8e-130">displayName</span></span>|<span data-ttu-id="a7f8e-131">String</span><span class="sxs-lookup"><span data-stu-id="a7f8e-131">String</span></span>| <span data-ttu-id="a7f8e-132">Nome para exibição do modelo</span><span class="sxs-lookup"><span data-stu-id="a7f8e-132">Display name of the template.</span></span> |
|<span data-ttu-id="a7f8e-133">id</span><span class="sxs-lookup"><span data-stu-id="a7f8e-133">id</span></span>|<span data-ttu-id="a7f8e-134">String</span><span class="sxs-lookup"><span data-stu-id="a7f8e-134">String</span></span>| <span data-ttu-id="a7f8e-p103">O identificador exclusivo do modelo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a7f8e-p103">Unique identifier for the template. Read-only.</span></span>|
|<span data-ttu-id="a7f8e-137">values</span><span class="sxs-lookup"><span data-stu-id="a7f8e-137">values</span></span>|<span data-ttu-id="a7f8e-138">Conjunto [settingTemplateValue](settingtemplatevalue.md)</span><span class="sxs-lookup"><span data-stu-id="a7f8e-138">[settingTemplateValue](settingtemplatevalue.md) collection</span></span>| <span data-ttu-id="a7f8e-139">Coleção de settingTemplateValues que lista o conjunto de configurações disponíveis, padrões e tipos que compõem este modelo.</span><span class="sxs-lookup"><span data-stu-id="a7f8e-139">Collection of settingTemplateValues that list the set of available settings, defaults and types that make up this template.</span></span> |

## <a name="relationships"></a><span data-ttu-id="a7f8e-140">Relações</span><span class="sxs-lookup"><span data-stu-id="a7f8e-140">Relationships</span></span>

<span data-ttu-id="a7f8e-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a7f8e-141">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="a7f8e-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a7f8e-142">JSON representation</span></span>

<span data-ttu-id="a7f8e-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a7f8e-143">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.groupSettingTemplate"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "values": [{"@odata.type": "microsoft.graph.settingTemplateValue"}]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupSettingTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
