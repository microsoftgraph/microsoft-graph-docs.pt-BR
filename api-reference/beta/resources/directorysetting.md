---
title: tipo de recurso directorySetting
description: As configurações de diretório podem ser criadas com base no directorySettingTemplates disponível e alteradas de seus padrões predefinidos. Essas configurações podem controlar comportamentos de entidade ou de recurso, tanto em um nível de locatário quanto em um nível de entidade específico. Quando a mesma configuração é definida no nível de entidade de todo o locatário e específico, a configuração de nível de entidade específica pode ser recusada a partir da configuração de todo o locatário.  Por exemplo, a configuração de todos os locatários pode permitir que convidados sejam convidados por membros existentes de grupos, mas uma configuração de grupo específico pode recusar e não permitir que convidados sejam convidados por membros do grupo. As configurações definidas pelo sistema atualmente são controlar o comportamento de grupos do Office.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3336ec351c44ba0b69df55e1383cca73b6ea1a96
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340739"
---
# <a name="directorysetting-resource-type"></a><span data-ttu-id="603fe-107">tipo de recurso directorySetting</span><span class="sxs-lookup"><span data-stu-id="603fe-107">directorySetting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="603fe-108">As configurações de diretório podem ser criadas com base no [directorySettingTemplates](directorysettingtemplate.md)disponível e alteradas de seus padrões predefinidos.</span><span class="sxs-lookup"><span data-stu-id="603fe-108">Directory settings can be created based on the available [directorySettingTemplates](directorysettingtemplate.md), and changed from their preset defaults.</span></span> <span data-ttu-id="603fe-109">Essas configurações podem controlar comportamentos de entidade ou de recurso, tanto em um nível de locatário quanto em um nível de entidade específico.</span><span class="sxs-lookup"><span data-stu-id="603fe-109">These settings can govern entity or feature behaviors, both at a tenant-wide level or at a specific entity level.</span></span> <span data-ttu-id="603fe-110">Quando a mesma configuração é definida no nível de entidade de todo o locatário e específico, a configuração de nível de entidade específica pode ser recusada a partir da configuração de todo o locatário.</span><span class="sxs-lookup"><span data-stu-id="603fe-110">When the same setting is defined at both the tenant-wide and specific entity level, the specific entity level setting may opt-out from the tenant-wide setting.</span></span>  <span data-ttu-id="603fe-111">Por exemplo, a configuração de todos os locatários pode permitir que convidados sejam convidados por membros existentes de grupos, mas uma configuração de grupo específico pode recusar e não permitir que convidados sejam convidados por membros do grupo.</span><span class="sxs-lookup"><span data-stu-id="603fe-111">For example, the tenant-wide setting may allow guests to be invited by existing members of groups, but a specific group setting may opt-out and not allow guests to be invited by members of the group.</span></span> <span data-ttu-id="603fe-112">As configurações definidas pelo sistema atualmente são controlar o comportamento de grupos do Office.</span><span class="sxs-lookup"><span data-stu-id="603fe-112">Currently system defined settings are only govern Office groups behavior.</span></span>

> <span data-ttu-id="603fe-113">**Observação**: a versão do/beta do tipo de recurso directorySetting só se aplica a grupos.</span><span class="sxs-lookup"><span data-stu-id="603fe-113">**Note**: The /beta version of the directorySetting resource type only applies to groups.</span></span> <span data-ttu-id="603fe-114">A versão do/v1.0 foi renomeada como groupSetting.</span><span class="sxs-lookup"><span data-stu-id="603fe-114">The /v1.0 version has been renamed to groupSetting.</span></span>

## <a name="methods"></a><span data-ttu-id="603fe-115">Métodos</span><span class="sxs-lookup"><span data-stu-id="603fe-115">Methods</span></span>

