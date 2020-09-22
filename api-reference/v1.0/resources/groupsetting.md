---
title: tipo de recurso groupSetting
description: Os comportamentos de controle de configurações de grupo, como listas de palavras bloqueadas para nomes de exibição de grupo, ou se os usuários convidados podem ser proprietários de grupo.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 5dc427dc2ea2bf4e47d101ded89fdfa819d678ba
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48062943"
---
# <a name="groupsetting-resource-type"></a><span data-ttu-id="03bf5-103">tipo de recurso groupSetting</span><span class="sxs-lookup"><span data-stu-id="03bf5-103">groupSetting resource type</span></span>

<span data-ttu-id="03bf5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03bf5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="03bf5-105">Os comportamentos de controle de configurações de grupo, como listas de palavras bloqueadas para nomes de exibição de grupo, ou se os usuários convidados podem ser proprietários de grupo.</span><span class="sxs-lookup"><span data-stu-id="03bf5-105">Group settings control behaviors such as blocked word lists for group display names or whether guest users are allowed to be group owners.</span></span>

<span data-ttu-id="03bf5-106">As configurações de grupo podem ser criadas com base no [groupSettingTemplates](groupsettingtemplate.md)disponível e alteradas de seus padrões predefinidos.</span><span class="sxs-lookup"><span data-stu-id="03bf5-106">Group settings can be created based on the available [groupSettingTemplates](groupsettingtemplate.md), and changed from their preset defaults.</span></span> <span data-ttu-id="03bf5-107">Essas configurações controlam os comportamentos de grupo em um nível de locatário ou em um grupo específico.</span><span class="sxs-lookup"><span data-stu-id="03bf5-107">These settings govern group behaviors at a tenant-wide level or to a specific group.</span></span> <span data-ttu-id="03bf5-108">Quando a mesma configuração é definida em todo o locatário e em um grupo específico, a configuração de nível de grupo substitui a configuração em todo o locatário.</span><span class="sxs-lookup"><span data-stu-id="03bf5-108">When the same setting is defined at both the tenant-wide and to a specific group, the group-level setting overrides the tenant-wide setting.</span></span>  <span data-ttu-id="03bf5-109">Por exemplo, a configuração em todo o locatário pode permitir que convidados sejam convidados por membros existentes de grupos, mas uma configuração de grupo individual pode substituir e não permitir que convidados sejam convidados por membros do grupo.</span><span class="sxs-lookup"><span data-stu-id="03bf5-109">For example, the tenant-wide setting may allow guests to be invited by existing members of groups, but an individual group setting can override and not allow guests to be invited by members of the group.</span></span> <span data-ttu-id="03bf5-110">As configurações de grupo controlam o comportamento de grupos do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="03bf5-110">Group settings only govern Microsoft 365 groups behavior.</span></span>

## <a name="methods"></a><span data-ttu-id="03bf5-111">Methods</span><span class="sxs-lookup"><span data-stu-id="03bf5-111">Methods</span></span>

| <span data-ttu-id="03bf5-112">Método</span><span class="sxs-lookup"><span data-stu-id="03bf5-112">Method</span></span> | <span data-ttu-id="03bf5-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="03bf5-113">Return Type</span></span> | <span data-ttu-id="03bf5-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="03bf5-114">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="03bf5-115">Criar configuração</span><span class="sxs-lookup"><span data-stu-id="03bf5-115">Create setting</span></span>](../api/groupsetting-post-groupsettings.md) | [<span data-ttu-id="03bf5-116">groupSetting</span><span class="sxs-lookup"><span data-stu-id="03bf5-116">groupSetting</span></span>](groupsetting.md) |<span data-ttu-id="03bf5-117">Criar um objeto Setting com base em um groupSettingTemplate.</span><span class="sxs-lookup"><span data-stu-id="03bf5-117">Create a setting object based on a groupSettingTemplate.</span></span> <span data-ttu-id="03bf5-118">A solicitação POST deve fornecer settingValues para todas as configurações definidas no modelo.</span><span class="sxs-lookup"><span data-stu-id="03bf5-118">The POST request must provide settingValues for all the settings defined in the template.</span></span> |
|[<span data-ttu-id="03bf5-119">Obter configuração</span><span class="sxs-lookup"><span data-stu-id="03bf5-119">Get setting</span></span>](../api/groupsetting-get.md) | [<span data-ttu-id="03bf5-120">groupSetting</span><span class="sxs-lookup"><span data-stu-id="03bf5-120">groupSetting</span></span>](groupsetting.md) | <span data-ttu-id="03bf5-121">Ler propriedades de um objeto de configuração específico.</span><span class="sxs-lookup"><span data-stu-id="03bf5-121">Read properties of a specific setting object.</span></span> |
|[<span data-ttu-id="03bf5-122">Listar configurações</span><span class="sxs-lookup"><span data-stu-id="03bf5-122">List settings</span></span>](../api/groupsetting-list.md) | <span data-ttu-id="03bf5-123">Conjunto [groupSetting](groupsetting.md)</span><span class="sxs-lookup"><span data-stu-id="03bf5-123">[groupSetting](groupsetting.md) collection</span></span> | <span data-ttu-id="03bf5-124">Lista propriedades de todos os objetos de configuração.</span><span class="sxs-lookup"><span data-stu-id="03bf5-124">List properties of all setting objects.</span></span> |
|[<span data-ttu-id="03bf5-125">Atualizar configuração</span><span class="sxs-lookup"><span data-stu-id="03bf5-125">Update setting</span></span>](../api/groupsetting-update.md) | [<span data-ttu-id="03bf5-126">groupSetting</span><span class="sxs-lookup"><span data-stu-id="03bf5-126">groupSetting</span></span>](groupsetting.md) | <span data-ttu-id="03bf5-127">Atualize o objeto groupsetting.</span><span class="sxs-lookup"><span data-stu-id="03bf5-127">Update groupsetting object.</span></span> |
|[<span data-ttu-id="03bf5-128">Excluir configuração</span><span class="sxs-lookup"><span data-stu-id="03bf5-128">Delete setting</span></span>](../api/groupsetting-delete.md) | <span data-ttu-id="03bf5-129">None</span><span class="sxs-lookup"><span data-stu-id="03bf5-129">None</span></span> | <span data-ttu-id="03bf5-130">Excluir um objeto de configuração.</span><span class="sxs-lookup"><span data-stu-id="03bf5-130">Delete a setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="03bf5-131">Propriedades</span><span class="sxs-lookup"><span data-stu-id="03bf5-131">Properties</span></span>

