---
title: tipo de recurso directorySetting
description: As configurações de diretório podem ser criadas com base no directorySettingTemplates disponível e alteradas de seus padrões predefinidos. Essas configurações podem controlar comportamentos de entidade ou de recurso, tanto em um nível de locatário quanto em um nível de entidade específico. Quando a mesma configuração é definida no nível de entidade de todo o locatário e específico, a configuração de nível de entidade específica pode ser recusada a partir da configuração de todo o locatário.  Por exemplo, a configuração de todos os locatários pode permitir que convidados sejam convidados por membros existentes de grupos, mas uma configuração de grupo específico pode recusar e não permitir que convidados sejam convidados por membros do grupo. As configurações definidas pelo sistema atualmente são controlar o comportamento de grupos do Office.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1d42e46d39e28357d6839111a5e6a865b421cf87
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42506628"
---
# <a name="directorysetting-resource-type"></a><span data-ttu-id="3adff-107">tipo de recurso directorySetting</span><span class="sxs-lookup"><span data-stu-id="3adff-107">directorySetting resource type</span></span>

<span data-ttu-id="3adff-108">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3adff-108">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3adff-109">As configurações de diretório podem ser criadas com base no [directorySettingTemplates](directorysettingtemplate.md)disponível e alteradas de seus padrões predefinidos.</span><span class="sxs-lookup"><span data-stu-id="3adff-109">Directory settings can be created based on the available [directorySettingTemplates](directorysettingtemplate.md), and changed from their preset defaults.</span></span> <span data-ttu-id="3adff-110">Essas configurações podem controlar comportamentos de entidade ou de recurso, tanto em um nível de locatário quanto em um nível de entidade específico.</span><span class="sxs-lookup"><span data-stu-id="3adff-110">These settings can govern entity or feature behaviors, both at a tenant-wide level or at a specific entity level.</span></span> <span data-ttu-id="3adff-111">Quando a mesma configuração é definida no nível de entidade de todo o locatário e específico, a configuração de nível de entidade específica pode ser recusada a partir da configuração de todo o locatário.</span><span class="sxs-lookup"><span data-stu-id="3adff-111">When the same setting is defined at both the tenant-wide and specific entity level, the specific entity level setting may opt-out from the tenant-wide setting.</span></span>  <span data-ttu-id="3adff-112">Por exemplo, a configuração de todos os locatários pode permitir que convidados sejam convidados por membros existentes de grupos, mas uma configuração de grupo específico pode recusar e não permitir que convidados sejam convidados por membros do grupo.</span><span class="sxs-lookup"><span data-stu-id="3adff-112">For example, the tenant-wide setting may allow guests to be invited by existing members of groups, but a specific group setting may opt-out and not allow guests to be invited by members of the group.</span></span> <span data-ttu-id="3adff-113">As configurações definidas pelo sistema atualmente são controlar o comportamento de grupos do Office.</span><span class="sxs-lookup"><span data-stu-id="3adff-113">Currently system defined settings are only govern Office groups behavior.</span></span>

> <span data-ttu-id="3adff-114">**Observação**: a versão do/beta do tipo de recurso directorySetting só se aplica a grupos.</span><span class="sxs-lookup"><span data-stu-id="3adff-114">**Note**: The /beta version of the directorySetting resource type only applies to groups.</span></span> <span data-ttu-id="3adff-115">A versão do/v1.0 foi renomeada como groupSetting.</span><span class="sxs-lookup"><span data-stu-id="3adff-115">The /v1.0 version has been renamed to groupSetting.</span></span>

## <a name="methods"></a><span data-ttu-id="3adff-116">Métodos</span><span class="sxs-lookup"><span data-stu-id="3adff-116">Methods</span></span>