| <span data-ttu-id="603fe-116">Método</span><span class="sxs-lookup"><span data-stu-id="603fe-116">Method</span></span>           | <span data-ttu-id="603fe-117">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="603fe-117">Return Type</span></span>    |<span data-ttu-id="603fe-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="603fe-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="603fe-119">Criar configuração</span><span class="sxs-lookup"><span data-stu-id="603fe-119">Create setting</span></span>](../api/directorysetting-post-settings.md) | [<span data-ttu-id="603fe-120">directorySetting</span><span class="sxs-lookup"><span data-stu-id="603fe-120">directorySetting</span></span>](directorysetting.md) |<span data-ttu-id="603fe-121">Criar um objeto Setting com base em um directorySettingTemplate.</span><span class="sxs-lookup"><span data-stu-id="603fe-121">Create a setting object based on a directorySettingTemplate.</span></span> <span data-ttu-id="603fe-122">A solicitação POST deve fornecer settingValues para todas as configurações definidas no modelo.</span><span class="sxs-lookup"><span data-stu-id="603fe-122">The POST request must provide settingValues for all the settings defined in the template.</span></span>|
|[<span data-ttu-id="603fe-123">Obter configuração</span><span class="sxs-lookup"><span data-stu-id="603fe-123">Get setting</span></span>](../api/directorysetting-get.md) | [<span data-ttu-id="603fe-124">directorySetting</span><span class="sxs-lookup"><span data-stu-id="603fe-124">directorySetting</span></span>](directorysetting.md) |<span data-ttu-id="603fe-125">Ler propriedades de um objeto de configuração específico.</span><span class="sxs-lookup"><span data-stu-id="603fe-125">Read properties of a specific setting object.</span></span>|
|[<span data-ttu-id="603fe-126">Listar configurações</span><span class="sxs-lookup"><span data-stu-id="603fe-126">List settings</span></span>](../api/directorysetting-list.md) | <span data-ttu-id="603fe-127">conjunto [directorySetting](directorysetting.md)</span><span class="sxs-lookup"><span data-stu-id="603fe-127">[directorySetting](directorysetting.md) collection</span></span> |<span data-ttu-id="603fe-128">Lista propriedades de todos os objetos de configuração.</span><span class="sxs-lookup"><span data-stu-id="603fe-128">List properties of all setting objects.</span></span>|
|[<span data-ttu-id="603fe-129">Atualizar configuração</span><span class="sxs-lookup"><span data-stu-id="603fe-129">Update setting</span></span>](../api/directorysetting-update.md) | [<span data-ttu-id="603fe-130">directorySetting</span><span class="sxs-lookup"><span data-stu-id="603fe-130">directorySetting</span></span>](directorysetting.md)  |<span data-ttu-id="603fe-131">Atualizar um objeto setting.</span><span class="sxs-lookup"><span data-stu-id="603fe-131">Update a setting object.</span></span> <span data-ttu-id="603fe-132">Somente settingValues pode ser alterado em uma atualização.</span><span class="sxs-lookup"><span data-stu-id="603fe-132">Only settingValues can be changed in an update.</span></span>|
|[<span data-ttu-id="603fe-133">Excluir configuração</span><span class="sxs-lookup"><span data-stu-id="603fe-133">Delete setting</span></span>](../api/directorysetting-delete.md) | <span data-ttu-id="603fe-134">None</span><span class="sxs-lookup"><span data-stu-id="603fe-134">None</span></span> |<span data-ttu-id="603fe-135">Excluir um objeto de configuração.</span><span class="sxs-lookup"><span data-stu-id="603fe-135">Delete a setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="603fe-136">Propriedades</span><span class="sxs-lookup"><span data-stu-id="603fe-136">Properties</span></span>
| <span data-ttu-id="603fe-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="603fe-137">Property</span></span>     | <span data-ttu-id="603fe-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="603fe-138">Type</span></span>   |<span data-ttu-id="603fe-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="603fe-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="603fe-140">displayName</span><span class="sxs-lookup"><span data-stu-id="603fe-140">displayName</span></span>|<span data-ttu-id="603fe-141">string</span><span class="sxs-lookup"><span data-stu-id="603fe-141">string</span></span>|<span data-ttu-id="603fe-142">Exibe o nome deste grupo de configurações, que vem do modelo associado.</span><span class="sxs-lookup"><span data-stu-id="603fe-142">Display name of this group of settings, which comes from the associated template.</span></span> <span data-ttu-id="603fe-143">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="603fe-143">Read-only.</span></span>|
|<span data-ttu-id="603fe-144">id</span><span class="sxs-lookup"><span data-stu-id="603fe-144">id</span></span>|<span data-ttu-id="603fe-145">string</span><span class="sxs-lookup"><span data-stu-id="603fe-145">string</span></span>| <span data-ttu-id="603fe-146">Identificador exclusivo dessas configurações.</span><span class="sxs-lookup"><span data-stu-id="603fe-146">Unique identifier for these settings.</span></span> <span data-ttu-id="603fe-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="603fe-147">Read-only.</span></span>|
|<span data-ttu-id="603fe-148">templateId</span><span class="sxs-lookup"><span data-stu-id="603fe-148">templateId</span></span>|<span data-ttu-id="603fe-149">string</span><span class="sxs-lookup"><span data-stu-id="603fe-149">string</span></span>| <span data-ttu-id="603fe-150">Identificador exclusivo para o modelo usado para criar esse grupo de configurações.</span><span class="sxs-lookup"><span data-stu-id="603fe-150">Unique identifier for the template used to create this group of settings.</span></span> <span data-ttu-id="603fe-151">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="603fe-151">Read-only.</span></span>|
|<span data-ttu-id="603fe-152">values</span><span class="sxs-lookup"><span data-stu-id="603fe-152">values</span></span>|<span data-ttu-id="603fe-153">[](settingvalue.md) coleção SettingValue</span><span class="sxs-lookup"><span data-stu-id="603fe-153">[settingValue](settingvalue.md) collection</span></span>| <span data-ttu-id="603fe-154">Coleção de pares de valor de nome.</span><span class="sxs-lookup"><span data-stu-id="603fe-154">Collection of name value pairs.</span></span> <span data-ttu-id="603fe-155">Deve conter e definir todas as configurações definidas no modelo.</span><span class="sxs-lookup"><span data-stu-id="603fe-155">Must contain and set all the settings defined in the template.</span></span>|

## <a name="relationships"></a><span data-ttu-id="603fe-156">Relações</span><span class="sxs-lookup"><span data-stu-id="603fe-156">Relationships</span></span>
<span data-ttu-id="603fe-157">Nenhum</span><span class="sxs-lookup"><span data-stu-id="603fe-157">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="603fe-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="603fe-158">JSON representation</span></span>

<span data-ttu-id="603fe-159">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="603fe-159">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directorySetting"
}-->

```json
{
  "displayName": "string",
  "id": "string (identifier)",
  "templateId": "string",
  "values": [{"@odata.type": "microsoft.graph.settingValue"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directorySetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
