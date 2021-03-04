---
title: Tipo de recurso directorySetting
description: As configurações de diretório podem ser criadas com base no directorySettingTemplates disponível e alteradas de seus padrões predefinidos.
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 50c73e9c68cd3d2fa3f4aed6c7eba84141443d1a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440448"
---
# <a name="directorysetting-resource-type"></a><span data-ttu-id="a63c8-103">Tipo de recurso directorySetting</span><span class="sxs-lookup"><span data-stu-id="a63c8-103">directorySetting resource type</span></span>

<span data-ttu-id="a63c8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a63c8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a63c8-105">As configurações de diretório podem ser criadas com base no [directorySettingTemplates](directorysettingtemplate.md)disponível e alteradas de seus padrões predefinidos.</span><span class="sxs-lookup"><span data-stu-id="a63c8-105">Directory settings can be created based on the available [directorySettingTemplates](directorysettingtemplate.md), and changed from their preset defaults.</span></span> <span data-ttu-id="a63c8-106">Essas configurações podem reger comportamentos de entidade ou recurso, tanto em um nível de locatário quanto em um nível específico de entidade.</span><span class="sxs-lookup"><span data-stu-id="a63c8-106">These settings can govern entity or feature behaviors, both at a tenant-wide level or at a specific entity level.</span></span> <span data-ttu-id="a63c8-107">Quando a mesma configuração é definida no nível de entidade específica e em todo o locatário, a configuração de nível de entidade específica pode optar pela configuração de todo o locatário.</span><span class="sxs-lookup"><span data-stu-id="a63c8-107">When the same setting is defined at both the tenant-wide and specific entity level, the specific entity level setting may opt-out from the tenant-wide setting.</span></span>  <span data-ttu-id="a63c8-108">Por exemplo, a configuração de todo o locatário pode permitir que os convidados sejam convidados por membros existentes de grupos, mas uma configuração de grupo específica pode optar por não permitir que os convidados sejam convidados pelos membros do grupo.</span><span class="sxs-lookup"><span data-stu-id="a63c8-108">For example, the tenant-wide setting may allow guests to be invited by existing members of groups, but a specific group setting may opt-out and not allow guests to be invited by members of the group.</span></span> <span data-ttu-id="a63c8-109">Atualmente, as configurações definidas pelo sistema são apenas o comportamento de grupos do Office.</span><span class="sxs-lookup"><span data-stu-id="a63c8-109">Currently system defined settings are only govern Office groups behavior.</span></span>

> <span data-ttu-id="a63c8-110">**Observação**: a versão /beta do tipo de recurso directorySetting só se aplica a grupos.</span><span class="sxs-lookup"><span data-stu-id="a63c8-110">**Note**: The /beta version of the directorySetting resource type only applies to groups.</span></span> <span data-ttu-id="a63c8-111">A versão /v1.0 foi renomeada para groupSetting.</span><span class="sxs-lookup"><span data-stu-id="a63c8-111">The /v1.0 version has been renamed to groupSetting.</span></span>

## <a name="methods"></a><span data-ttu-id="a63c8-112">Methods</span><span class="sxs-lookup"><span data-stu-id="a63c8-112">Methods</span></span>

