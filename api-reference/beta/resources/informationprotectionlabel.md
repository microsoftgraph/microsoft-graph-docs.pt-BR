---
title: Tipo de recurso informationProtectionLabel
description: Descreve o rótulo de proteção de informações que detalha como aplicar corretamente um rótulo de sensibilidade às informações.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 4937d428fd480c0f31a5368a76c4eede9efef851
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953751"
---
# <a name="informationprotectionlabel-resource-type"></a><span data-ttu-id="7751f-103">Tipo de recurso informationProtectionLabel</span><span class="sxs-lookup"><span data-stu-id="7751f-103">informationProtectionLabel resource type</span></span>

<span data-ttu-id="7751f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7751f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7751f-105">Descreve o rótulo de proteção de informações que detalha como aplicar corretamente um rótulo de sensibilidade às informações.</span><span class="sxs-lookup"><span data-stu-id="7751f-105">Describes the information protection label that details how to properly apply a sensitivity label to information.</span></span> <span data-ttu-id="7751f-106">O **recurso informationProtectionLabel** descreve a configuração de rótulos de sensibilidade que se aplicam a um usuário ou locatário.</span><span class="sxs-lookup"><span data-stu-id="7751f-106">The **informationProtectionLabel** resource describes the configuration of sensitivity labels that apply to a user or tenant.</span></span>  

## <a name="methods"></a><span data-ttu-id="7751f-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="7751f-107">Methods</span></span>

| <span data-ttu-id="7751f-108">Método</span><span class="sxs-lookup"><span data-stu-id="7751f-108">Method</span></span>                                                                                              | <span data-ttu-id="7751f-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7751f-109">Return Type</span></span>                                                               | <span data-ttu-id="7751f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7751f-110">Description</span></span>                                                                                                                                                            |
| :-------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------ | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [<span data-ttu-id="7751f-111">Listar informationProtectionLabel</span><span class="sxs-lookup"><span data-stu-id="7751f-111">List informationProtectionLabel</span></span>](../api/informationprotectionpolicy-list-labels.md)                | <span data-ttu-id="7751f-112">[Coleção informationProtectionLabel](informationprotectionlabel.md)</span><span class="sxs-lookup"><span data-stu-id="7751f-112">[informationProtectionLabel](informationprotectionlabel.md) collection</span></span> | <span data-ttu-id="7751f-113">Listar todos os rótulos de proteção de informações configurados para um usuário ou locatário.</span><span class="sxs-lookup"><span data-stu-id="7751f-113">List all configured information protection labels for a user or tenant.</span></span>                                                                                                |
| [<span data-ttu-id="7751f-114">Obter informationProtectionLabel</span><span class="sxs-lookup"><span data-stu-id="7751f-114">Get informationProtectionLabel</span></span>](../api/informationprotectionlabel-get.md)                          | [<span data-ttu-id="7751f-115">informationProtectionLabel</span><span class="sxs-lookup"><span data-stu-id="7751f-115">informationProtectionLabel</span></span>](informationprotectionlabel.md)               | <span data-ttu-id="7751f-116">Dada uma ID de rótulo específica, retorne **informationProtectionLabel**.</span><span class="sxs-lookup"><span data-stu-id="7751f-116">Given a specific label ID, return the **informationProtectionLabel**.</span></span>                                                                                                  |
| [<span data-ttu-id="7751f-117">evaluateapplication</span><span class="sxs-lookup"><span data-stu-id="7751f-117">evaluateapplication</span></span>](../api/informationprotectionlabel-evaluateapplication.md)                     | <span data-ttu-id="7751f-118">[Coleção informationProtectionAction](informationprotectionaction.md)</span><span class="sxs-lookup"><span data-stu-id="7751f-118">[informationProtectionAction](informationprotectionaction.md) collection</span></span>  | <span data-ttu-id="7751f-119">Dada uma entrada [de contentInfo](contentinfo.md) e [labelingOptions](labelingoptions.md), calcule o conjunto de ações necessárias para aplicar o rótulo.</span><span class="sxs-lookup"><span data-stu-id="7751f-119">Given an input of [contentInfo](contentinfo.md) and [labelingOptions](labelingoptions.md), compute the set of actions require to apply the label.</span></span>                      |
| [<span data-ttu-id="7751f-120">evaluateClassificationResults</span><span class="sxs-lookup"><span data-stu-id="7751f-120">evaluateClassificationResults</span></span>](../api/informationprotectionlabel-evaluateclassificationresults.md) | <span data-ttu-id="7751f-121">[Coleção informationProtectionAction](informationprotectionaction.md)</span><span class="sxs-lookup"><span data-stu-id="7751f-121">[informationProtectionAction](informationprotectionaction.md) collection</span></span>  | <span data-ttu-id="7751f-122">Dada uma entrada de [contentInfo](contentinfo.md) e resultados de classificação, calcule o conjunto de ações necessárias para aplicar o rótulo.</span><span class="sxs-lookup"><span data-stu-id="7751f-122">Given an input of [contentInfo](contentinfo.md) and classification results, compute the set of actions require to apply the label.</span></span>                                  |
| [<span data-ttu-id="7751f-123">evaluateRemoval</span><span class="sxs-lookup"><span data-stu-id="7751f-123">evaluateRemoval</span></span>](../api/informationprotectionlabel-evaluateremoval.md)                             | <span data-ttu-id="7751f-124">[Coleção informationProtectionAction](informationprotectionaction.md)</span><span class="sxs-lookup"><span data-stu-id="7751f-124">[informationProtectionAction](informationprotectionaction.md) collection</span></span>  | <span data-ttu-id="7751f-125">Dada uma entrada [de contentInfo](contentinfo.md) e [downgradeJustification](downgradejustification.md), calcule as ações que devem ser tomadas para remover o rótulo.</span><span class="sxs-lookup"><span data-stu-id="7751f-125">Given an input of [contentInfo](contentinfo.md) and [downgradeJustification](downgradejustification.md), compute the actions that should be taken to remove the label.</span></span> |
| [<span data-ttu-id="7751f-126">extractLabel</span><span class="sxs-lookup"><span data-stu-id="7751f-126">extractLabel</span></span>](../api/informationprotectionlabel-extractlabel.md)                                   | [<span data-ttu-id="7751f-127">informationProtectionContentLabel</span><span class="sxs-lookup"><span data-stu-id="7751f-127">informationProtectionContentLabel</span></span>](informationprotectioncontentlabel.md) | <span data-ttu-id="7751f-128">Dada uma entrada de [contentInfo](contentinfo.md), retorne detalhes sobre [informationProtectionLabel](informationprotectionlabel.md) que os metadados representam.</span><span class="sxs-lookup"><span data-stu-id="7751f-128">Given an input of [contentInfo](contentinfo.md), return details on the [informationProtectionLabel](informationprotectionlabel.md) that the metadata represents.</span></span>       |

