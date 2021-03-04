---
title: Tipo de recurso directorySettingTemplate
description: Os modelos de configuração de diretório representam configurações definidas pelo sistema disponíveis para o locatário.
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 71984d472aab9f78197134fae0668fd0a90d7716
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440406"
---
# <a name="directorysettingtemplate-resource-type"></a><span data-ttu-id="6951d-103">Tipo de recurso directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="6951d-103">directorySettingTemplate resource type</span></span>

<span data-ttu-id="6951d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6951d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6951d-105">Os modelos de configuração de diretório representam configurações definidas pelo sistema disponíveis para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6951d-105">Directory setting templates represent system-defined settings available to the tenant.</span></span> <span data-ttu-id="6951d-106">[As configurações de](directorysetting.md) diretório podem ser criadas com base nos directorySettingTemplates disponíveis e valores alterados de seus padrões predefinidos.</span><span class="sxs-lookup"><span data-stu-id="6951d-106">[Directory settings](directorysetting.md) can be created based on the available directorySettingTemplates, and values changed from their preset defaults.</span></span> <span data-ttu-id="6951d-107">Modelos de configuração de diretório não podem ser criados, atualizados ou excluídos.</span><span class="sxs-lookup"><span data-stu-id="6951d-107">Directory setting templates cannot be created, updated or deleted.</span></span> <span data-ttu-id="6951d-108">Essas configurações podem representar configurações de todo o locatário ou podem representar configurações de entidade específicas.</span><span class="sxs-lookup"><span data-stu-id="6951d-108">These settings can represent tenant-wide settings, or can represent specific entity settings.</span></span>  <span data-ttu-id="6951d-109">Atualmente, os únicos modelos disponíveis se aplicam a grupos do Office e incluem configurações como se os usuários podem criar grupos ou convidar convidados de fora da organização para se tornarem membros de um grupo.</span><span class="sxs-lookup"><span data-stu-id="6951d-109">Currently, the only templates available apply to Office groups, and include settings such as whether users can create groups or invite guests from outside the organization to become members of a group.</span></span>

> <span data-ttu-id="6951d-110">**Observação**: a versão /beta do tipo de recurso directorySettingTemplate só se aplica a grupos.</span><span class="sxs-lookup"><span data-stu-id="6951d-110">**Note**: The /beta version of the directorySettingTemplate resource type only applies to groups.</span></span> <span data-ttu-id="6951d-111">A versão /v1.0 foi renomeada para groupSettingTemplate.</span><span class="sxs-lookup"><span data-stu-id="6951d-111">The /v1.0 version has been renamed to groupSettingTemplate.</span></span>

## <a name="methods"></a><span data-ttu-id="6951d-112">Methods</span><span class="sxs-lookup"><span data-stu-id="6951d-112">Methods</span></span>

| <span data-ttu-id="6951d-113">Método</span><span class="sxs-lookup"><span data-stu-id="6951d-113">Method</span></span>           | <span data-ttu-id="6951d-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6951d-114">Return Type</span></span>    |<span data-ttu-id="6951d-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="6951d-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6951d-116">Obter directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="6951d-116">Get directorySettingTemplate</span></span>](../api/directorysettingtemplate-get.md) | [<span data-ttu-id="6951d-117">directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="6951d-117">directorySettingTemplate</span></span>](directorysettingtemplate.md) |<span data-ttu-id="6951d-118">Leia as propriedades específicas de um dos objetos directorySettingTemplate definidos pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="6951d-118">Read the specific properties of one of the system defined directorySettingTemplate objects.</span></span>|
|[<span data-ttu-id="6951d-119">Listar directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="6951d-119">List directorySettingTemplate</span></span>](../api/directorysettingtemplate-list.md) | [<span data-ttu-id="6951d-120">Coleção de directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="6951d-120">Collection of directorySettingTemplate</span></span>](directorysettingtemplate.md) |<span data-ttu-id="6951d-121">Listar todos os objetos directorySettingTemplate definidos pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="6951d-121">List all of the system defined directorySettingTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="6951d-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6951d-122">Properties</span></span>
| <span data-ttu-id="6951d-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6951d-123">Property</span></span>     | <span data-ttu-id="6951d-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="6951d-124">Type</span></span>   |<span data-ttu-id="6951d-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="6951d-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6951d-126">description</span><span class="sxs-lookup"><span data-stu-id="6951d-126">description</span></span>|<span data-ttu-id="6951d-127">string</span><span class="sxs-lookup"><span data-stu-id="6951d-127">string</span></span>|<span data-ttu-id="6951d-128">Descrição do modelo.</span><span class="sxs-lookup"><span data-stu-id="6951d-128">Description of the template.</span></span> <span data-ttu-id="6951d-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6951d-129">Read-only.</span></span>|
|<span data-ttu-id="6951d-130">displayName</span><span class="sxs-lookup"><span data-stu-id="6951d-130">displayName</span></span>|<span data-ttu-id="6951d-131">string</span><span class="sxs-lookup"><span data-stu-id="6951d-131">string</span></span>|<span data-ttu-id="6951d-132">Nome de exibição do modelo.</span><span class="sxs-lookup"><span data-stu-id="6951d-132">Display name of the template.</span></span> <span data-ttu-id="6951d-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6951d-133">Read-only.</span></span> |
|<span data-ttu-id="6951d-134">id</span><span class="sxs-lookup"><span data-stu-id="6951d-134">id</span></span>|<span data-ttu-id="6951d-135">string</span><span class="sxs-lookup"><span data-stu-id="6951d-135">string</span></span>| <span data-ttu-id="6951d-136">Identificador exclusivo do modelo.</span><span class="sxs-lookup"><span data-stu-id="6951d-136">Unique identifier for the template.</span></span> <span data-ttu-id="6951d-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6951d-137">Read-only.</span></span>|
|<span data-ttu-id="6951d-138">values</span><span class="sxs-lookup"><span data-stu-id="6951d-138">values</span></span>|<span data-ttu-id="6951d-139">[Coleção settingTemplateValue](settingtemplatevalue.md)</span><span class="sxs-lookup"><span data-stu-id="6951d-139">[settingTemplateValue](settingtemplatevalue.md) collection</span></span>| <span data-ttu-id="6951d-140">Coleção de settingTemplateValues que lista o conjunto de configurações, padrões e tipos disponíveis que comem esse modelo.</span><span class="sxs-lookup"><span data-stu-id="6951d-140">Collection of settingTemplateValues that list the set of available settings, defaults and types that make up this template.</span></span>  <span data-ttu-id="6951d-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6951d-141">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="6951d-142">Relações</span><span class="sxs-lookup"><span data-stu-id="6951d-142">Relationships</span></span>
<span data-ttu-id="6951d-143">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6951d-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="6951d-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6951d-144">JSON representation</span></span>

<span data-ttu-id="6951d-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6951d-145">Here is a JSON representation of the resource.</span></span>

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


