---
title: tipo de recurso directorySettingTemplate
description: Modelos de configuração de diretório representam configurações definidas pelo sistema disponíveis para o locatário.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 032ddf2ffd557f88a944aafbb72164e2fe356d77
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48010420"
---
# <a name="directorysettingtemplate-resource-type"></a><span data-ttu-id="615f5-103">tipo de recurso directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="615f5-103">directorySettingTemplate resource type</span></span>

<span data-ttu-id="615f5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="615f5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="615f5-105">Modelos de configuração de diretório representam configurações definidas pelo sistema disponíveis para o locatário.</span><span class="sxs-lookup"><span data-stu-id="615f5-105">Directory setting templates represent system-defined settings available to the tenant.</span></span> <span data-ttu-id="615f5-106">[As configurações de diretório](directorysetting.md) podem ser criadas com base no directorySettingTemplates disponível e os valores alterados de seus padrões predefinidos.</span><span class="sxs-lookup"><span data-stu-id="615f5-106">[Directory settings](directorysetting.md) can be created based on the available directorySettingTemplates, and values changed from their preset defaults.</span></span> <span data-ttu-id="615f5-107">Os modelos de configuração de diretório não podem ser criados, atualizados ou excluídos.</span><span class="sxs-lookup"><span data-stu-id="615f5-107">Directory setting templates cannot be created, updated or deleted.</span></span> <span data-ttu-id="615f5-108">Essas configurações podem representar configurações de todo o locatário ou podem representar configurações específicas da entidade.</span><span class="sxs-lookup"><span data-stu-id="615f5-108">These settings can represent tenant-wide settings, or can represent specific entity settings.</span></span>  <span data-ttu-id="615f5-109">Atualmente, os únicos modelos disponíveis se aplicam aos grupos do Office e incluem configurações como se os usuários podem criar grupos ou convidar convidados de fora da organização para se tornarem membros de um grupo.</span><span class="sxs-lookup"><span data-stu-id="615f5-109">Currently, the only templates available apply to Office groups, and include settings such as whether users can create groups or invite guests from outside the organization to become members of a group.</span></span>

> <span data-ttu-id="615f5-110">**Observação**: a versão do/beta do tipo de recurso directorySettingTemplate só se aplica a grupos.</span><span class="sxs-lookup"><span data-stu-id="615f5-110">**Note**: The /beta version of the directorySettingTemplate resource type only applies to groups.</span></span> <span data-ttu-id="615f5-111">A versão do/v1.0 foi renomeada como groupSettingTemplate.</span><span class="sxs-lookup"><span data-stu-id="615f5-111">The /v1.0 version has been renamed to groupSettingTemplate.</span></span>

## <a name="methods"></a><span data-ttu-id="615f5-112">Methods</span><span class="sxs-lookup"><span data-stu-id="615f5-112">Methods</span></span>

| <span data-ttu-id="615f5-113">Método</span><span class="sxs-lookup"><span data-stu-id="615f5-113">Method</span></span>           | <span data-ttu-id="615f5-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="615f5-114">Return Type</span></span>    |<span data-ttu-id="615f5-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="615f5-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="615f5-116">Obter directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="615f5-116">Get directorySettingTemplate</span></span>](../api/directorysettingtemplate-get.md) | [<span data-ttu-id="615f5-117">directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="615f5-117">directorySettingTemplate</span></span>](directorysettingtemplate.md) |<span data-ttu-id="615f5-118">Leia as propriedades específicas de um dos objetos directorySettingTemplate definidos pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="615f5-118">Read the specific properties of one of the system defined directorySettingTemplate objects.</span></span>|
|[<span data-ttu-id="615f5-119">Listar directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="615f5-119">List directorySettingTemplate</span></span>](../api/directorysettingtemplate-list.md) | [<span data-ttu-id="615f5-120">Coleção de directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="615f5-120">Collection of directorySettingTemplate</span></span>](directorysettingtemplate.md) |<span data-ttu-id="615f5-121">Lista todos os objetos directorySettingTemplate definidos pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="615f5-121">List all of the system defined directorySettingTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="615f5-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="615f5-122">Properties</span></span>
| <span data-ttu-id="615f5-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="615f5-123">Property</span></span>     | <span data-ttu-id="615f5-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="615f5-124">Type</span></span>   |<span data-ttu-id="615f5-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="615f5-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="615f5-126">description</span><span class="sxs-lookup"><span data-stu-id="615f5-126">description</span></span>|<span data-ttu-id="615f5-127">string</span><span class="sxs-lookup"><span data-stu-id="615f5-127">string</span></span>|<span data-ttu-id="615f5-128">Descrição do modelo.</span><span class="sxs-lookup"><span data-stu-id="615f5-128">Description of the template.</span></span> <span data-ttu-id="615f5-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="615f5-129">Read-only.</span></span>|
|<span data-ttu-id="615f5-130">displayName</span><span class="sxs-lookup"><span data-stu-id="615f5-130">displayName</span></span>|<span data-ttu-id="615f5-131">string</span><span class="sxs-lookup"><span data-stu-id="615f5-131">string</span></span>|<span data-ttu-id="615f5-132">Nome para exibição do modelo.</span><span class="sxs-lookup"><span data-stu-id="615f5-132">Display name of the template.</span></span> <span data-ttu-id="615f5-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="615f5-133">Read-only.</span></span> |
|<span data-ttu-id="615f5-134">id</span><span class="sxs-lookup"><span data-stu-id="615f5-134">id</span></span>|<span data-ttu-id="615f5-135">string</span><span class="sxs-lookup"><span data-stu-id="615f5-135">string</span></span>| <span data-ttu-id="615f5-136">Identificador exclusivo do modelo.</span><span class="sxs-lookup"><span data-stu-id="615f5-136">Unique identifier for the template.</span></span> <span data-ttu-id="615f5-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="615f5-137">Read-only.</span></span>|
|<span data-ttu-id="615f5-138">values</span><span class="sxs-lookup"><span data-stu-id="615f5-138">values</span></span>|<span data-ttu-id="615f5-139">coleção [settingTemplateValue](settingtemplatevalue.md)</span><span class="sxs-lookup"><span data-stu-id="615f5-139">[settingTemplateValue](settingtemplatevalue.md) collection</span></span>| <span data-ttu-id="615f5-140">Coleção de settingTemplateValues que lista o conjunto de configurações disponíveis, padrões e tipos que compõem esse modelo.</span><span class="sxs-lookup"><span data-stu-id="615f5-140">Collection of settingTemplateValues that list the set of available settings, defaults and types that make up this template.</span></span>  <span data-ttu-id="615f5-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="615f5-141">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="615f5-142">Relações</span><span class="sxs-lookup"><span data-stu-id="615f5-142">Relationships</span></span>
<span data-ttu-id="615f5-143">Nenhum</span><span class="sxs-lookup"><span data-stu-id="615f5-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="615f5-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="615f5-144">JSON representation</span></span>

<span data-ttu-id="615f5-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="615f5-145">Here is a JSON representation of the resource.</span></span>

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


