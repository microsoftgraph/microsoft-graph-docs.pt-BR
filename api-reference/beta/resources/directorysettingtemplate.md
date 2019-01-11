---
title: tipo de recurso de directorySettingTemplate
description: Modelos de configuração de diretório representam as configurações definidas pelo sistema disponíveis para o inquilino. Configurações do diretório podem ser criadas com base nos directorySettingTemplates disponíveis e valores alterados de seus padrões predefinidas. Modelos de configuração do diretório não podem ser criados, atualizados ou excluídos. Essas configurações podem representar as configurações de todo o locatário, ou podem representar as configurações de entidade específica.  Atualmente, os únicos modelos disponíveis se aplicam a grupos do Office e incluem configurações como se os usuários podem criar grupos ou convidar pessoas de fora da organização para se tornar membros de um grupo.
localization_priority: Normal
ms.openlocfilehash: e0df923854059723ee83380f7aa0f6425cf2afb9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806143"
---
# <a name="directorysettingtemplate-resource-type"></a><span data-ttu-id="f21e3-107">tipo de recurso de directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="f21e3-107">directorySettingTemplate resource type</span></span>

> <span data-ttu-id="f21e3-108">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f21e3-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f21e3-109">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f21e3-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f21e3-110">Modelos de configuração de diretório representam as configurações definidas pelo sistema disponíveis para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="f21e3-110">Directory setting templates represent system-defined settings available to the tenant.</span></span> <span data-ttu-id="f21e3-111">[Configurações do diretório](directorysetting.md) podem ser criados com base nos directorySettingTemplates disponíveis e valores alterados de seus padrões predefinidas.</span><span class="sxs-lookup"><span data-stu-id="f21e3-111">[Directory settings](directorysetting.md) can be created based on the available directorySettingTemplates, and values changed from their preset defaults.</span></span> <span data-ttu-id="f21e3-112">Modelos de configuração do diretório não podem ser criados, atualizados ou excluídos.</span><span class="sxs-lookup"><span data-stu-id="f21e3-112">Directory setting templates cannot be created, updated or deleted.</span></span> <span data-ttu-id="f21e3-113">Essas configurações podem representar as configurações de todo o locatário, ou podem representar as configurações de entidade específica.</span><span class="sxs-lookup"><span data-stu-id="f21e3-113">These settings can represent tenant-wide settings, or can represent specific entity settings.</span></span>  <span data-ttu-id="f21e3-114">Atualmente, os únicos modelos disponíveis se aplicam a grupos do Office e incluem configurações como se os usuários podem criar grupos ou convidar pessoas de fora da organização para se tornar membros de um grupo.</span><span class="sxs-lookup"><span data-stu-id="f21e3-114">Currently, the only templates available apply to Office groups, and include settings such as whether users can create groups or invite guests from outside the organization to become members of a group.</span></span>

> <span data-ttu-id="f21e3-115">**Observação**: A versão /beta do tipo de recurso directorySettingTemplate se aplica apenas aos grupos.</span><span class="sxs-lookup"><span data-stu-id="f21e3-115">**Note**: The /beta version of the directorySettingTemplate resource type only applies to groups.</span></span> <span data-ttu-id="f21e3-116">A versão /v1.0 foi renomeada para groupSettingTemplate.</span><span class="sxs-lookup"><span data-stu-id="f21e3-116">The /v1.0 version has been renamed to groupSettingTemplate.</span></span>

## <a name="methods"></a><span data-ttu-id="f21e3-117">Métodos</span><span class="sxs-lookup"><span data-stu-id="f21e3-117">Methods</span></span>

