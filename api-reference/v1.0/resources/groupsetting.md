---
title: tipo de recurso groupSetting
description: Os comportamentos de controle de configurações de grupo, como listas de palavras bloqueadas para nomes de exibição de grupo, ou se os usuários convidados podem ser proprietários de grupo.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c85b062e955fc15f83728813427f2de5579e297e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030237"
---
# <a name="groupsetting-resource-type"></a><span data-ttu-id="f45fc-103">tipo de recurso groupSetting</span><span class="sxs-lookup"><span data-stu-id="f45fc-103">groupSetting resource type</span></span>

<span data-ttu-id="f45fc-104">Os comportamentos de controle de configurações de grupo, como listas de palavras bloqueadas para nomes de exibição de grupo, ou se os usuários convidados podem ser proprietários de grupo.</span><span class="sxs-lookup"><span data-stu-id="f45fc-104">Group settings control behaviors such as blocked word lists for group display names or whether guest users are allowed to be group owners.</span></span>

<span data-ttu-id="f45fc-105">As configurações de grupo podem ser criadas com base no [groupSettingTemplates](groupsettingtemplate.md)disponível e alteradas de seus padrões predefinidos.</span><span class="sxs-lookup"><span data-stu-id="f45fc-105">Group settings can be created based on the available [groupSettingTemplates](groupsettingtemplate.md), and changed from their preset defaults.</span></span> <span data-ttu-id="f45fc-106">Essas configurações controlam os comportamentos de grupo em um nível de locatário ou em um grupo específico.</span><span class="sxs-lookup"><span data-stu-id="f45fc-106">These settings govern group behaviors at a tenant-wide level or to a specific group.</span></span> <span data-ttu-id="f45fc-107">Quando a mesma configuração é definida em todo o locatário e em um grupo específico, a configuração de nível de grupo substitui a configuração em todo o locatário.</span><span class="sxs-lookup"><span data-stu-id="f45fc-107">When the same setting is defined at both the tenant-wide and to a specific group, the group-level setting overrides the tenant-wide setting.</span></span>  <span data-ttu-id="f45fc-108">Por exemplo, a configuração em todo o locatário pode permitir que convidados sejam convidados por membros existentes de grupos, mas uma configuração de grupo individual pode substituir e não permitir que convidados sejam convidados por membros do grupo.</span><span class="sxs-lookup"><span data-stu-id="f45fc-108">For example, the tenant-wide setting may allow guests to be invited by existing members of groups, but an individual group setting can override and not allow guests to be invited by members of the group.</span></span> <span data-ttu-id="f45fc-109">As configurações de grupo regem o comportamento de grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="f45fc-109">Group settings only govern Office 365 groups behavior.</span></span>

## <a name="methods"></a><span data-ttu-id="f45fc-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="f45fc-110">Methods</span></span>

| <span data-ttu-id="f45fc-111">Método</span><span class="sxs-lookup"><span data-stu-id="f45fc-111">Method</span></span> | <span data-ttu-id="f45fc-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f45fc-112">Return Type</span></span> | <span data-ttu-id="f45fc-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="f45fc-113">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="f45fc-114">Criar configuração</span><span class="sxs-lookup"><span data-stu-id="f45fc-114">Create setting</span></span>](../api/groupsetting-post-groupsettings.md) | [<span data-ttu-id="f45fc-115">groupSetting</span><span class="sxs-lookup"><span data-stu-id="f45fc-115">groupSetting</span></span>](groupsetting.md) |<span data-ttu-id="f45fc-116">Criar um objeto Setting com base em um groupSettingTemplate.</span><span class="sxs-lookup"><span data-stu-id="f45fc-116">Create a setting object based on a groupSettingTemplate.</span></span> <span data-ttu-id="f45fc-117">A solicitação POST deve fornecer settingValues para todas as configurações definidas no modelo.</span><span class="sxs-lookup"><span data-stu-id="f45fc-117">The POST request must provide settingValues for all the settings defined in the template.</span></span> |
|[<span data-ttu-id="f45fc-118">Obter configuração</span><span class="sxs-lookup"><span data-stu-id="f45fc-118">Get setting</span></span>](../api/groupsetting-get.md) | [<span data-ttu-id="f45fc-119">groupSetting</span><span class="sxs-lookup"><span data-stu-id="f45fc-119">groupSetting</span></span>](groupsetting.md) | <span data-ttu-id="f45fc-120">Ler propriedades de um objeto de configuração específico.</span><span class="sxs-lookup"><span data-stu-id="f45fc-120">Read properties of a specific setting object.</span></span> |
|[<span data-ttu-id="f45fc-121">Listar configurações</span><span class="sxs-lookup"><span data-stu-id="f45fc-121">List settings</span></span>](../api/groupsetting-list.md) | <span data-ttu-id="f45fc-122">Conjunto [groupSetting](groupsetting.md)</span><span class="sxs-lookup"><span data-stu-id="f45fc-122">[groupSetting](groupsetting.md) collection</span></span> | <span data-ttu-id="f45fc-123">Lista propriedades de todos os objetos de configuração.</span><span class="sxs-lookup"><span data-stu-id="f45fc-123">List properties of all setting objects.</span></span> |
|[<span data-ttu-id="f45fc-124">Atualizar configuração</span><span class="sxs-lookup"><span data-stu-id="f45fc-124">Update setting</span></span>](../api/groupsetting-update.md) | [<span data-ttu-id="f45fc-125">groupSetting</span><span class="sxs-lookup"><span data-stu-id="f45fc-125">groupSetting</span></span>](groupsetting.md) | <span data-ttu-id="f45fc-126">Atualize o objeto groupsetting.</span><span class="sxs-lookup"><span data-stu-id="f45fc-126">Update groupsetting object.</span></span> |
|[<span data-ttu-id="f45fc-127">Excluir configuração</span><span class="sxs-lookup"><span data-stu-id="f45fc-127">Delete setting</span></span>](../api/groupsetting-delete.md) | <span data-ttu-id="f45fc-128">None</span><span class="sxs-lookup"><span data-stu-id="f45fc-128">None</span></span> | <span data-ttu-id="f45fc-129">Excluir um objeto de configuração.</span><span class="sxs-lookup"><span data-stu-id="f45fc-129">Delete a setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="f45fc-130">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f45fc-130">Properties</span></span>

