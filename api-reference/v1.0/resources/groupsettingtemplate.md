---
title: tipo de recurso groupSettingTemplate
description: Modelos de configuração de grupo representam configurações definidas pelo sistema disponíveis para o locatário.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 0d1d1359a515d854b71fab5b01792d1e31843343
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896921"
---
# <a name="groupsettingtemplate-resource-type"></a><span data-ttu-id="2c191-103">tipo de recurso groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="2c191-103">groupSettingTemplate resource type</span></span>

<span data-ttu-id="2c191-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c191-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2c191-105">Modelos de configuração de grupo representam configurações definidas pelo sistema disponíveis para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2c191-105">Group setting templates represent system-defined settings available to the tenant.</span></span> <span data-ttu-id="2c191-106">[As configurações de grupo](groupsetting.md) podem ser criadas com base no **groupSettingTemplates**disponível e os valores alterados de seus padrões predefinidos.</span><span class="sxs-lookup"><span data-stu-id="2c191-106">[Group settings](groupsetting.md) can be created based on the available **groupSettingTemplates**, and values changed from their preset defaults.</span></span> <span data-ttu-id="2c191-107">Modelos de configuração de grupo não podem ser criados, atualizados ou excluídos.</span><span class="sxs-lookup"><span data-stu-id="2c191-107">Group setting templates cannot be created, updated or deleted.</span></span> <span data-ttu-id="2c191-108">Essas configurações podem representar configurações de todo o locatário ou podem representar configurações de grupo específicas.</span><span class="sxs-lookup"><span data-stu-id="2c191-108">These settings can represent tenant-wide settings, or can represent specific group settings.</span></span> <span data-ttu-id="2c191-109">Atualmente, os únicos modelos disponíveis se aplicam aos grupos do Microsoft 365 e incluem configurações como se os usuários podem criar grupos ou convidar convidados de fora da organização para se tornarem membros de um grupo.</span><span class="sxs-lookup"><span data-stu-id="2c191-109">Currently, the only templates available apply to Microsoft 365 groups, and include settings such as whether users can create groups or invite guests from outside the organization to become members of a group.</span></span>

## <a name="methods"></a><span data-ttu-id="2c191-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="2c191-110">Methods</span></span>

| <span data-ttu-id="2c191-111">Método</span><span class="sxs-lookup"><span data-stu-id="2c191-111">Method</span></span> | <span data-ttu-id="2c191-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2c191-112">Return Type</span></span> | <span data-ttu-id="2c191-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c191-113">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="2c191-114">Obter groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="2c191-114">Get groupSettingTemplate</span></span>](../api/groupsettingtemplate-get.md) | [<span data-ttu-id="2c191-115">groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="2c191-115">groupSettingTemplate</span></span>](groupsettingtemplate.md) | <span data-ttu-id="2c191-116">Leia as propriedades específicas de um dos objetos groupSettingTemplate definidos pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="2c191-116">Read the specific properties of one of the system defined groupSettingTemplate objects.</span></span> |
|[<span data-ttu-id="2c191-117">Listar groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="2c191-117">List groupSettingTemplate</span></span>](../api/groupsettingtemplate-list.md) | [<span data-ttu-id="2c191-118">Coleção de groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="2c191-118">Collection of groupSettingTemplate</span></span>](groupsettingtemplate.md) |<span data-ttu-id="2c191-119">Lista todos os objetos groupSettingTemplate definidos pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="2c191-119">List all of the system defined groupSettingTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="2c191-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2c191-120">Properties</span></span>

| <span data-ttu-id="2c191-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2c191-121">Property</span></span> | <span data-ttu-id="2c191-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="2c191-122">Type</span></span> | <span data-ttu-id="2c191-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c191-123">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="2c191-124">description</span><span class="sxs-lookup"><span data-stu-id="2c191-124">description</span></span>|<span data-ttu-id="2c191-125">String</span><span class="sxs-lookup"><span data-stu-id="2c191-125">String</span></span>| <span data-ttu-id="2c191-126">Descrição do modelo.</span><span class="sxs-lookup"><span data-stu-id="2c191-126">Description of the template.</span></span> |
|<span data-ttu-id="2c191-127">displayName</span><span class="sxs-lookup"><span data-stu-id="2c191-127">displayName</span></span>|<span data-ttu-id="2c191-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2c191-128">String</span></span>| <span data-ttu-id="2c191-129">Nome para exibição do modelo.</span><span class="sxs-lookup"><span data-stu-id="2c191-129">Display name of the template.</span></span> |
|<span data-ttu-id="2c191-130">id</span><span class="sxs-lookup"><span data-stu-id="2c191-130">id</span></span>|<span data-ttu-id="2c191-131">String</span><span class="sxs-lookup"><span data-stu-id="2c191-131">String</span></span>| <span data-ttu-id="2c191-132">Identificador exclusivo do modelo.</span><span class="sxs-lookup"><span data-stu-id="2c191-132">Unique identifier for the template.</span></span> <span data-ttu-id="2c191-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2c191-133">Read-only.</span></span>|
|<span data-ttu-id="2c191-134">values</span><span class="sxs-lookup"><span data-stu-id="2c191-134">values</span></span>|<span data-ttu-id="2c191-135">coleção [settingTemplateValue](settingtemplatevalue.md)</span><span class="sxs-lookup"><span data-stu-id="2c191-135">[settingTemplateValue](settingtemplatevalue.md) collection</span></span>| <span data-ttu-id="2c191-136">Coleção de settingTemplateValues que lista o conjunto de configurações disponíveis, padrões e tipos que compõem esse modelo.</span><span class="sxs-lookup"><span data-stu-id="2c191-136">Collection of settingTemplateValues that list the set of available settings, defaults and types that make up this template.</span></span> |

## <a name="relationships"></a><span data-ttu-id="2c191-137">Relações</span><span class="sxs-lookup"><span data-stu-id="2c191-137">Relationships</span></span>

<span data-ttu-id="2c191-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2c191-138">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="2c191-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2c191-139">JSON representation</span></span>

<span data-ttu-id="2c191-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2c191-140">Here is a JSON representation of the resource.</span></span>

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