| <span data-ttu-id="3adff-117">Método</span><span class="sxs-lookup"><span data-stu-id="3adff-117">Method</span></span>           | <span data-ttu-id="3adff-118">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3adff-118">Return Type</span></span>    |<span data-ttu-id="3adff-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="3adff-119">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3adff-120">Criar configuração</span><span class="sxs-lookup"><span data-stu-id="3adff-120">Create setting</span></span>](../api/directorysetting-post-settings.md) | [<span data-ttu-id="3adff-121">directorySetting</span><span class="sxs-lookup"><span data-stu-id="3adff-121">directorySetting</span></span>](directorysetting.md) |<span data-ttu-id="3adff-122">Criar um objeto Setting com base em um directorySettingTemplate.</span><span class="sxs-lookup"><span data-stu-id="3adff-122">Create a setting object based on a directorySettingTemplate.</span></span> <span data-ttu-id="3adff-123">A solicitação POST deve fornecer settingValues para todas as configurações definidas no modelo.</span><span class="sxs-lookup"><span data-stu-id="3adff-123">The POST request must provide settingValues for all the settings defined in the template.</span></span>|
|[<span data-ttu-id="3adff-124">Obter configuração</span><span class="sxs-lookup"><span data-stu-id="3adff-124">Get setting</span></span>](../api/directorysetting-get.md) | [<span data-ttu-id="3adff-125">directorySetting</span><span class="sxs-lookup"><span data-stu-id="3adff-125">directorySetting</span></span>](directorysetting.md) |<span data-ttu-id="3adff-126">Ler propriedades de um objeto de configuração específico.</span><span class="sxs-lookup"><span data-stu-id="3adff-126">Read properties of a specific setting object.</span></span>|
|[<span data-ttu-id="3adff-127">Listar configurações</span><span class="sxs-lookup"><span data-stu-id="3adff-127">List settings</span></span>](../api/directorysetting-list.md) | <span data-ttu-id="3adff-128">conjunto [directorySetting](directorysetting.md)</span><span class="sxs-lookup"><span data-stu-id="3adff-128">[directorySetting](directorysetting.md) collection</span></span> |<span data-ttu-id="3adff-129">Lista propriedades de todos os objetos de configuração.</span><span class="sxs-lookup"><span data-stu-id="3adff-129">List properties of all setting objects.</span></span>|
|[<span data-ttu-id="3adff-130">Atualizar configuração</span><span class="sxs-lookup"><span data-stu-id="3adff-130">Update setting</span></span>](../api/directorysetting-update.md) | [<span data-ttu-id="3adff-131">directorySetting</span><span class="sxs-lookup"><span data-stu-id="3adff-131">directorySetting</span></span>](directorysetting.md)  |<span data-ttu-id="3adff-132">Atualizar um objeto setting.</span><span class="sxs-lookup"><span data-stu-id="3adff-132">Update a setting object.</span></span> <span data-ttu-id="3adff-133">Somente settingValues pode ser alterado em uma atualização.</span><span class="sxs-lookup"><span data-stu-id="3adff-133">Only settingValues can be changed in an update.</span></span>|
|[<span data-ttu-id="3adff-134">Excluir configuração</span><span class="sxs-lookup"><span data-stu-id="3adff-134">Delete setting</span></span>](../api/directorysetting-delete.md) | <span data-ttu-id="3adff-135">None</span><span class="sxs-lookup"><span data-stu-id="3adff-135">None</span></span> |<span data-ttu-id="3adff-136">Excluir um objeto de configuração.</span><span class="sxs-lookup"><span data-stu-id="3adff-136">Delete a setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="3adff-137">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3adff-137">Properties</span></span>
| <span data-ttu-id="3adff-138">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3adff-138">Property</span></span>     | <span data-ttu-id="3adff-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="3adff-139">Type</span></span>   |<span data-ttu-id="3adff-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="3adff-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3adff-141">displayName</span><span class="sxs-lookup"><span data-stu-id="3adff-141">displayName</span></span>|<span data-ttu-id="3adff-142">string</span><span class="sxs-lookup"><span data-stu-id="3adff-142">string</span></span>|<span data-ttu-id="3adff-143">Exibe o nome deste grupo de configurações, que vem do modelo associado.</span><span class="sxs-lookup"><span data-stu-id="3adff-143">Display name of this group of settings, which comes from the associated template.</span></span> <span data-ttu-id="3adff-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3adff-144">Read-only.</span></span>|
|<span data-ttu-id="3adff-145">id</span><span class="sxs-lookup"><span data-stu-id="3adff-145">id</span></span>|<span data-ttu-id="3adff-146">string</span><span class="sxs-lookup"><span data-stu-id="3adff-146">string</span></span>| <span data-ttu-id="3adff-147">Identificador exclusivo dessas configurações.</span><span class="sxs-lookup"><span data-stu-id="3adff-147">Unique identifier for these settings.</span></span> <span data-ttu-id="3adff-148">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3adff-148">Read-only.</span></span>|
|<span data-ttu-id="3adff-149">templateId</span><span class="sxs-lookup"><span data-stu-id="3adff-149">templateId</span></span>|<span data-ttu-id="3adff-150">string</span><span class="sxs-lookup"><span data-stu-id="3adff-150">string</span></span>| <span data-ttu-id="3adff-151">Identificador exclusivo para o modelo usado para criar esse grupo de configurações.</span><span class="sxs-lookup"><span data-stu-id="3adff-151">Unique identifier for the template used to create this group of settings.</span></span> <span data-ttu-id="3adff-152">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3adff-152">Read-only.</span></span>|
|<span data-ttu-id="3adff-153">values</span><span class="sxs-lookup"><span data-stu-id="3adff-153">values</span></span>|<span data-ttu-id="3adff-154">coleção [SettingValue](settingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="3adff-154">[settingValue](settingvalue.md) collection</span></span>| <span data-ttu-id="3adff-155">Coleção de pares de valor de nome.</span><span class="sxs-lookup"><span data-stu-id="3adff-155">Collection of name value pairs.</span></span> <span data-ttu-id="3adff-156">Deve conter e definir todas as configurações definidas no modelo.</span><span class="sxs-lookup"><span data-stu-id="3adff-156">Must contain and set all the settings defined in the template.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3adff-157">Relações</span><span class="sxs-lookup"><span data-stu-id="3adff-157">Relationships</span></span>
<span data-ttu-id="3adff-158">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3adff-158">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="3adff-159">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3adff-159">JSON representation</span></span>

<span data-ttu-id="3adff-160">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3adff-160">Here is a JSON representation of the resource.</span></span>

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