| <span data-ttu-id="a63c8-113">Método</span><span class="sxs-lookup"><span data-stu-id="a63c8-113">Method</span></span>           | <span data-ttu-id="a63c8-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a63c8-114">Return Type</span></span>    |<span data-ttu-id="a63c8-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="a63c8-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a63c8-116">Criar configuração</span><span class="sxs-lookup"><span data-stu-id="a63c8-116">Create setting</span></span>](../api/directorysetting-post-settings.md) | [<span data-ttu-id="a63c8-117">directorySetting</span><span class="sxs-lookup"><span data-stu-id="a63c8-117">directorySetting</span></span>](directorysetting.md) |<span data-ttu-id="a63c8-118">Crie um objeto de configuração com base em um directorySettingTemplate.</span><span class="sxs-lookup"><span data-stu-id="a63c8-118">Create a setting object based on a directorySettingTemplate.</span></span> <span data-ttu-id="a63c8-119">A solicitação POST deve fornecer settingValues para todas as configurações definidas no modelo.</span><span class="sxs-lookup"><span data-stu-id="a63c8-119">The POST request must provide settingValues for all the settings defined in the template.</span></span>|
|[<span data-ttu-id="a63c8-120">Obter configuração</span><span class="sxs-lookup"><span data-stu-id="a63c8-120">Get setting</span></span>](../api/directorysetting-get.md) | [<span data-ttu-id="a63c8-121">directorySetting</span><span class="sxs-lookup"><span data-stu-id="a63c8-121">directorySetting</span></span>](directorysetting.md) |<span data-ttu-id="a63c8-122">Ler propriedades de um objeto de configuração específico.</span><span class="sxs-lookup"><span data-stu-id="a63c8-122">Read properties of a specific setting object.</span></span>|
|[<span data-ttu-id="a63c8-123">Listar configurações</span><span class="sxs-lookup"><span data-stu-id="a63c8-123">List settings</span></span>](../api/directorysetting-list.md) | <span data-ttu-id="a63c8-124">conjunto [directorySetting](directorysetting.md)</span><span class="sxs-lookup"><span data-stu-id="a63c8-124">[directorySetting](directorysetting.md) collection</span></span> |<span data-ttu-id="a63c8-125">Lista propriedades de todos os objetos de configuração.</span><span class="sxs-lookup"><span data-stu-id="a63c8-125">List properties of all setting objects.</span></span>|
|[<span data-ttu-id="a63c8-126">Atualizar configuração</span><span class="sxs-lookup"><span data-stu-id="a63c8-126">Update setting</span></span>](../api/directorysetting-update.md) | [<span data-ttu-id="a63c8-127">directorySetting</span><span class="sxs-lookup"><span data-stu-id="a63c8-127">directorySetting</span></span>](directorysetting.md)  |<span data-ttu-id="a63c8-128">Atualizar um objeto setting.</span><span class="sxs-lookup"><span data-stu-id="a63c8-128">Update a setting object.</span></span> <span data-ttu-id="a63c8-129">Somente settingValues pode ser alterado em uma atualização.</span><span class="sxs-lookup"><span data-stu-id="a63c8-129">Only settingValues can be changed in an update.</span></span>|
|[<span data-ttu-id="a63c8-130">Excluir configuração</span><span class="sxs-lookup"><span data-stu-id="a63c8-130">Delete setting</span></span>](../api/directorysetting-delete.md) | <span data-ttu-id="a63c8-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a63c8-131">None</span></span> |<span data-ttu-id="a63c8-132">Excluir um objeto de configuração.</span><span class="sxs-lookup"><span data-stu-id="a63c8-132">Delete a setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="a63c8-133">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a63c8-133">Properties</span></span>
| <span data-ttu-id="a63c8-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a63c8-134">Property</span></span>     | <span data-ttu-id="a63c8-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="a63c8-135">Type</span></span>   |<span data-ttu-id="a63c8-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="a63c8-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a63c8-137">displayName</span><span class="sxs-lookup"><span data-stu-id="a63c8-137">displayName</span></span>|<span data-ttu-id="a63c8-138">string</span><span class="sxs-lookup"><span data-stu-id="a63c8-138">string</span></span>|<span data-ttu-id="a63c8-139">Nome de exibição desse grupo de configurações, que vem do modelo associado.</span><span class="sxs-lookup"><span data-stu-id="a63c8-139">Display name of this group of settings, which comes from the associated template.</span></span> <span data-ttu-id="a63c8-140">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a63c8-140">Read-only.</span></span>|
|<span data-ttu-id="a63c8-141">id</span><span class="sxs-lookup"><span data-stu-id="a63c8-141">id</span></span>|<span data-ttu-id="a63c8-142">string</span><span class="sxs-lookup"><span data-stu-id="a63c8-142">string</span></span>| <span data-ttu-id="a63c8-143">Identificador exclusivo para essas configurações.</span><span class="sxs-lookup"><span data-stu-id="a63c8-143">Unique identifier for these settings.</span></span> <span data-ttu-id="a63c8-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a63c8-144">Read-only.</span></span>|
|<span data-ttu-id="a63c8-145">templateId</span><span class="sxs-lookup"><span data-stu-id="a63c8-145">templateId</span></span>|<span data-ttu-id="a63c8-146">string</span><span class="sxs-lookup"><span data-stu-id="a63c8-146">string</span></span>| <span data-ttu-id="a63c8-147">Identificador exclusivo do modelo usado para criar esse grupo de configurações.</span><span class="sxs-lookup"><span data-stu-id="a63c8-147">Unique identifier for the template used to create this group of settings.</span></span> <span data-ttu-id="a63c8-148">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a63c8-148">Read-only.</span></span>|
|<span data-ttu-id="a63c8-149">values</span><span class="sxs-lookup"><span data-stu-id="a63c8-149">values</span></span>|<span data-ttu-id="a63c8-150">[coleção settingValue](settingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="a63c8-150">[settingValue](settingvalue.md) collection</span></span>| <span data-ttu-id="a63c8-151">Coleção de pares de valores de nome.</span><span class="sxs-lookup"><span data-stu-id="a63c8-151">Collection of name value pairs.</span></span> <span data-ttu-id="a63c8-152">Deve conter e definir todas as configurações definidas no modelo.</span><span class="sxs-lookup"><span data-stu-id="a63c8-152">Must contain and set all the settings defined in the template.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a63c8-153">Relações</span><span class="sxs-lookup"><span data-stu-id="a63c8-153">Relationships</span></span>
<span data-ttu-id="a63c8-154">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a63c8-154">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="a63c8-155">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a63c8-155">JSON representation</span></span>

<span data-ttu-id="a63c8-156">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a63c8-156">Here is a JSON representation of the resource.</span></span>

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


