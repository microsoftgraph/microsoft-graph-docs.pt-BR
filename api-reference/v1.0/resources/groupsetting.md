---
title: Tipo de recurso groupSetting
description: As configurações de grupo controlam comportamentos como listas de palavras bloqueadas para nomes de exibição de grupo ou se os usuários convidados têm permissão para serem proprietários do grupo.
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 1e18f78f0b0d7c9e8cb9c054afd5645ae45e1c48
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680875"
---
# <a name="groupsetting-resource-type"></a><span data-ttu-id="f30cf-103">Tipo de recurso groupSetting</span><span class="sxs-lookup"><span data-stu-id="f30cf-103">groupSetting resource type</span></span>

<span data-ttu-id="f30cf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f30cf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f30cf-105">As configurações de grupo controlam comportamentos como listas de palavras bloqueadas para nomes de exibição de grupo ou se os usuários convidados têm permissão para serem proprietários do grupo.</span><span class="sxs-lookup"><span data-stu-id="f30cf-105">Group settings control behaviors such as blocked word lists for group display names or whether guest users are allowed to be group owners.</span></span>

<span data-ttu-id="f30cf-106">As configurações de grupo podem ser criadas com base no [groupSettingTemplates](groupsettingtemplate.md)disponível e alteradas de seus padrões predefinidos.</span><span class="sxs-lookup"><span data-stu-id="f30cf-106">Group settings can be created based on the available [groupSettingTemplates](groupsettingtemplate.md), and changed from their preset defaults.</span></span> <span data-ttu-id="f30cf-107">Essas configurações governam comportamentos de grupo em um nível de locatário ou em um grupo específico.</span><span class="sxs-lookup"><span data-stu-id="f30cf-107">These settings govern group behaviors at a tenant-wide level or to a specific group.</span></span> <span data-ttu-id="f30cf-108">Quando a mesma configuração é definida em todo o locatário e em um grupo específico, a configuração de nível de grupo substitui a configuração de todo o locatário.</span><span class="sxs-lookup"><span data-stu-id="f30cf-108">When the same setting is defined at both the tenant-wide and to a specific group, the group-level setting overrides the tenant-wide setting.</span></span>  <span data-ttu-id="f30cf-109">Por exemplo, a configuração de todo o locatário pode permitir que os convidados sejam convidados por membros existentes de grupos, mas uma configuração de grupo individual pode substituir e não permitir que os convidados sejam convidados por membros do grupo.</span><span class="sxs-lookup"><span data-stu-id="f30cf-109">For example, the tenant-wide setting may allow guests to be invited by existing members of groups, but an individual group setting can override and not allow guests to be invited by members of the group.</span></span> <span data-ttu-id="f30cf-110">As configurações de grupo governam apenas Microsoft 365 comportamento de grupos.</span><span class="sxs-lookup"><span data-stu-id="f30cf-110">Group settings only govern Microsoft 365 groups behavior.</span></span>

## <a name="methods"></a><span data-ttu-id="f30cf-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="f30cf-111">Methods</span></span>

