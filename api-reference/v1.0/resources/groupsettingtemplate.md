---
title: Tipo de recurso groupSettingTemplate
description: Os modelos de configuração de grupo representam as configurações definidas pelo sistema disponíveis para o locatário.
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: a7868538c13b1e386e7aa10dcdf3fed9c03b198f
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680868"
---
# <a name="groupsettingtemplate-resource-type"></a><span data-ttu-id="7c29f-103">Tipo de recurso groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="7c29f-103">groupSettingTemplate resource type</span></span>

<span data-ttu-id="7c29f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c29f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7c29f-105">Os modelos de configuração de grupo representam as configurações definidas pelo sistema disponíveis para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7c29f-105">Group setting templates represent system-defined settings available to the tenant.</span></span> <span data-ttu-id="7c29f-106">[As configurações de grupo](groupsetting.md) podem ser criadas com base no **groupSettingTemplates** disponível e valores alterados de seus padrões predefinidos.</span><span class="sxs-lookup"><span data-stu-id="7c29f-106">[Group settings](groupsetting.md) can be created based on the available **groupSettingTemplates**, and values changed from their preset defaults.</span></span> <span data-ttu-id="7c29f-107">Modelos de configuração de grupo não podem ser criados, atualizados ou excluídos.</span><span class="sxs-lookup"><span data-stu-id="7c29f-107">Group setting templates cannot be created, updated or deleted.</span></span> <span data-ttu-id="7c29f-108">Essas configurações podem representar configurações de todo o locatário ou representar configurações de grupo específicas.</span><span class="sxs-lookup"><span data-stu-id="7c29f-108">These settings can represent tenant-wide settings, or can represent specific group settings.</span></span> <span data-ttu-id="7c29f-109">Atualmente, os únicos modelos disponíveis se aplicam Microsoft 365 grupos e incluem configurações como se os usuários podem criar grupos ou convidar convidados de fora da organização para se tornarem membros de um grupo.</span><span class="sxs-lookup"><span data-stu-id="7c29f-109">Currently, the only templates available apply to Microsoft 365 groups, and include settings such as whether users can create groups or invite guests from outside the organization to become members of a group.</span></span>

## <a name="methods"></a><span data-ttu-id="7c29f-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="7c29f-110">Methods</span></span>

| <span data-ttu-id="7c29f-111">Método</span><span class="sxs-lookup"><span data-stu-id="7c29f-111">Method</span></span> | <span data-ttu-id="7c29f-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7c29f-112">Return Type</span></span> | <span data-ttu-id="7c29f-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c29f-113">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="7c29f-114">Obter groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="7c29f-114">Get groupSettingTemplate</span></span>](../api/groupsettingtemplate-get.md) | [<span data-ttu-id="7c29f-115">groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="7c29f-115">groupSettingTemplate</span></span>](groupsettingtemplate.md) | <span data-ttu-id="7c29f-116">Leia as propriedades específicas de um dos objetos groupSettingTemplate definidos pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="7c29f-116">Read the specific properties of one of the system defined groupSettingTemplate objects.</span></span> |
|[<span data-ttu-id="7c29f-117">Listar groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="7c29f-117">List groupSettingTemplate</span></span>](../api/groupsettingtemplate-list.md) | [<span data-ttu-id="7c29f-118">Coleção de groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="7c29f-118">Collection of groupSettingTemplate</span></span>](groupsettingtemplate.md) |<span data-ttu-id="7c29f-119">Listar todos os objetos groupSettingTemplate definidos pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="7c29f-119">List all of the system defined groupSettingTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="7c29f-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7c29f-120">Properties</span></span>

| <span data-ttu-id="7c29f-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7c29f-121">Property</span></span> | <span data-ttu-id="7c29f-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="7c29f-122">Type</span></span> | <span data-ttu-id="7c29f-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c29f-123">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="7c29f-124">description</span><span class="sxs-lookup"><span data-stu-id="7c29f-124">description</span></span>|<span data-ttu-id="7c29f-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7c29f-125">String</span></span>| <span data-ttu-id="7c29f-126">Descrição do modelo.</span><span class="sxs-lookup"><span data-stu-id="7c29f-126">Description of the template.</span></span> |
|<span data-ttu-id="7c29f-127">displayName</span><span class="sxs-lookup"><span data-stu-id="7c29f-127">displayName</span></span>|<span data-ttu-id="7c29f-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7c29f-128">String</span></span>| <span data-ttu-id="7c29f-129">Nome de exibição do modelo.</span><span class="sxs-lookup"><span data-stu-id="7c29f-129">Display name of the template.</span></span> |
|<span data-ttu-id="7c29f-130">id</span><span class="sxs-lookup"><span data-stu-id="7c29f-130">id</span></span>|<span data-ttu-id="7c29f-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7c29f-131">String</span></span>| <span data-ttu-id="7c29f-132">Identificador exclusivo do modelo.</span><span class="sxs-lookup"><span data-stu-id="7c29f-132">Unique identifier for the template.</span></span> <span data-ttu-id="7c29f-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7c29f-133">Read-only.</span></span>|
|<span data-ttu-id="7c29f-134">values</span><span class="sxs-lookup"><span data-stu-id="7c29f-134">values</span></span>|<span data-ttu-id="7c29f-135">[Coleção settingTemplateValue](settingtemplatevalue.md)</span><span class="sxs-lookup"><span data-stu-id="7c29f-135">[settingTemplateValue](settingtemplatevalue.md) collection</span></span>| <span data-ttu-id="7c29f-136">Coleção de settingTemplateValues que lista o conjunto de configurações, padrões e tipos disponíveis que comem esse modelo.</span><span class="sxs-lookup"><span data-stu-id="7c29f-136">Collection of settingTemplateValues that list the set of available settings, defaults and types that make up this template.</span></span> |

## <a name="relationships"></a><span data-ttu-id="7c29f-137">Relações</span><span class="sxs-lookup"><span data-stu-id="7c29f-137">Relationships</span></span>

<span data-ttu-id="7c29f-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7c29f-138">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="7c29f-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7c29f-139">JSON representation</span></span>

<span data-ttu-id="7c29f-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7c29f-140">Here is a JSON representation of the resource.</span></span>

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

