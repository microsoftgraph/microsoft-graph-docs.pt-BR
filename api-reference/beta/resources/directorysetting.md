---
title: tipo de recurso directorySetting
description: As configurações de diretório podem ser criadas com base no directorySettingTemplates disponível e alteradas de seus padrões predefinidos.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c3626d2e63fcea6a536d6dbd18845ea5331b428d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027073"
---
# <a name="directorysetting-resource-type"></a><span data-ttu-id="fda9f-103">tipo de recurso directorySetting</span><span class="sxs-lookup"><span data-stu-id="fda9f-103">directorySetting resource type</span></span>

<span data-ttu-id="fda9f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fda9f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fda9f-105">As configurações de diretório podem ser criadas com base no [directorySettingTemplates](directorysettingtemplate.md)disponível e alteradas de seus padrões predefinidos.</span><span class="sxs-lookup"><span data-stu-id="fda9f-105">Directory settings can be created based on the available [directorySettingTemplates](directorysettingtemplate.md), and changed from their preset defaults.</span></span> <span data-ttu-id="fda9f-106">Essas configurações podem controlar comportamentos de entidade ou de recurso, tanto em um nível de locatário quanto em um nível de entidade específico.</span><span class="sxs-lookup"><span data-stu-id="fda9f-106">These settings can govern entity or feature behaviors, both at a tenant-wide level or at a specific entity level.</span></span> <span data-ttu-id="fda9f-107">Quando a mesma configuração é definida no nível de entidade de todo o locatário e específico, a configuração de nível de entidade específica pode ser recusada a partir da configuração de todo o locatário.</span><span class="sxs-lookup"><span data-stu-id="fda9f-107">When the same setting is defined at both the tenant-wide and specific entity level, the specific entity level setting may opt-out from the tenant-wide setting.</span></span>  <span data-ttu-id="fda9f-108">Por exemplo, a configuração de todos os locatários pode permitir que convidados sejam convidados por membros existentes de grupos, mas uma configuração de grupo específico pode recusar e não permitir que convidados sejam convidados por membros do grupo.</span><span class="sxs-lookup"><span data-stu-id="fda9f-108">For example, the tenant-wide setting may allow guests to be invited by existing members of groups, but a specific group setting may opt-out and not allow guests to be invited by members of the group.</span></span> <span data-ttu-id="fda9f-109">As configurações definidas pelo sistema atualmente são controlar o comportamento de grupos do Office.</span><span class="sxs-lookup"><span data-stu-id="fda9f-109">Currently system defined settings are only govern Office groups behavior.</span></span>

> <span data-ttu-id="fda9f-110">**Observação**: a versão do/beta do tipo de recurso directorySetting só se aplica a grupos.</span><span class="sxs-lookup"><span data-stu-id="fda9f-110">**Note**: The /beta version of the directorySetting resource type only applies to groups.</span></span> <span data-ttu-id="fda9f-111">A versão do/v1.0 foi renomeada como groupSetting.</span><span class="sxs-lookup"><span data-stu-id="fda9f-111">The /v1.0 version has been renamed to groupSetting.</span></span>

## <a name="methods"></a><span data-ttu-id="fda9f-112">Métodos</span><span class="sxs-lookup"><span data-stu-id="fda9f-112">Methods</span></span>

