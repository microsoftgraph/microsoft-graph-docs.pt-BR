---
title: tipo de recurso directorySettingTemplate
description: Modelos de configuração de diretório representam configurações definidas pelo sistema disponíveis para o locatário. As configurações de diretório podem ser criadas com base no directorySettingTemplates disponível e os valores alterados de seus padrões predefinidos. Os modelos de configuração de diretório não podem ser criados, atualizados ou excluídos. Essas configurações podem representar configurações de todo o locatário ou podem representar configurações específicas da entidade.  Atualmente, os únicos modelos disponíveis se aplicam aos grupos do Office e incluem configurações como se os usuários podem criar grupos ou convidar convidados de fora da organização para se tornarem membros de um grupo.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4239a12be5fffbf5c579752c3de4998c88749bd3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012783"
---
# <a name="directorysettingtemplate-resource-type"></a><span data-ttu-id="c4a5b-107">tipo de recurso directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="c4a5b-107">directorySettingTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4a5b-108">Modelos de configuração de diretório representam configurações definidas pelo sistema disponíveis para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c4a5b-108">Directory setting templates represent system-defined settings available to the tenant.</span></span> <span data-ttu-id="c4a5b-109">[As configurações de diretório](directorysetting.md) podem ser criadas com base no directorySettingTemplates disponível e os valores alterados de seus padrões predefinidos.</span><span class="sxs-lookup"><span data-stu-id="c4a5b-109">[Directory settings](directorysetting.md) can be created based on the available directorySettingTemplates, and values changed from their preset defaults.</span></span> <span data-ttu-id="c4a5b-110">Os modelos de configuração de diretório não podem ser criados, atualizados ou excluídos.</span><span class="sxs-lookup"><span data-stu-id="c4a5b-110">Directory setting templates cannot be created, updated or deleted.</span></span> <span data-ttu-id="c4a5b-111">Essas configurações podem representar configurações de todo o locatário ou podem representar configurações específicas da entidade.</span><span class="sxs-lookup"><span data-stu-id="c4a5b-111">These settings can represent tenant-wide settings, or can represent specific entity settings.</span></span>  <span data-ttu-id="c4a5b-112">Atualmente, os únicos modelos disponíveis se aplicam aos grupos do Office e incluem configurações como se os usuários podem criar grupos ou convidar convidados de fora da organização para se tornarem membros de um grupo.</span><span class="sxs-lookup"><span data-stu-id="c4a5b-112">Currently, the only templates available apply to Office groups, and include settings such as whether users can create groups or invite guests from outside the organization to become members of a group.</span></span>

> <span data-ttu-id="c4a5b-113">**Observação**: a versão do/beta do tipo de recurso directorySettingTemplate só se aplica a grupos.</span><span class="sxs-lookup"><span data-stu-id="c4a5b-113">**Note**: The /beta version of the directorySettingTemplate resource type only applies to groups.</span></span> <span data-ttu-id="c4a5b-114">A versão do/v1.0 foi renomeada como groupSettingTemplate.</span><span class="sxs-lookup"><span data-stu-id="c4a5b-114">The /v1.0 version has been renamed to groupSettingTemplate.</span></span>

## <a name="methods"></a><span data-ttu-id="c4a5b-115">Métodos</span><span class="sxs-lookup"><span data-stu-id="c4a5b-115">Methods</span></span>

