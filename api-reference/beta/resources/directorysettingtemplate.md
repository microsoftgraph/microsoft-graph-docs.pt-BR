---
title: tipo de recurso de directorySettingTemplate
description: Modelos de configuração de diretório representam as configurações definidas pelo sistema disponíveis para o inquilino. Configurações do diretório podem ser criadas com base nos directorySettingTemplates disponíveis e valores alterados de seus padrões predefinidas. Modelos de configuração do diretório não podem ser criados, atualizados ou excluídos. Essas configurações podem representar as configurações de todo o locatário, ou podem representar as configurações de entidade específica.  Atualmente, os únicos modelos disponíveis se aplicam a grupos do Office e incluem configurações como se os usuários podem criar grupos ou convidar pessoas de fora da organização para se tornar membros de um grupo.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 366817df422686a8db658f1cab1d5805c24c4f91
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516655"
---
# <a name="directorysettingtemplate-resource-type"></a><span data-ttu-id="26450-107">tipo de recurso de directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="26450-107">directorySettingTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26450-108">Modelos de configuração de diretório representam as configurações definidas pelo sistema disponíveis para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="26450-108">Directory setting templates represent system-defined settings available to the tenant.</span></span> <span data-ttu-id="26450-109">[Configurações do diretório](directorysetting.md) podem ser criados com base nos directorySettingTemplates disponíveis e valores alterados de seus padrões predefinidas.</span><span class="sxs-lookup"><span data-stu-id="26450-109">[Directory settings](directorysetting.md) can be created based on the available directorySettingTemplates, and values changed from their preset defaults.</span></span> <span data-ttu-id="26450-110">Modelos de configuração do diretório não podem ser criados, atualizados ou excluídos.</span><span class="sxs-lookup"><span data-stu-id="26450-110">Directory setting templates cannot be created, updated or deleted.</span></span> <span data-ttu-id="26450-111">Essas configurações podem representar as configurações de todo o locatário, ou podem representar as configurações de entidade específica.</span><span class="sxs-lookup"><span data-stu-id="26450-111">These settings can represent tenant-wide settings, or can represent specific entity settings.</span></span>  <span data-ttu-id="26450-112">Atualmente, os únicos modelos disponíveis se aplicam a grupos do Office e incluem configurações como se os usuários podem criar grupos ou convidar pessoas de fora da organização para se tornar membros de um grupo.</span><span class="sxs-lookup"><span data-stu-id="26450-112">Currently, the only templates available apply to Office groups, and include settings such as whether users can create groups or invite guests from outside the organization to become members of a group.</span></span>

> <span data-ttu-id="26450-113">**Observação**: A versão /beta do tipo de recurso directorySettingTemplate se aplica apenas aos grupos.</span><span class="sxs-lookup"><span data-stu-id="26450-113">**Note**: The /beta version of the directorySettingTemplate resource type only applies to groups.</span></span> <span data-ttu-id="26450-114">A versão /v1.0 foi renomeada para groupSettingTemplate.</span><span class="sxs-lookup"><span data-stu-id="26450-114">The /v1.0 version has been renamed to groupSettingTemplate.</span></span>

## <a name="methods"></a><span data-ttu-id="26450-115">Métodos</span><span class="sxs-lookup"><span data-stu-id="26450-115">Methods</span></span>

| <span data-ttu-id="26450-116">Método</span><span class="sxs-lookup"><span data-stu-id="26450-116">Method</span></span>           | <span data-ttu-id="26450-117">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="26450-117">Return Type</span></span>    |<span data-ttu-id="26450-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="26450-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="26450-119">Obter directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="26450-119">Get directorySettingTemplate</span></span>](../api/directorysettingtemplate-get.md) | [<span data-ttu-id="26450-120">directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="26450-120">directorySettingTemplate</span></span>](directorysettingtemplate.md) |<span data-ttu-id="26450-121">Leia as propriedades específicas de um dos objetos directorySettingTemplate definidas pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="26450-121">Read the specific properties of one of the system defined directorySettingTemplate objects.</span></span>|
|[<span data-ttu-id="26450-122">Lista directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="26450-122">List directorySettingTemplate</span></span>](../api/directorysettingtemplate-list.md) | [<span data-ttu-id="26450-123">Coleção de directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="26450-123">Collection of directorySettingTemplate</span></span>](directorysettingtemplate.md) |<span data-ttu-id="26450-124">Liste todos os objetos directorySettingTemplate definidas pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="26450-124">List all of the system defined directorySettingTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="26450-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="26450-125">Properties</span></span>
| <span data-ttu-id="26450-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="26450-126">Property</span></span>     | <span data-ttu-id="26450-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="26450-127">Type</span></span>   |<span data-ttu-id="26450-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="26450-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="26450-129">description</span><span class="sxs-lookup"><span data-stu-id="26450-129">description</span></span>|<span data-ttu-id="26450-130">string</span><span class="sxs-lookup"><span data-stu-id="26450-130">string</span></span>|<span data-ttu-id="26450-131">Descrição do modelo.</span><span class="sxs-lookup"><span data-stu-id="26450-131">Description of the template.</span></span> <span data-ttu-id="26450-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="26450-132">Read-only.</span></span>|
|<span data-ttu-id="26450-133">displayName</span><span class="sxs-lookup"><span data-stu-id="26450-133">displayName</span></span>|<span data-ttu-id="26450-134">string</span><span class="sxs-lookup"><span data-stu-id="26450-134">string</span></span>|<span data-ttu-id="26450-135">Nome para exibição do modelo</span><span class="sxs-lookup"><span data-stu-id="26450-135">Display name of the template.</span></span> <span data-ttu-id="26450-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="26450-136">Read-only.</span></span> |
|<span data-ttu-id="26450-137">id</span><span class="sxs-lookup"><span data-stu-id="26450-137">id</span></span>|<span data-ttu-id="26450-138">string</span><span class="sxs-lookup"><span data-stu-id="26450-138">string</span></span>| <span data-ttu-id="26450-p106">O identificador exclusivo do modelo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="26450-p106">Unique identifier for the template. Read-only.</span></span>|
|<span data-ttu-id="26450-141">values</span><span class="sxs-lookup"><span data-stu-id="26450-141">values</span></span>|<span data-ttu-id="26450-142">Conjunto [settingTemplateValue](settingtemplatevalue.md)</span><span class="sxs-lookup"><span data-stu-id="26450-142">[settingTemplateValue](settingtemplatevalue.md) collection</span></span>| <span data-ttu-id="26450-143">Coleção de settingTemplateValues que lista o conjunto de configurações disponíveis, padrões e tipos que compõem este modelo.</span><span class="sxs-lookup"><span data-stu-id="26450-143">Collection of settingTemplateValues that list the set of available settings, defaults and types that make up this template.</span></span>  <span data-ttu-id="26450-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="26450-144">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="26450-145">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="26450-145">Relationships</span></span>
<span data-ttu-id="26450-146">Nenhum</span><span class="sxs-lookup"><span data-stu-id="26450-146">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="26450-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="26450-147">JSON representation</span></span>

<span data-ttu-id="26450-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="26450-148">Here is a JSON representation of the resource.</span></span>

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
