---
title: tipo de recurso informationProtectionLabel
description: Descreve o rótulo de proteção de informações que detalha como aplicar corretamente um rótulo de confidencialidade às informações.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8b634166896932897b200d2eeb17a1e54aadb543
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021921"
---
# <a name="informationprotectionlabel-resource-type"></a><span data-ttu-id="db432-103">tipo de recurso informationProtectionLabel</span><span class="sxs-lookup"><span data-stu-id="db432-103">informationProtectionLabel resource type</span></span>

<span data-ttu-id="db432-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db432-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db432-105">Descreve o rótulo de proteção de informações que detalha como aplicar corretamente um rótulo de confidencialidade às informações.</span><span class="sxs-lookup"><span data-stu-id="db432-105">Describes the information protection label that details how to properly apply a sensitivity label to information.</span></span> <span data-ttu-id="db432-106">O recurso **informationProtectionLabel** descreve a configuração de rótulos de confidencialidade que se aplicam a um usuário ou locatário.</span><span class="sxs-lookup"><span data-stu-id="db432-106">The **informationProtectionLabel** resource describes the configuration of sensitivity labels that apply to a user or tenant.</span></span>  

## <a name="methods"></a><span data-ttu-id="db432-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="db432-107">Methods</span></span>

| <span data-ttu-id="db432-108">Método</span><span class="sxs-lookup"><span data-stu-id="db432-108">Method</span></span>                                                                                              | <span data-ttu-id="db432-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="db432-109">Return Type</span></span>                                                               | <span data-ttu-id="db432-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="db432-110">Description</span></span>                                                                                                                                                            |
| :-------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------ | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [<span data-ttu-id="db432-111">Listar informationProtectionLabel</span><span class="sxs-lookup"><span data-stu-id="db432-111">List informationProtectionLabel</span></span>](../api/informationprotectionpolicy-list-labels.md)                | <span data-ttu-id="db432-112">coleção [informationProtectionLabel](informationprotectionlabel.md)</span><span class="sxs-lookup"><span data-stu-id="db432-112">[informationProtectionLabel](informationprotectionlabel.md) collection</span></span> | <span data-ttu-id="db432-113">Listar todos os rótulos de proteção de informações configurados para um usuário ou locatário.</span><span class="sxs-lookup"><span data-stu-id="db432-113">List all configured information protection labels for a user or tenant.</span></span>                                                                                                |
| [<span data-ttu-id="db432-114">Obter informationProtectionLabel</span><span class="sxs-lookup"><span data-stu-id="db432-114">Get informationProtectionLabel</span></span>](../api/informationprotectionlabel-get.md)                          | [<span data-ttu-id="db432-115">informationProtectionLabel</span><span class="sxs-lookup"><span data-stu-id="db432-115">informationProtectionLabel</span></span>](informationprotectionlabel.md)               | <span data-ttu-id="db432-116">Dada uma ID de etiqueta específica, retorne o **informationProtectionLabel**.</span><span class="sxs-lookup"><span data-stu-id="db432-116">Given a specific label ID, return the **informationProtectionLabel**.</span></span>                                                                                                  |
| [<span data-ttu-id="db432-117">evaluateapplication</span><span class="sxs-lookup"><span data-stu-id="db432-117">evaluateapplication</span></span>](../api/informationprotectionlabel-evaluateapplication.md)                     | <span data-ttu-id="db432-118">coleção [informationProtectionAction](informationprotectionaction.md)</span><span class="sxs-lookup"><span data-stu-id="db432-118">[informationProtectionAction](informationprotectionaction.md) collection</span></span>  | <span data-ttu-id="db432-119">Dada uma entrada de [contentInfo](contentinfo.md) e [labelingOptions](labelingoptions.md), COMPUTE o conjunto de ações necessárias para aplicar o rótulo.</span><span class="sxs-lookup"><span data-stu-id="db432-119">Given an input of [contentInfo](contentinfo.md) and [labelingOptions](labelingoptions.md), compute the set of actions require to apply the label.</span></span>                      |
| [<span data-ttu-id="db432-120">evaluateClassificationResults</span><span class="sxs-lookup"><span data-stu-id="db432-120">evaluateClassificationResults</span></span>](../api/informationprotectionlabel-evaluateclassificationresults.md) | <span data-ttu-id="db432-121">coleção [informationProtectionAction](informationprotectionaction.md)</span><span class="sxs-lookup"><span data-stu-id="db432-121">[informationProtectionAction](informationprotectionaction.md) collection</span></span>  | <span data-ttu-id="db432-122">Dada uma entrada de [contentInfo](contentinfo.md) e resultados de classificação, COMPUTE o conjunto de ações necessárias para aplicar o rótulo.</span><span class="sxs-lookup"><span data-stu-id="db432-122">Given an input of [contentInfo](contentinfo.md) and classification results, compute the set of actions require to apply the label.</span></span>                                  |
| [<span data-ttu-id="db432-123">evaluateRemoval</span><span class="sxs-lookup"><span data-stu-id="db432-123">evaluateRemoval</span></span>](../api/informationprotectionlabel-evaluateremoval.md)                             | <span data-ttu-id="db432-124">coleção [informationProtectionAction](informationprotectionaction.md)</span><span class="sxs-lookup"><span data-stu-id="db432-124">[informationProtectionAction](informationprotectionaction.md) collection</span></span>  | <span data-ttu-id="db432-125">Dada uma entrada de [contentInfo](contentinfo.md) e [downgradeJustification](downgradejustification.md), calcule as ações que devem ser executadas para remover o rótulo.</span><span class="sxs-lookup"><span data-stu-id="db432-125">Given an input of [contentInfo](contentinfo.md) and [downgradeJustification](downgradejustification.md), compute the actions that should be taken to remove the label.</span></span> |
| [<span data-ttu-id="db432-126">extractLabel</span><span class="sxs-lookup"><span data-stu-id="db432-126">extractLabel</span></span>](../api/informationprotectionlabel-extractlabel.md)                                   | [<span data-ttu-id="db432-127">informationProtectionContentLabel</span><span class="sxs-lookup"><span data-stu-id="db432-127">informationProtectionContentLabel</span></span>](informationprotectioncontentlabel.md) | <span data-ttu-id="db432-128">Dada uma entrada de [contentInfo](contentinfo.md), detalhes de retorno no [informationProtectionLabel](informationprotectionlabel.md) que os metadados representam.</span><span class="sxs-lookup"><span data-stu-id="db432-128">Given an input of [contentInfo](contentinfo.md), return details on the [informationProtectionLabel](informationprotectionlabel.md) that the metadata represents.</span></span>       |

