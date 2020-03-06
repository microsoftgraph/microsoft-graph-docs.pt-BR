---
title: tipo de recurso groupSettingTemplate
description: Modelos de configuração de grupo representam configurações definidas pelo sistema disponíveis para o locatário. As configurações de grupo podem ser criadas com base no **groupSettingTemplates**disponível e os valores alterados de seus padrões predefinidos. Modelos de configuração de grupo não podem ser criados, atualizados ou excluídos. Essas configurações podem representar configurações de todo o locatário ou podem representar configurações de grupo específicas. Atualmente, os únicos modelos disponíveis se aplicam aos grupos do Office 365 e incluem configurações como se os usuários podem criar grupos ou convidar convidados de fora da organização para se tornarem membros de um grupo.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fa392d6bf6dcd8ceaf15d97dfe695fbaaeabed4b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531353"
---
# <a name="groupsettingtemplate-resource-type"></a><span data-ttu-id="f2c56-107">tipo de recurso groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="f2c56-107">groupSettingTemplate resource type</span></span>

<span data-ttu-id="f2c56-108">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2c56-108">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f2c56-109">Modelos de configuração de grupo representam configurações definidas pelo sistema disponíveis para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f2c56-109">Group setting templates represent system-defined settings available to the tenant.</span></span> <span data-ttu-id="f2c56-110">[As configurações de grupo](groupsetting.md) podem ser criadas com base no **groupSettingTemplates**disponível e os valores alterados de seus padrões predefinidos.</span><span class="sxs-lookup"><span data-stu-id="f2c56-110">[Group settings](groupsetting.md) can be created based on the available **groupSettingTemplates**, and values changed from their preset defaults.</span></span> <span data-ttu-id="f2c56-111">Modelos de configuração de grupo não podem ser criados, atualizados ou excluídos.</span><span class="sxs-lookup"><span data-stu-id="f2c56-111">Group setting templates cannot be created, updated or deleted.</span></span> <span data-ttu-id="f2c56-112">Essas configurações podem representar configurações de todo o locatário ou podem representar configurações de grupo específicas.</span><span class="sxs-lookup"><span data-stu-id="f2c56-112">These settings can represent tenant-wide settings, or can represent specific group settings.</span></span> <span data-ttu-id="f2c56-113">Atualmente, os únicos modelos disponíveis se aplicam aos grupos do Office 365 e incluem configurações como se os usuários podem criar grupos ou convidar convidados de fora da organização para se tornarem membros de um grupo.</span><span class="sxs-lookup"><span data-stu-id="f2c56-113">Currently, the only templates available apply to Office 365 groups, and include settings such as whether users can create groups or invite guests from outside the organization to become members of a group.</span></span>

## <a name="methods"></a><span data-ttu-id="f2c56-114">Métodos</span><span class="sxs-lookup"><span data-stu-id="f2c56-114">Methods</span></span>

| <span data-ttu-id="f2c56-115">Método</span><span class="sxs-lookup"><span data-stu-id="f2c56-115">Method</span></span> | <span data-ttu-id="f2c56-116">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f2c56-116">Return Type</span></span> | <span data-ttu-id="f2c56-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2c56-117">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="f2c56-118">Obter groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="f2c56-118">Get groupSettingTemplate</span></span>](../api/groupsettingtemplate-get.md) | [<span data-ttu-id="f2c56-119">groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="f2c56-119">groupSettingTemplate</span></span>](groupsettingtemplate.md) | <span data-ttu-id="f2c56-120">Leia as propriedades específicas de um dos objetos groupSettingTemplate definidos pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="f2c56-120">Read the specific properties of one of the system defined groupSettingTemplate objects.</span></span> |
|[<span data-ttu-id="f2c56-121">Listar groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="f2c56-121">List groupSettingTemplate</span></span>](../api/groupsettingtemplate-list.md) | [<span data-ttu-id="f2c56-122">Coleção de groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="f2c56-122">Collection of groupSettingTemplate</span></span>](groupsettingtemplate.md) |<span data-ttu-id="f2c56-123">Lista todos os objetos groupSettingTemplate definidos pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="f2c56-123">List all of the system defined groupSettingTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="f2c56-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f2c56-124">Properties</span></span>

| <span data-ttu-id="f2c56-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f2c56-125">Property</span></span> | <span data-ttu-id="f2c56-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2c56-126">Type</span></span> | <span data-ttu-id="f2c56-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2c56-127">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="f2c56-128">description</span><span class="sxs-lookup"><span data-stu-id="f2c56-128">description</span></span>|<span data-ttu-id="f2c56-129">String</span><span class="sxs-lookup"><span data-stu-id="f2c56-129">String</span></span>| <span data-ttu-id="f2c56-130">Descrição do modelo.</span><span class="sxs-lookup"><span data-stu-id="f2c56-130">Description of the template.</span></span> |
|<span data-ttu-id="f2c56-131">displayName</span><span class="sxs-lookup"><span data-stu-id="f2c56-131">displayName</span></span>|<span data-ttu-id="f2c56-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2c56-132">String</span></span>| <span data-ttu-id="f2c56-133">Nome para exibição do modelo.</span><span class="sxs-lookup"><span data-stu-id="f2c56-133">Display name of the template.</span></span> |
|<span data-ttu-id="f2c56-134">id</span><span class="sxs-lookup"><span data-stu-id="f2c56-134">id</span></span>|<span data-ttu-id="f2c56-135">String</span><span class="sxs-lookup"><span data-stu-id="f2c56-135">String</span></span>| <span data-ttu-id="f2c56-136">Identificador exclusivo do modelo.</span><span class="sxs-lookup"><span data-stu-id="f2c56-136">Unique identifier for the template.</span></span> <span data-ttu-id="f2c56-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f2c56-137">Read-only.</span></span>|
|<span data-ttu-id="f2c56-138">values</span><span class="sxs-lookup"><span data-stu-id="f2c56-138">values</span></span>|<span data-ttu-id="f2c56-139">coleção [settingTemplateValue](settingtemplatevalue.md)</span><span class="sxs-lookup"><span data-stu-id="f2c56-139">[settingTemplateValue](settingtemplatevalue.md) collection</span></span>| <span data-ttu-id="f2c56-140">Coleção de settingTemplateValues que lista o conjunto de configurações disponíveis, padrões e tipos que compõem esse modelo.</span><span class="sxs-lookup"><span data-stu-id="f2c56-140">Collection of settingTemplateValues that list the set of available settings, defaults and types that make up this template.</span></span> |

## <a name="relationships"></a><span data-ttu-id="f2c56-141">Relações</span><span class="sxs-lookup"><span data-stu-id="f2c56-141">Relationships</span></span>

<span data-ttu-id="f2c56-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f2c56-142">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="f2c56-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f2c56-143">JSON representation</span></span>

<span data-ttu-id="f2c56-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f2c56-144">Here is a JSON representation of the resource.</span></span>

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
