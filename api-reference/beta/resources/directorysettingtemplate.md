---
title: tipo de recurso directorySettingTemplate
description: Modelos de configuração de diretório representam configurações definidas pelo sistema disponíveis para o locatário. As configurações de diretório podem ser criadas com base no directorySettingTemplates disponível e os valores alterados de seus padrões predefinidos. Os modelos de configuração de diretório não podem ser criados, atualizados ou excluídos. Essas configurações podem representar configurações de todo o locatário ou podem representar configurações específicas da entidade.  Atualmente, os únicos modelos disponíveis se aplicam aos grupos do Office e incluem configurações como se os usuários podem criar grupos ou convidar convidados de fora da organização para se tornarem membros de um grupo.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f1881c697eae6b4032635d2e4797a14ef2e848e2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42506460"
---
# <a name="directorysettingtemplate-resource-type"></a><span data-ttu-id="03079-107">tipo de recurso directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="03079-107">directorySettingTemplate resource type</span></span>

<span data-ttu-id="03079-108">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="03079-108">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03079-109">Modelos de configuração de diretório representam configurações definidas pelo sistema disponíveis para o locatário.</span><span class="sxs-lookup"><span data-stu-id="03079-109">Directory setting templates represent system-defined settings available to the tenant.</span></span> <span data-ttu-id="03079-110">[As configurações de diretório](directorysetting.md) podem ser criadas com base no directorySettingTemplates disponível e os valores alterados de seus padrões predefinidos.</span><span class="sxs-lookup"><span data-stu-id="03079-110">[Directory settings](directorysetting.md) can be created based on the available directorySettingTemplates, and values changed from their preset defaults.</span></span> <span data-ttu-id="03079-111">Os modelos de configuração de diretório não podem ser criados, atualizados ou excluídos.</span><span class="sxs-lookup"><span data-stu-id="03079-111">Directory setting templates cannot be created, updated or deleted.</span></span> <span data-ttu-id="03079-112">Essas configurações podem representar configurações de todo o locatário ou podem representar configurações específicas da entidade.</span><span class="sxs-lookup"><span data-stu-id="03079-112">These settings can represent tenant-wide settings, or can represent specific entity settings.</span></span>  <span data-ttu-id="03079-113">Atualmente, os únicos modelos disponíveis se aplicam aos grupos do Office e incluem configurações como se os usuários podem criar grupos ou convidar convidados de fora da organização para se tornarem membros de um grupo.</span><span class="sxs-lookup"><span data-stu-id="03079-113">Currently, the only templates available apply to Office groups, and include settings such as whether users can create groups or invite guests from outside the organization to become members of a group.</span></span>

> <span data-ttu-id="03079-114">**Observação**: a versão do/beta do tipo de recurso directorySettingTemplate só se aplica a grupos.</span><span class="sxs-lookup"><span data-stu-id="03079-114">**Note**: The /beta version of the directorySettingTemplate resource type only applies to groups.</span></span> <span data-ttu-id="03079-115">A versão do/v1.0 foi renomeada como groupSettingTemplate.</span><span class="sxs-lookup"><span data-stu-id="03079-115">The /v1.0 version has been renamed to groupSettingTemplate.</span></span>

## <a name="methods"></a><span data-ttu-id="03079-116">Métodos</span><span class="sxs-lookup"><span data-stu-id="03079-116">Methods</span></span>

| <span data-ttu-id="03079-117">Método</span><span class="sxs-lookup"><span data-stu-id="03079-117">Method</span></span>           | <span data-ttu-id="03079-118">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="03079-118">Return Type</span></span>    |<span data-ttu-id="03079-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="03079-119">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="03079-120">Obter directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="03079-120">Get directorySettingTemplate</span></span>](../api/directorysettingtemplate-get.md) | [<span data-ttu-id="03079-121">directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="03079-121">directorySettingTemplate</span></span>](directorysettingtemplate.md) |<span data-ttu-id="03079-122">Leia as propriedades específicas de um dos objetos directorySettingTemplate definidos pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="03079-122">Read the specific properties of one of the system defined directorySettingTemplate objects.</span></span>|
|[<span data-ttu-id="03079-123">Listar directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="03079-123">List directorySettingTemplate</span></span>](../api/directorysettingtemplate-list.md) | [<span data-ttu-id="03079-124">Coleção de directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="03079-124">Collection of directorySettingTemplate</span></span>](directorysettingtemplate.md) |<span data-ttu-id="03079-125">Lista todos os objetos directorySettingTemplate definidos pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="03079-125">List all of the system defined directorySettingTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="03079-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="03079-126">Properties</span></span>
| <span data-ttu-id="03079-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="03079-127">Property</span></span>     | <span data-ttu-id="03079-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="03079-128">Type</span></span>   |<span data-ttu-id="03079-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="03079-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="03079-130">description</span><span class="sxs-lookup"><span data-stu-id="03079-130">description</span></span>|<span data-ttu-id="03079-131">string</span><span class="sxs-lookup"><span data-stu-id="03079-131">string</span></span>|<span data-ttu-id="03079-132">Descrição do modelo.</span><span class="sxs-lookup"><span data-stu-id="03079-132">Description of the template.</span></span> <span data-ttu-id="03079-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="03079-133">Read-only.</span></span>|
|<span data-ttu-id="03079-134">displayName</span><span class="sxs-lookup"><span data-stu-id="03079-134">displayName</span></span>|<span data-ttu-id="03079-135">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="03079-135">string</span></span>|<span data-ttu-id="03079-136">Nome para exibição do modelo.</span><span class="sxs-lookup"><span data-stu-id="03079-136">Display name of the template.</span></span> <span data-ttu-id="03079-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="03079-137">Read-only.</span></span> |
|<span data-ttu-id="03079-138">id</span><span class="sxs-lookup"><span data-stu-id="03079-138">id</span></span>|<span data-ttu-id="03079-139">string</span><span class="sxs-lookup"><span data-stu-id="03079-139">string</span></span>| <span data-ttu-id="03079-140">Identificador exclusivo do modelo.</span><span class="sxs-lookup"><span data-stu-id="03079-140">Unique identifier for the template.</span></span> <span data-ttu-id="03079-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="03079-141">Read-only.</span></span>|
|<span data-ttu-id="03079-142">values</span><span class="sxs-lookup"><span data-stu-id="03079-142">values</span></span>|<span data-ttu-id="03079-143">coleção [settingTemplateValue](settingtemplatevalue.md)</span><span class="sxs-lookup"><span data-stu-id="03079-143">[settingTemplateValue](settingtemplatevalue.md) collection</span></span>| <span data-ttu-id="03079-144">Coleção de settingTemplateValues que lista o conjunto de configurações disponíveis, padrões e tipos que compõem esse modelo.</span><span class="sxs-lookup"><span data-stu-id="03079-144">Collection of settingTemplateValues that list the set of available settings, defaults and types that make up this template.</span></span>  <span data-ttu-id="03079-145">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="03079-145">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="03079-146">Relações</span><span class="sxs-lookup"><span data-stu-id="03079-146">Relationships</span></span>
<span data-ttu-id="03079-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="03079-147">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="03079-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="03079-148">JSON representation</span></span>

<span data-ttu-id="03079-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="03079-149">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directorySettingTemplate"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
  "values": [{"@odata.type": "microsoft.graph.settingTemplateValue"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directorySettingTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