## <a name="properties"></a><span data-ttu-id="db432-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="db432-129">Properties</span></span>

| <span data-ttu-id="db432-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="db432-130">Property</span></span>    | <span data-ttu-id="db432-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="db432-131">Type</span></span>    | <span data-ttu-id="db432-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="db432-132">Description</span></span>                                                                                     |
| :---------- | :------ | :---------------------------------------------------------------------------------------------- |
| <span data-ttu-id="db432-133">color</span><span class="sxs-lookup"><span data-stu-id="db432-133">color</span></span>       | <span data-ttu-id="db432-134">String</span><span class="sxs-lookup"><span data-stu-id="db432-134">String</span></span>  | <span data-ttu-id="db432-135">A cor que a interface do usuário deve exibir para o rótulo, se configurada.</span><span class="sxs-lookup"><span data-stu-id="db432-135">The color that the UI should display for the label, if configured.</span></span>                              |
| <span data-ttu-id="db432-136">description</span><span class="sxs-lookup"><span data-stu-id="db432-136">description</span></span> | <span data-ttu-id="db432-137">String</span><span class="sxs-lookup"><span data-stu-id="db432-137">String</span></span>  | <span data-ttu-id="db432-138">A descrição definida pelo administrador para o rótulo.</span><span class="sxs-lookup"><span data-stu-id="db432-138">The admin-defined description for the label.</span></span>                                                    |
| <span data-ttu-id="db432-139">id</span><span class="sxs-lookup"><span data-stu-id="db432-139">id</span></span>          | <span data-ttu-id="db432-140">String</span><span class="sxs-lookup"><span data-stu-id="db432-140">String</span></span>  | <span data-ttu-id="db432-141">A ID do rótulo é um identificador global exclusivo (GUID)</span><span class="sxs-lookup"><span data-stu-id="db432-141">The label ID is a globally unique identifier (GUID)</span></span>                                             |
| <span data-ttu-id="db432-142">isActive</span><span class="sxs-lookup"><span data-stu-id="db432-142">isActive</span></span>    | <span data-ttu-id="db432-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="db432-143">Boolean</span></span> | <span data-ttu-id="db432-144">Indica se o rótulo está ativo ou não.</span><span class="sxs-lookup"><span data-stu-id="db432-144">Indicates whether the label is active or not.</span></span> <span data-ttu-id="db432-145">Os rótulos ativos devem ser ocultos ou desabilitados na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="db432-145">Active labels should be hidden or disabled in UI.</span></span> |
| <span data-ttu-id="db432-146">nome</span><span class="sxs-lookup"><span data-stu-id="db432-146">name</span></span>        | <span data-ttu-id="db432-147">String</span><span class="sxs-lookup"><span data-stu-id="db432-147">String</span></span>  | <span data-ttu-id="db432-148">O nome de texto não criptografado do rótulo.</span><span class="sxs-lookup"><span data-stu-id="db432-148">The plaintext name of the label.</span></span>                                                                |
| <span data-ttu-id="db432-149">sensibilidade</span><span class="sxs-lookup"><span data-stu-id="db432-149">sensitivity</span></span> | <span data-ttu-id="db432-150">Int32</span><span class="sxs-lookup"><span data-stu-id="db432-150">Int32</span></span>   | <span data-ttu-id="db432-151">O valor de confidencialidade do rótulo, onde inferior é menos confidencial.</span><span class="sxs-lookup"><span data-stu-id="db432-151">The sensitivity value of the label, where lower is less sensitive.</span></span>                              |
| <span data-ttu-id="db432-152">tooltip</span><span class="sxs-lookup"><span data-stu-id="db432-152">tooltip</span></span>     | <span data-ttu-id="db432-153">String</span><span class="sxs-lookup"><span data-stu-id="db432-153">String</span></span>  | <span data-ttu-id="db432-154">A dica de ferramenta que deve ser exibida para o rótulo em uma interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="db432-154">The tooltip that should be displayed for the label in a UI.</span></span>                                     |

## <a name="relationships"></a><span data-ttu-id="db432-155">Relações</span><span class="sxs-lookup"><span data-stu-id="db432-155">Relationships</span></span>

<span data-ttu-id="db432-156">Nenhum</span><span class="sxs-lookup"><span data-stu-id="db432-156">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="db432-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="db432-157">JSON representation</span></span>

<span data-ttu-id="db432-158">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="db432-158">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.informationProtectionLabel",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "color": "String",
  "description": "String",
  "id": "String (identifier)",
  "isActive": true,
  "name": "String",
  "sensitivity": 1024,
  "tooltip": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "informationProtectionLabel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