| <span data-ttu-id="c4a5b-116">Método</span><span class="sxs-lookup"><span data-stu-id="c4a5b-116">Method</span></span>           | <span data-ttu-id="c4a5b-117">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c4a5b-117">Return Type</span></span>    |<span data-ttu-id="c4a5b-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4a5b-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c4a5b-119">Obter directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="c4a5b-119">Get directorySettingTemplate</span></span>](../api/directorysettingtemplate-get.md) | [<span data-ttu-id="c4a5b-120">directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="c4a5b-120">directorySettingTemplate</span></span>](directorysettingtemplate.md) |<span data-ttu-id="c4a5b-121">Leia as propriedades específicas de um dos objetos directorySettingTemplate definidos pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="c4a5b-121">Read the specific properties of one of the system defined directorySettingTemplate objects.</span></span>|
|[<span data-ttu-id="c4a5b-122">Listar directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="c4a5b-122">List directorySettingTemplate</span></span>](../api/directorysettingtemplate-list.md) | [<span data-ttu-id="c4a5b-123">Coleção de directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="c4a5b-123">Collection of directorySettingTemplate</span></span>](directorysettingtemplate.md) |<span data-ttu-id="c4a5b-124">Lista todos os objetos directorySettingTemplate definidos pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="c4a5b-124">List all of the system defined directorySettingTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="c4a5b-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c4a5b-125">Properties</span></span>
| <span data-ttu-id="c4a5b-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c4a5b-126">Property</span></span>     | <span data-ttu-id="c4a5b-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="c4a5b-127">Type</span></span>   |<span data-ttu-id="c4a5b-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4a5b-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c4a5b-129">description</span><span class="sxs-lookup"><span data-stu-id="c4a5b-129">description</span></span>|<span data-ttu-id="c4a5b-130">string</span><span class="sxs-lookup"><span data-stu-id="c4a5b-130">string</span></span>|<span data-ttu-id="c4a5b-131">Descrição do modelo.</span><span class="sxs-lookup"><span data-stu-id="c4a5b-131">Description of the template.</span></span> <span data-ttu-id="c4a5b-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c4a5b-132">Read-only.</span></span>|
|<span data-ttu-id="c4a5b-133">displayName</span><span class="sxs-lookup"><span data-stu-id="c4a5b-133">displayName</span></span>|<span data-ttu-id="c4a5b-134">string</span><span class="sxs-lookup"><span data-stu-id="c4a5b-134">string</span></span>|<span data-ttu-id="c4a5b-135">Nome para exibição do modelo.</span><span class="sxs-lookup"><span data-stu-id="c4a5b-135">Display name of the template.</span></span> <span data-ttu-id="c4a5b-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c4a5b-136">Read-only.</span></span> |
|<span data-ttu-id="c4a5b-137">id</span><span class="sxs-lookup"><span data-stu-id="c4a5b-137">id</span></span>|<span data-ttu-id="c4a5b-138">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c4a5b-138">string</span></span>| <span data-ttu-id="c4a5b-139">Identificador exclusivo do modelo.</span><span class="sxs-lookup"><span data-stu-id="c4a5b-139">Unique identifier for the template.</span></span> <span data-ttu-id="c4a5b-140">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c4a5b-140">Read-only.</span></span>|
|<span data-ttu-id="c4a5b-141">values</span><span class="sxs-lookup"><span data-stu-id="c4a5b-141">values</span></span>|<span data-ttu-id="c4a5b-142">coleção [settingTemplateValue](settingtemplatevalue.md)</span><span class="sxs-lookup"><span data-stu-id="c4a5b-142">[settingTemplateValue](settingtemplatevalue.md) collection</span></span>| <span data-ttu-id="c4a5b-143">Coleção de settingTemplateValues que lista o conjunto de configurações disponíveis, padrões e tipos que compõem esse modelo.</span><span class="sxs-lookup"><span data-stu-id="c4a5b-143">Collection of settingTemplateValues that list the set of available settings, defaults and types that make up this template.</span></span>  <span data-ttu-id="c4a5b-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c4a5b-144">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="c4a5b-145">Relações</span><span class="sxs-lookup"><span data-stu-id="c4a5b-145">Relationships</span></span>
<span data-ttu-id="c4a5b-146">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c4a5b-146">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="c4a5b-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c4a5b-147">JSON representation</span></span>

<span data-ttu-id="c4a5b-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c4a5b-148">Here is a JSON representation of the resource.</span></span>

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