| <span data-ttu-id="f45fc-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f45fc-131">Property</span></span> | <span data-ttu-id="f45fc-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="f45fc-132">Type</span></span> | <span data-ttu-id="f45fc-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="f45fc-133">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="f45fc-134">displayName</span><span class="sxs-lookup"><span data-stu-id="f45fc-134">displayName</span></span>|<span data-ttu-id="f45fc-135">String</span><span class="sxs-lookup"><span data-stu-id="f45fc-135">String</span></span>| <span data-ttu-id="f45fc-136">Exibe o nome deste grupo de configurações, que vem do modelo associado.</span><span class="sxs-lookup"><span data-stu-id="f45fc-136">Display name of this group of settings, which comes from the associated template.</span></span> |
|<span data-ttu-id="f45fc-137">id</span><span class="sxs-lookup"><span data-stu-id="f45fc-137">id</span></span>|<span data-ttu-id="f45fc-138">String</span><span class="sxs-lookup"><span data-stu-id="f45fc-138">String</span></span>| <span data-ttu-id="f45fc-139">Identificador exclusivo dessas configurações.</span><span class="sxs-lookup"><span data-stu-id="f45fc-139">Unique identifier for these settings.</span></span> <span data-ttu-id="f45fc-140">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f45fc-140">Read-only.</span></span> |
|<span data-ttu-id="f45fc-141">templateId</span><span class="sxs-lookup"><span data-stu-id="f45fc-141">templateId</span></span>|<span data-ttu-id="f45fc-142">String</span><span class="sxs-lookup"><span data-stu-id="f45fc-142">String</span></span>| <span data-ttu-id="f45fc-143">Identificador exclusivo para o modelo usado para criar esse grupo de configurações.</span><span class="sxs-lookup"><span data-stu-id="f45fc-143">Unique identifier for the template used to create this group of settings.</span></span> <span data-ttu-id="f45fc-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f45fc-144">Read-only.</span></span> |
|<span data-ttu-id="f45fc-145">values</span><span class="sxs-lookup"><span data-stu-id="f45fc-145">values</span></span>|<span data-ttu-id="f45fc-146">[](settingvalue.md) coleção SettingValue</span><span class="sxs-lookup"><span data-stu-id="f45fc-146">[settingValue](settingvalue.md) collection</span></span>| <span data-ttu-id="f45fc-147">Coleção de pares de valor de nome.</span><span class="sxs-lookup"><span data-stu-id="f45fc-147">Collection of name value pairs.</span></span> <span data-ttu-id="f45fc-148">Deve conter e definir todas as configurações definidas no modelo.</span><span class="sxs-lookup"><span data-stu-id="f45fc-148">Must contain and set all the settings defined in the template.</span></span> |

## <a name="relationships"></a><span data-ttu-id="f45fc-149">Relações</span><span class="sxs-lookup"><span data-stu-id="f45fc-149">Relationships</span></span>

<span data-ttu-id="f45fc-150">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f45fc-150">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f45fc-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f45fc-151">JSON representation</span></span>

<span data-ttu-id="f45fc-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f45fc-152">Here is a JSON representation of the resource.</span></span>

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