| <span data-ttu-id="f21e3-118">Método</span><span class="sxs-lookup"><span data-stu-id="f21e3-118">Method</span></span>           | <span data-ttu-id="f21e3-119">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f21e3-119">Return Type</span></span>    |<span data-ttu-id="f21e3-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f21e3-120">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f21e3-121">Obter directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="f21e3-121">Get directorySettingTemplate</span></span>](../api/directorysettingtemplate-get.md) | [<span data-ttu-id="f21e3-122">directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="f21e3-122">directorySettingTemplate</span></span>](directorysettingtemplate.md) |<span data-ttu-id="f21e3-123">Leia as propriedades específicas de um dos objetos directorySettingTemplate definidas pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="f21e3-123">Read the specific properties of one of the system defined directorySettingTemplate objects.</span></span>|
|[<span data-ttu-id="f21e3-124">Lista directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="f21e3-124">List directorySettingTemplate</span></span>](../api/directorysettingtemplate-list.md) | [<span data-ttu-id="f21e3-125">Coleção de directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="f21e3-125">Collection of directorySettingTemplate</span></span>](directorysettingtemplate.md) |<span data-ttu-id="f21e3-126">Liste todos os objetos directorySettingTemplate definidas pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="f21e3-126">List all of the system defined directorySettingTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="f21e3-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f21e3-127">Properties</span></span>
| <span data-ttu-id="f21e3-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f21e3-128">Property</span></span>     | <span data-ttu-id="f21e3-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="f21e3-129">Type</span></span>   |<span data-ttu-id="f21e3-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="f21e3-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f21e3-131">description</span><span class="sxs-lookup"><span data-stu-id="f21e3-131">description</span></span>|<span data-ttu-id="f21e3-132">string</span><span class="sxs-lookup"><span data-stu-id="f21e3-132">string</span></span>|<span data-ttu-id="f21e3-133">Descrição do modelo.</span><span class="sxs-lookup"><span data-stu-id="f21e3-133">Description of the template.</span></span> <span data-ttu-id="f21e3-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f21e3-134">Read-only.</span></span>|
|<span data-ttu-id="f21e3-135">displayName</span><span class="sxs-lookup"><span data-stu-id="f21e3-135">displayName</span></span>|<span data-ttu-id="f21e3-136">string</span><span class="sxs-lookup"><span data-stu-id="f21e3-136">string</span></span>|<span data-ttu-id="f21e3-137">Nome para exibição do modelo</span><span class="sxs-lookup"><span data-stu-id="f21e3-137">Display name of the template.</span></span> <span data-ttu-id="f21e3-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f21e3-138">Read-only.</span></span> |
|<span data-ttu-id="f21e3-139">id</span><span class="sxs-lookup"><span data-stu-id="f21e3-139">id</span></span>|<span data-ttu-id="f21e3-140">string</span><span class="sxs-lookup"><span data-stu-id="f21e3-140">string</span></span>| <span data-ttu-id="f21e3-p107">O identificador exclusivo do modelo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f21e3-p107">Unique identifier for the template. Read-only.</span></span>|
|<span data-ttu-id="f21e3-143">values</span><span class="sxs-lookup"><span data-stu-id="f21e3-143">values</span></span>|<span data-ttu-id="f21e3-144">Conjunto [settingTemplateValue](settingtemplatevalue.md)</span><span class="sxs-lookup"><span data-stu-id="f21e3-144">[settingTemplateValue](settingtemplatevalue.md) collection</span></span>| <span data-ttu-id="f21e3-145">Coleção de settingTemplateValues que lista o conjunto de configurações disponíveis, padrões e tipos que compõem este modelo.</span><span class="sxs-lookup"><span data-stu-id="f21e3-145">Collection of settingTemplateValues that list the set of available settings, defaults and types that make up this template.</span></span>  <span data-ttu-id="f21e3-146">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f21e3-146">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="f21e3-147">Relações</span><span class="sxs-lookup"><span data-stu-id="f21e3-147">Relationships</span></span>
<span data-ttu-id="f21e3-148">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f21e3-148">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="f21e3-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f21e3-149">JSON representation</span></span>

<span data-ttu-id="f21e3-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f21e3-150">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "directorySettingTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