| <span data-ttu-id="03bf5-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="03bf5-132">Property</span></span> | <span data-ttu-id="03bf5-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="03bf5-133">Type</span></span> | <span data-ttu-id="03bf5-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="03bf5-134">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="03bf5-135">displayName</span><span class="sxs-lookup"><span data-stu-id="03bf5-135">displayName</span></span>|<span data-ttu-id="03bf5-136">String</span><span class="sxs-lookup"><span data-stu-id="03bf5-136">String</span></span>| <span data-ttu-id="03bf5-137">Exibe o nome deste grupo de configurações, que vem do modelo associado.</span><span class="sxs-lookup"><span data-stu-id="03bf5-137">Display name of this group of settings, which comes from the associated template.</span></span> |
|<span data-ttu-id="03bf5-138">id</span><span class="sxs-lookup"><span data-stu-id="03bf5-138">id</span></span>|<span data-ttu-id="03bf5-139">String</span><span class="sxs-lookup"><span data-stu-id="03bf5-139">String</span></span>| <span data-ttu-id="03bf5-140">Identificador exclusivo dessas configurações.</span><span class="sxs-lookup"><span data-stu-id="03bf5-140">Unique identifier for these settings.</span></span> <span data-ttu-id="03bf5-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="03bf5-141">Read-only.</span></span> |
|<span data-ttu-id="03bf5-142">templateId</span><span class="sxs-lookup"><span data-stu-id="03bf5-142">templateId</span></span>|<span data-ttu-id="03bf5-143">String</span><span class="sxs-lookup"><span data-stu-id="03bf5-143">String</span></span>| <span data-ttu-id="03bf5-144">Identificador exclusivo para o modelo usado para criar esse grupo de configurações.</span><span class="sxs-lookup"><span data-stu-id="03bf5-144">Unique identifier for the template used to create this group of settings.</span></span> <span data-ttu-id="03bf5-145">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="03bf5-145">Read-only.</span></span> |
|<span data-ttu-id="03bf5-146">values</span><span class="sxs-lookup"><span data-stu-id="03bf5-146">values</span></span>|<span data-ttu-id="03bf5-147">coleção [SettingValue](settingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="03bf5-147">[settingValue](settingvalue.md) collection</span></span>| <span data-ttu-id="03bf5-148">Coleção de pares de valor de nome.</span><span class="sxs-lookup"><span data-stu-id="03bf5-148">Collection of name value pairs.</span></span> <span data-ttu-id="03bf5-149">Deve conter e definir todas as configurações definidas no modelo.</span><span class="sxs-lookup"><span data-stu-id="03bf5-149">Must contain and set all the settings defined in the template.</span></span> |

## <a name="relationships"></a><span data-ttu-id="03bf5-150">Relações</span><span class="sxs-lookup"><span data-stu-id="03bf5-150">Relationships</span></span>

<span data-ttu-id="03bf5-151">Nenhum</span><span class="sxs-lookup"><span data-stu-id="03bf5-151">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="03bf5-152">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="03bf5-152">JSON representation</span></span>

<span data-ttu-id="03bf5-153">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="03bf5-153">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.groupSetting"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)",
  "templateId": "String",
  "values": [{"@odata.type": "microsoft.graph.settingValue"}]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupSetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