| <span data-ttu-id="fda9f-113">Método</span><span class="sxs-lookup"><span data-stu-id="fda9f-113">Method</span></span>           | <span data-ttu-id="fda9f-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="fda9f-114">Return Type</span></span>    |<span data-ttu-id="fda9f-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="fda9f-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fda9f-116">Criar configuração</span><span class="sxs-lookup"><span data-stu-id="fda9f-116">Create setting</span></span>](../api/directorysetting-post-settings.md) | [<span data-ttu-id="fda9f-117">directorySetting</span><span class="sxs-lookup"><span data-stu-id="fda9f-117">directorySetting</span></span>](directorysetting.md) |<span data-ttu-id="fda9f-118">Criar um objeto Setting com base em um directorySettingTemplate.</span><span class="sxs-lookup"><span data-stu-id="fda9f-118">Create a setting object based on a directorySettingTemplate.</span></span> <span data-ttu-id="fda9f-119">A solicitação POST deve fornecer settingValues para todas as configurações definidas no modelo.</span><span class="sxs-lookup"><span data-stu-id="fda9f-119">The POST request must provide settingValues for all the settings defined in the template.</span></span>|
|[<span data-ttu-id="fda9f-120">Obter configuração</span><span class="sxs-lookup"><span data-stu-id="fda9f-120">Get setting</span></span>](../api/directorysetting-get.md) | [<span data-ttu-id="fda9f-121">directorySetting</span><span class="sxs-lookup"><span data-stu-id="fda9f-121">directorySetting</span></span>](directorysetting.md) |<span data-ttu-id="fda9f-122">Ler propriedades de um objeto de configuração específico.</span><span class="sxs-lookup"><span data-stu-id="fda9f-122">Read properties of a specific setting object.</span></span>|
|[<span data-ttu-id="fda9f-123">Listar configurações</span><span class="sxs-lookup"><span data-stu-id="fda9f-123">List settings</span></span>](../api/directorysetting-list.md) | <span data-ttu-id="fda9f-124">conjunto [directorySetting](directorysetting.md)</span><span class="sxs-lookup"><span data-stu-id="fda9f-124">[directorySetting](directorysetting.md) collection</span></span> |<span data-ttu-id="fda9f-125">Lista propriedades de todos os objetos de configuração.</span><span class="sxs-lookup"><span data-stu-id="fda9f-125">List properties of all setting objects.</span></span>|
|[<span data-ttu-id="fda9f-126">Atualizar configuração</span><span class="sxs-lookup"><span data-stu-id="fda9f-126">Update setting</span></span>](../api/directorysetting-update.md) | [<span data-ttu-id="fda9f-127">directorySetting</span><span class="sxs-lookup"><span data-stu-id="fda9f-127">directorySetting</span></span>](directorysetting.md)  |<span data-ttu-id="fda9f-128">Atualizar um objeto setting.</span><span class="sxs-lookup"><span data-stu-id="fda9f-128">Update a setting object.</span></span> <span data-ttu-id="fda9f-129">Somente settingValues pode ser alterado em uma atualização.</span><span class="sxs-lookup"><span data-stu-id="fda9f-129">Only settingValues can be changed in an update.</span></span>|
|[<span data-ttu-id="fda9f-130">Excluir configuração</span><span class="sxs-lookup"><span data-stu-id="fda9f-130">Delete setting</span></span>](../api/directorysetting-delete.md) | <span data-ttu-id="fda9f-131">None</span><span class="sxs-lookup"><span data-stu-id="fda9f-131">None</span></span> |<span data-ttu-id="fda9f-132">Excluir um objeto de configuração.</span><span class="sxs-lookup"><span data-stu-id="fda9f-132">Delete a setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="fda9f-133">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fda9f-133">Properties</span></span>
| <span data-ttu-id="fda9f-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fda9f-134">Property</span></span>     | <span data-ttu-id="fda9f-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="fda9f-135">Type</span></span>   |<span data-ttu-id="fda9f-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="fda9f-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fda9f-137">displayName</span><span class="sxs-lookup"><span data-stu-id="fda9f-137">displayName</span></span>|<span data-ttu-id="fda9f-138">string</span><span class="sxs-lookup"><span data-stu-id="fda9f-138">string</span></span>|<span data-ttu-id="fda9f-139">Exibe o nome deste grupo de configurações, que vem do modelo associado.</span><span class="sxs-lookup"><span data-stu-id="fda9f-139">Display name of this group of settings, which comes from the associated template.</span></span> <span data-ttu-id="fda9f-140">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fda9f-140">Read-only.</span></span>|
|<span data-ttu-id="fda9f-141">id</span><span class="sxs-lookup"><span data-stu-id="fda9f-141">id</span></span>|<span data-ttu-id="fda9f-142">string</span><span class="sxs-lookup"><span data-stu-id="fda9f-142">string</span></span>| <span data-ttu-id="fda9f-143">Identificador exclusivo dessas configurações.</span><span class="sxs-lookup"><span data-stu-id="fda9f-143">Unique identifier for these settings.</span></span> <span data-ttu-id="fda9f-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fda9f-144">Read-only.</span></span>|
|<span data-ttu-id="fda9f-145">templateId</span><span class="sxs-lookup"><span data-stu-id="fda9f-145">templateId</span></span>|<span data-ttu-id="fda9f-146">string</span><span class="sxs-lookup"><span data-stu-id="fda9f-146">string</span></span>| <span data-ttu-id="fda9f-147">Identificador exclusivo para o modelo usado para criar esse grupo de configurações.</span><span class="sxs-lookup"><span data-stu-id="fda9f-147">Unique identifier for the template used to create this group of settings.</span></span> <span data-ttu-id="fda9f-148">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fda9f-148">Read-only.</span></span>|
|<span data-ttu-id="fda9f-149">values</span><span class="sxs-lookup"><span data-stu-id="fda9f-149">values</span></span>|<span data-ttu-id="fda9f-150">coleção [SettingValue](settingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="fda9f-150">[settingValue](settingvalue.md) collection</span></span>| <span data-ttu-id="fda9f-151">Coleção de pares de valor de nome.</span><span class="sxs-lookup"><span data-stu-id="fda9f-151">Collection of name value pairs.</span></span> <span data-ttu-id="fda9f-152">Deve conter e definir todas as configurações definidas no modelo.</span><span class="sxs-lookup"><span data-stu-id="fda9f-152">Must contain and set all the settings defined in the template.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fda9f-153">Relações</span><span class="sxs-lookup"><span data-stu-id="fda9f-153">Relationships</span></span>
<span data-ttu-id="fda9f-154">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fda9f-154">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="fda9f-155">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fda9f-155">JSON representation</span></span>

<span data-ttu-id="fda9f-156">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fda9f-156">Here is a JSON representation of the resource.</span></span>

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


