---
title: tipo de recurso groupSetting
description: As configurações de grupo controlam comportamentos como listas de palavras bloqueadas para nomes de exibição de grupo ou se os usuários convidados podem ser proprietários de grupo.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 42e6c0dc0f0ffd48da84023c5e4ff0d97cb446f2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911690"
---
# <a name="groupsetting-resource-type"></a><span data-ttu-id="e91f7-103">tipo de recurso groupSetting</span><span class="sxs-lookup"><span data-stu-id="e91f7-103">groupSetting resource type</span></span>

<span data-ttu-id="e91f7-104">As configurações de grupo controlam comportamentos como listas de palavras bloqueadas para nomes de exibição de grupo ou se os usuários convidados podem ser proprietários de grupo.</span><span class="sxs-lookup"><span data-stu-id="e91f7-104">Group settings control behaviors such as blocked word lists for group display names or whether guest users are allowed to be group owners.</span></span>

<span data-ttu-id="e91f7-p101">As configurações de grupo podem ser criadas com base no [groupSettingTemplates](groupsettingtemplate.md) disponível e alteradas de seus padrões predefinidos. Essas configurações regem os comportamentos de grupo em um nível total de locatários ou para um grupo específico. Quando a mesma configuração é definida no nível do locatário e para um grupo específico, a configuração de nível de grupo anula a configuração de nível de locatários.  Por exemplo, a configuração de nível de locatário pode permitir que os convidados sejam convidados por membros existentes dos grupos, mas uma configuração de grupo individual pode substitui-la e não permitir que os convidados sejam convidados por membros do grupo. As configurações de grupo regem apenas o comportamento dos grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="e91f7-p101">Group settings can be created based on the available [groupSettingTemplates](groupsettingtemplate.md), and changed from their preset defaults. These settings govern group behaviors at a tenant-wide level or to a specific group. When the same setting is defined at both the tenant-wide and to a specific group, the group-level setting overrides the tenant-wide setting.  For example, the tenant-wide setting may allow guests to be invited by existing members of groups, but an individual group setting can override and not allow guests to be invited by members of the group. Group settings only govern Office 365 groups behavior.</span></span>

## <a name="methods"></a><span data-ttu-id="e91f7-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="e91f7-110">Methods</span></span>

| <span data-ttu-id="e91f7-111">Método</span><span class="sxs-lookup"><span data-stu-id="e91f7-111">Method</span></span> | <span data-ttu-id="e91f7-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e91f7-112">Return Type</span></span> | <span data-ttu-id="e91f7-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="e91f7-113">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="e91f7-114">Criar configuração</span><span class="sxs-lookup"><span data-stu-id="e91f7-114">Create setting</span></span>](../api/groupsetting-post-groupsettings.md) | [<span data-ttu-id="e91f7-115">groupSetting</span><span class="sxs-lookup"><span data-stu-id="e91f7-115">groupSetting</span></span>](groupsetting.md) |<span data-ttu-id="e91f7-p102">Crie um objeto de configuração com base em um groupSettingTemplate. A solicitação POST deve fornecer settingValues para todas as configurações definidas no modelo.</span><span class="sxs-lookup"><span data-stu-id="e91f7-p102">Create a setting object based on a groupSettingTemplate. The POST request must provide settingValues for all the settings defined in the template.</span></span> |
|[<span data-ttu-id="e91f7-118">Obter configuração</span><span class="sxs-lookup"><span data-stu-id="e91f7-118">Get setting</span></span>](../api/groupsetting-get.md) | [<span data-ttu-id="e91f7-119">groupSetting</span><span class="sxs-lookup"><span data-stu-id="e91f7-119">groupSetting</span></span>](groupsetting.md) | <span data-ttu-id="e91f7-120">Ler propriedades de um objeto de configuração específico.</span><span class="sxs-lookup"><span data-stu-id="e91f7-120">Read properties of a specific setting object.</span></span> |
|[<span data-ttu-id="e91f7-121">Listar configurações</span><span class="sxs-lookup"><span data-stu-id="e91f7-121">List settings</span></span>](../api/groupsetting-list.md) | <span data-ttu-id="e91f7-122">Conjunto [groupSetting](groupsetting.md)</span><span class="sxs-lookup"><span data-stu-id="e91f7-122">[groupSetting](groupsetting.md) collection</span></span> | <span data-ttu-id="e91f7-123">Lista propriedades de todos os objetos de configuração.</span><span class="sxs-lookup"><span data-stu-id="e91f7-123">List properties of all setting objects.</span></span> |
|[<span data-ttu-id="e91f7-124">Atualizar configuração</span><span class="sxs-lookup"><span data-stu-id="e91f7-124">Update setting</span></span>](../api/groupsetting-update.md) | [<span data-ttu-id="e91f7-125">groupSetting</span><span class="sxs-lookup"><span data-stu-id="e91f7-125">groupSetting</span></span>](groupsetting.md) | <span data-ttu-id="e91f7-126">Atualize o objeto groupsetting.</span><span class="sxs-lookup"><span data-stu-id="e91f7-126">Update groupsetting object.</span></span> |
|[<span data-ttu-id="e91f7-127">Excluir configuração</span><span class="sxs-lookup"><span data-stu-id="e91f7-127">Delete setting</span></span>](../api/groupsetting-delete.md) | <span data-ttu-id="e91f7-128">None</span><span class="sxs-lookup"><span data-stu-id="e91f7-128">None</span></span> | <span data-ttu-id="e91f7-129">Excluir um objeto de configuração.</span><span class="sxs-lookup"><span data-stu-id="e91f7-129">Delete a setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e91f7-130">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e91f7-130">Properties</span></span>

