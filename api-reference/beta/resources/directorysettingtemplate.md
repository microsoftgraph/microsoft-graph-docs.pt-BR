---
title: tipo de recurso directorySettingTemplate
description: Modelos de configuração de diretório representam configurações definidas pelo sistema disponíveis para o locatário. As configurações de diretório podem ser criadas com base no directorySettingTemplates disponível e os valores alterados de seus padrões predefinidos. Os modelos de configuração de diretório não podem ser criados, atualizados ou excluídos. Essas configurações podem representar configurações de todo o locatário ou podem representar configurações específicas da entidade.  Atualmente, os únicos modelos disponíveis se aplicam aos grupos do Office e incluem configurações como se os usuários podem criar grupos ou convidar convidados de fora da organização para se tornarem membros de um grupo.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 366817df422686a8db658f1cab1d5805c24c4f91
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543244"
---
# <a name="directorysettingtemplate-resource-type"></a><span data-ttu-id="84292-107">tipo de recurso directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="84292-107">directorySettingTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84292-108">Modelos de configuração de diretório representam configurações definidas pelo sistema disponíveis para o locatário.</span><span class="sxs-lookup"><span data-stu-id="84292-108">Directory setting templates represent system-defined settings available to the tenant.</span></span> <span data-ttu-id="84292-109">[As configurações de diretório](directorysetting.md) podem ser criadas com base no directorySettingTemplates disponível e os valores alterados de seus padrões predefinidos.</span><span class="sxs-lookup"><span data-stu-id="84292-109">[Directory settings](directorysetting.md) can be created based on the available directorySettingTemplates, and values changed from their preset defaults.</span></span> <span data-ttu-id="84292-110">Os modelos de configuração de diretório não podem ser criados, atualizados ou excluídos.</span><span class="sxs-lookup"><span data-stu-id="84292-110">Directory setting templates cannot be created, updated or deleted.</span></span> <span data-ttu-id="84292-111">Essas configurações podem representar configurações de todo o locatário ou podem representar configurações específicas da entidade.</span><span class="sxs-lookup"><span data-stu-id="84292-111">These settings can represent tenant-wide settings, or can represent specific entity settings.</span></span>  <span data-ttu-id="84292-112">Atualmente, os únicos modelos disponíveis se aplicam aos grupos do Office e incluem configurações como se os usuários podem criar grupos ou convidar convidados de fora da organização para se tornarem membros de um grupo.</span><span class="sxs-lookup"><span data-stu-id="84292-112">Currently, the only templates available apply to Office groups, and include settings such as whether users can create groups or invite guests from outside the organization to become members of a group.</span></span>

> <span data-ttu-id="84292-113">**Observação**: a versão do/beta do tipo de recurso directorySettingTemplate só se aplica a grupos.</span><span class="sxs-lookup"><span data-stu-id="84292-113">**Note**: The /beta version of the directorySettingTemplate resource type only applies to groups.</span></span> <span data-ttu-id="84292-114">A versão do/v1.0 foi renomeada como groupSettingTemplate.</span><span class="sxs-lookup"><span data-stu-id="84292-114">The /v1.0 version has been renamed to groupSettingTemplate.</span></span>

## <a name="methods"></a><span data-ttu-id="84292-115">Métodos</span><span class="sxs-lookup"><span data-stu-id="84292-115">Methods</span></span>

| <span data-ttu-id="84292-116">Método</span><span class="sxs-lookup"><span data-stu-id="84292-116">Method</span></span>           | <span data-ttu-id="84292-117">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="84292-117">Return Type</span></span>    |<span data-ttu-id="84292-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="84292-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="84292-119">Obter directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="84292-119">Get directorySettingTemplate</span></span>](../api/directorysettingtemplate-get.md) | [<span data-ttu-id="84292-120">directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="84292-120">directorySettingTemplate</span></span>](directorysettingtemplate.md) |<span data-ttu-id="84292-121">Leia as propriedades específicas de um dos objetos directorySettingTemplate definidos pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="84292-121">Read the specific properties of one of the system defined directorySettingTemplate objects.</span></span>|
|[<span data-ttu-id="84292-122">Listar directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="84292-122">List directorySettingTemplate</span></span>](../api/directorysettingtemplate-list.md) | [<span data-ttu-id="84292-123">Coleção de directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="84292-123">Collection of directorySettingTemplate</span></span>](directorysettingtemplate.md) |<span data-ttu-id="84292-124">Lista todos os objetos directorySettingTemplate definidos pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="84292-124">List all of the system defined directorySettingTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="84292-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="84292-125">Properties</span></span>
| <span data-ttu-id="84292-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="84292-126">Property</span></span>     | <span data-ttu-id="84292-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="84292-127">Type</span></span>   |<span data-ttu-id="84292-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="84292-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="84292-129">description</span><span class="sxs-lookup"><span data-stu-id="84292-129">description</span></span>|<span data-ttu-id="84292-130">string</span><span class="sxs-lookup"><span data-stu-id="84292-130">string</span></span>|<span data-ttu-id="84292-131">Descrição do modelo.</span><span class="sxs-lookup"><span data-stu-id="84292-131">Description of the template.</span></span> <span data-ttu-id="84292-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="84292-132">Read-only.</span></span>|
|<span data-ttu-id="84292-133">displayName</span><span class="sxs-lookup"><span data-stu-id="84292-133">displayName</span></span>|<span data-ttu-id="84292-134">string</span><span class="sxs-lookup"><span data-stu-id="84292-134">string</span></span>|<span data-ttu-id="84292-135">Nome para exibição do modelo.</span><span class="sxs-lookup"><span data-stu-id="84292-135">Display name of the template.</span></span> <span data-ttu-id="84292-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="84292-136">Read-only.</span></span> |
|<span data-ttu-id="84292-137">id</span><span class="sxs-lookup"><span data-stu-id="84292-137">id</span></span>|<span data-ttu-id="84292-138">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="84292-138">string</span></span>| <span data-ttu-id="84292-139">Identificador exclusivo do modelo.</span><span class="sxs-lookup"><span data-stu-id="84292-139">Unique identifier for the template.</span></span> <span data-ttu-id="84292-140">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="84292-140">Read-only.</span></span>|
|<span data-ttu-id="84292-141">values</span><span class="sxs-lookup"><span data-stu-id="84292-141">values</span></span>|<span data-ttu-id="84292-142">coleção [settingTemplateValue](settingtemplatevalue.md)</span><span class="sxs-lookup"><span data-stu-id="84292-142">[settingTemplateValue](settingtemplatevalue.md) collection</span></span>| <span data-ttu-id="84292-143">Coleção de settingTemplateValues que lista o conjunto de configurações disponíveis, padrões e tipos que compõem esse modelo.</span><span class="sxs-lookup"><span data-stu-id="84292-143">Collection of settingTemplateValues that list the set of available settings, defaults and types that make up this template.</span></span>  <span data-ttu-id="84292-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="84292-144">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="84292-145">Relações</span><span class="sxs-lookup"><span data-stu-id="84292-145">Relationships</span></span>
<span data-ttu-id="84292-146">Nenhum</span><span class="sxs-lookup"><span data-stu-id="84292-146">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="84292-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="84292-147">JSON representation</span></span>

<span data-ttu-id="84292-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="84292-148">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/directorysettingtemplate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