| <span data-ttu-id="f30cf-112">Método</span><span class="sxs-lookup"><span data-stu-id="f30cf-112">Method</span></span> | <span data-ttu-id="f30cf-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f30cf-113">Return Type</span></span> | <span data-ttu-id="f30cf-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="f30cf-114">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="f30cf-115">Criar configuração</span><span class="sxs-lookup"><span data-stu-id="f30cf-115">Create setting</span></span>](../api/groupsetting-post-groupsettings.md) | [<span data-ttu-id="f30cf-116">groupSetting</span><span class="sxs-lookup"><span data-stu-id="f30cf-116">groupSetting</span></span>](groupsetting.md) |<span data-ttu-id="f30cf-117">Crie um objeto de configuração com base em um groupSettingTemplate.</span><span class="sxs-lookup"><span data-stu-id="f30cf-117">Create a setting object based on a groupSettingTemplate.</span></span> <span data-ttu-id="f30cf-118">A solicitação POST deve fornecer settingValues para todas as configurações definidas no modelo.</span><span class="sxs-lookup"><span data-stu-id="f30cf-118">The POST request must provide settingValues for all the settings defined in the template.</span></span> |
|[<span data-ttu-id="f30cf-119">Obter configuração</span><span class="sxs-lookup"><span data-stu-id="f30cf-119">Get setting</span></span>](../api/groupsetting-get.md) | [<span data-ttu-id="f30cf-120">groupSetting</span><span class="sxs-lookup"><span data-stu-id="f30cf-120">groupSetting</span></span>](groupsetting.md) | <span data-ttu-id="f30cf-121">Ler propriedades de um objeto de configuração específico.</span><span class="sxs-lookup"><span data-stu-id="f30cf-121">Read properties of a specific setting object.</span></span> |
|[<span data-ttu-id="f30cf-122">Listar configurações</span><span class="sxs-lookup"><span data-stu-id="f30cf-122">List settings</span></span>](../api/groupsetting-list.md) | <span data-ttu-id="f30cf-123">Conjunto [groupSetting](groupsetting.md)</span><span class="sxs-lookup"><span data-stu-id="f30cf-123">[groupSetting](groupsetting.md) collection</span></span> | <span data-ttu-id="f30cf-124">Lista propriedades de todos os objetos de configuração.</span><span class="sxs-lookup"><span data-stu-id="f30cf-124">List properties of all setting objects.</span></span> |
|[<span data-ttu-id="f30cf-125">Atualizar configuração</span><span class="sxs-lookup"><span data-stu-id="f30cf-125">Update setting</span></span>](../api/groupsetting-update.md) | [<span data-ttu-id="f30cf-126">groupSetting</span><span class="sxs-lookup"><span data-stu-id="f30cf-126">groupSetting</span></span>](groupsetting.md) | <span data-ttu-id="f30cf-127">Atualizar objeto groupsetting.</span><span class="sxs-lookup"><span data-stu-id="f30cf-127">Update groupsetting object.</span></span> |
|[<span data-ttu-id="f30cf-128">Excluir configuração</span><span class="sxs-lookup"><span data-stu-id="f30cf-128">Delete setting</span></span>](../api/groupsetting-delete.md) | <span data-ttu-id="f30cf-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f30cf-129">None</span></span> | <span data-ttu-id="f30cf-130">Excluir um objeto de configuração.</span><span class="sxs-lookup"><span data-stu-id="f30cf-130">Delete a setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="f30cf-131">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f30cf-131">Properties</span></span>

| <span data-ttu-id="f30cf-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f30cf-132">Property</span></span> | <span data-ttu-id="f30cf-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="f30cf-133">Type</span></span> | <span data-ttu-id="f30cf-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="f30cf-134">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="f30cf-135">displayName</span><span class="sxs-lookup"><span data-stu-id="f30cf-135">displayName</span></span>|<span data-ttu-id="f30cf-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f30cf-136">String</span></span>| <span data-ttu-id="f30cf-137">Nome de exibição desse grupo de configurações, que vem do modelo associado.</span><span class="sxs-lookup"><span data-stu-id="f30cf-137">Display name of this group of settings, which comes from the associated template.</span></span> |
|<span data-ttu-id="f30cf-138">id</span><span class="sxs-lookup"><span data-stu-id="f30cf-138">id</span></span>|<span data-ttu-id="f30cf-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f30cf-139">String</span></span>| <span data-ttu-id="f30cf-140">Identificador exclusivo para essas configurações.</span><span class="sxs-lookup"><span data-stu-id="f30cf-140">Unique identifier for these settings.</span></span> <span data-ttu-id="f30cf-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f30cf-141">Read-only.</span></span> |
|<span data-ttu-id="f30cf-142">templateId</span><span class="sxs-lookup"><span data-stu-id="f30cf-142">templateId</span></span>|<span data-ttu-id="f30cf-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f30cf-143">String</span></span>| <span data-ttu-id="f30cf-144">Identificador exclusivo do modelo usado para criar esse grupo de configurações.</span><span class="sxs-lookup"><span data-stu-id="f30cf-144">Unique identifier for the template used to create this group of settings.</span></span> <span data-ttu-id="f30cf-145">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f30cf-145">Read-only.</span></span> |
|<span data-ttu-id="f30cf-146">values</span><span class="sxs-lookup"><span data-stu-id="f30cf-146">values</span></span>|<span data-ttu-id="f30cf-147">[coleção settingValue](settingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="f30cf-147">[settingValue](settingvalue.md) collection</span></span>| <span data-ttu-id="f30cf-148">Coleção de pares de valores de nome.</span><span class="sxs-lookup"><span data-stu-id="f30cf-148">Collection of name value pairs.</span></span> <span data-ttu-id="f30cf-149">Deve conter e definir todas as configurações definidas no modelo.</span><span class="sxs-lookup"><span data-stu-id="f30cf-149">Must contain and set all the settings defined in the template.</span></span> |

## <a name="relationships"></a><span data-ttu-id="f30cf-150">Relações</span><span class="sxs-lookup"><span data-stu-id="f30cf-150">Relationships</span></span>

<span data-ttu-id="f30cf-151">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f30cf-151">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f30cf-152">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f30cf-152">JSON representation</span></span>

<span data-ttu-id="f30cf-153">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f30cf-153">Here is a JSON representation of the resource.</span></span>

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