## <a name="properties"></a><span data-ttu-id="7751f-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7751f-129">Properties</span></span>

| <span data-ttu-id="7751f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7751f-130">Property</span></span>    | <span data-ttu-id="7751f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7751f-131">Type</span></span>    | <span data-ttu-id="7751f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7751f-132">Description</span></span>                                                                                     |
| :---------- | :------ | :---------------------------------------------------------------------------------------------- |
| <span data-ttu-id="7751f-133">color</span><span class="sxs-lookup"><span data-stu-id="7751f-133">color</span></span>       | <span data-ttu-id="7751f-134">String</span><span class="sxs-lookup"><span data-stu-id="7751f-134">String</span></span>  | <span data-ttu-id="7751f-135">A cor que a interface do usuário deve exibir para o rótulo, se configurada.</span><span class="sxs-lookup"><span data-stu-id="7751f-135">The color that the UI should display for the label, if configured.</span></span>                              |
| <span data-ttu-id="7751f-136">description</span><span class="sxs-lookup"><span data-stu-id="7751f-136">description</span></span> | <span data-ttu-id="7751f-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7751f-137">String</span></span>  | <span data-ttu-id="7751f-138">A descrição definida pelo administrador para o rótulo.</span><span class="sxs-lookup"><span data-stu-id="7751f-138">The admin-defined description for the label.</span></span>                                                    |
| <span data-ttu-id="7751f-139">id</span><span class="sxs-lookup"><span data-stu-id="7751f-139">id</span></span>          | <span data-ttu-id="7751f-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7751f-140">String</span></span>  | <span data-ttu-id="7751f-141">A ID do rótulo é um identificador global exclusivo (GUID)</span><span class="sxs-lookup"><span data-stu-id="7751f-141">The label ID is a globally unique identifier (GUID)</span></span>                                             |
| <span data-ttu-id="7751f-142">isActive</span><span class="sxs-lookup"><span data-stu-id="7751f-142">isActive</span></span>    | <span data-ttu-id="7751f-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="7751f-143">Boolean</span></span> | <span data-ttu-id="7751f-144">Indica se o rótulo está ativo ou não.</span><span class="sxs-lookup"><span data-stu-id="7751f-144">Indicates whether the label is active or not.</span></span> <span data-ttu-id="7751f-145">Os rótulos ativos devem ser ocultos ou desabilitados na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="7751f-145">Active labels should be hidden or disabled in UI.</span></span> |
| <span data-ttu-id="7751f-146">nome</span><span class="sxs-lookup"><span data-stu-id="7751f-146">name</span></span>        | <span data-ttu-id="7751f-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7751f-147">String</span></span>  | <span data-ttu-id="7751f-148">O nome do texto sem formatção do rótulo.</span><span class="sxs-lookup"><span data-stu-id="7751f-148">The plaintext name of the label.</span></span>                                                                |
| <span data-ttu-id="7751f-149">sensibilidade</span><span class="sxs-lookup"><span data-stu-id="7751f-149">sensitivity</span></span> | <span data-ttu-id="7751f-150">Int32</span><span class="sxs-lookup"><span data-stu-id="7751f-150">Int32</span></span>   | <span data-ttu-id="7751f-151">O valor de sensibilidade do rótulo, onde menor é menos sensível.</span><span class="sxs-lookup"><span data-stu-id="7751f-151">The sensitivity value of the label, where lower is less sensitive.</span></span>                              |
| <span data-ttu-id="7751f-152">tooltip</span><span class="sxs-lookup"><span data-stu-id="7751f-152">tooltip</span></span>     | <span data-ttu-id="7751f-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7751f-153">String</span></span>  | <span data-ttu-id="7751f-154">A dica de ferramenta que deve ser exibida para o rótulo em uma interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="7751f-154">The tooltip that should be displayed for the label in a UI.</span></span>                                     |

## <a name="relationships"></a><span data-ttu-id="7751f-155">Relações</span><span class="sxs-lookup"><span data-stu-id="7751f-155">Relationships</span></span>

<span data-ttu-id="7751f-156">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7751f-156">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7751f-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7751f-157">JSON representation</span></span>

<span data-ttu-id="7751f-158">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7751f-158">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.informationProtectionLabel",
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