| <span data-ttu-id="e91f7-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e91f7-131">Property</span></span> | <span data-ttu-id="e91f7-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="e91f7-132">Type</span></span> | <span data-ttu-id="e91f7-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="e91f7-133">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="e91f7-134">displayName</span><span class="sxs-lookup"><span data-stu-id="e91f7-134">displayName</span></span>|<span data-ttu-id="e91f7-135">String</span><span class="sxs-lookup"><span data-stu-id="e91f7-135">String</span></span>| <span data-ttu-id="e91f7-136">Nome de exibição deste grupo de configurações, originado do modelo associado.</span><span class="sxs-lookup"><span data-stu-id="e91f7-136">Display name of this group of settings, which comes from the associated template.</span></span> |
|<span data-ttu-id="e91f7-137">id</span><span class="sxs-lookup"><span data-stu-id="e91f7-137">id</span></span>|<span data-ttu-id="e91f7-138">String</span><span class="sxs-lookup"><span data-stu-id="e91f7-138">String</span></span>| <span data-ttu-id="e91f7-p103">Identificador exclusivo destas configurações. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e91f7-p103">Unique identifier for these settings. Read-only.</span></span> |
|<span data-ttu-id="e91f7-141">templateId</span><span class="sxs-lookup"><span data-stu-id="e91f7-141">templateId</span></span>|<span data-ttu-id="e91f7-142">String</span><span class="sxs-lookup"><span data-stu-id="e91f7-142">String</span></span>| <span data-ttu-id="e91f7-p104">Identificador exclusivo para o modelo usado para criar este grupo de configurações. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e91f7-p104">Unique identifier for the template used to create this group of settings. Read-only.</span></span> |
|<span data-ttu-id="e91f7-145">values</span><span class="sxs-lookup"><span data-stu-id="e91f7-145">values</span></span>|<span data-ttu-id="e91f7-146">conjunto [settingValue](settingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="e91f7-146">[settingValue](settingvalue.md) collection</span></span>| <span data-ttu-id="e91f7-p105">Conjunto de pares de nome/valor. Deve conter e ajustar todas as configurações definidas no modelo.</span><span class="sxs-lookup"><span data-stu-id="e91f7-p105">Collection of name value pairs. Must contain and set all the settings defined in the template.</span></span> |

## <a name="relationships"></a><span data-ttu-id="e91f7-149">Relações</span><span class="sxs-lookup"><span data-stu-id="e91f7-149">Relationships</span></span>

<span data-ttu-id="e91f7-150">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e91f7-150">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e91f7-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e91f7-151">JSON representation</span></span>

<span data-ttu-id="e91f7-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e91f7-152">Here is a JSON representation of the resource.</span></span>

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
