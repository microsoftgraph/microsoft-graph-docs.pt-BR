---
title: tipo de recurso informationProtectionLabel
description: Descreve o rótulo de proteção de informações que detalha como aplicar corretamente um rótulo de confidencialidade às informações.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 528238d904ac9807027dd51a8c59ed03570c7bc3
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938741"
---
# <a name="informationprotectionlabel-resource-type"></a><span data-ttu-id="5b339-103">tipo de recurso informationProtectionLabel</span><span class="sxs-lookup"><span data-stu-id="5b339-103">informationProtectionLabel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b339-104">Descreve o rótulo de proteção de informações que detalha como aplicar corretamente um rótulo de confidencialidade às informações.</span><span class="sxs-lookup"><span data-stu-id="5b339-104">Describes the information protection label that details how to properly apply a sensitivity label to information.</span></span> <span data-ttu-id="5b339-105">O recurso **informationProtectionLabel** descreve a configuração de rótulos de confidencialidade que se aplicam a um usuário ou locatário.</span><span class="sxs-lookup"><span data-stu-id="5b339-105">The **informationProtectionLabel** resource describes the configuration of sensitivity labels that apply to a user or tenant.</span></span>  

## <a name="methods"></a><span data-ttu-id="5b339-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="5b339-106">Methods</span></span>

| <span data-ttu-id="5b339-107">Método</span><span class="sxs-lookup"><span data-stu-id="5b339-107">Method</span></span>                                                                                              | <span data-ttu-id="5b339-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5b339-108">Return Type</span></span>                                                               | <span data-ttu-id="5b339-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b339-109">Description</span></span>                                                                                                                                                            |
| :-------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------ | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [<span data-ttu-id="5b339-110">Listar informationProtectionLabel</span><span class="sxs-lookup"><span data-stu-id="5b339-110">List informationProtectionLabel</span></span>](../api/informationprotectionpolicy-list-labels.md)                | <span data-ttu-id="5b339-111">coleção [informationProtectionLabel](informationprotectionlabel.md)</span><span class="sxs-lookup"><span data-stu-id="5b339-111">[informationProtectionLabel](informationprotectionlabel.md) collection</span></span> | <span data-ttu-id="5b339-112">Listar todos os rótulos de proteção de informações configurados para um usuário ou locatário.</span><span class="sxs-lookup"><span data-stu-id="5b339-112">List all configured information protection labels for a user or tenant.</span></span>                                                                                                |
| [<span data-ttu-id="5b339-113">Obter informationProtectionLabel</span><span class="sxs-lookup"><span data-stu-id="5b339-113">Get informationProtectionLabel</span></span>](../api/informationprotectionlabel-get.md)                          | [<span data-ttu-id="5b339-114">informationProtectionLabel</span><span class="sxs-lookup"><span data-stu-id="5b339-114">informationProtectionLabel</span></span>](informationprotectionlabel.md)               | <span data-ttu-id="5b339-115">Dada uma ID de etiqueta específica, retorne o **informationProtectionLabel**.</span><span class="sxs-lookup"><span data-stu-id="5b339-115">Given a specific label ID, return the **informationProtectionLabel**.</span></span>                                                                                                  |
| [<span data-ttu-id="5b339-116">evaluateapplication</span><span class="sxs-lookup"><span data-stu-id="5b339-116">evaluateapplication</span></span>](../api/informationprotectionlabel-evaluateapplication.md)                     | <span data-ttu-id="5b339-117">coleção [informationProtectionAction](informationprotectionaction.md)</span><span class="sxs-lookup"><span data-stu-id="5b339-117">[informationProtectionAction](informationprotectionaction.md) collection</span></span>  | <span data-ttu-id="5b339-118">Dada uma entrada de [contentInfo](contentinfo.md) e [labelingOptions](labelingoptions.md), COMPUTE o conjunto de ações necessárias para aplicar o rótulo.</span><span class="sxs-lookup"><span data-stu-id="5b339-118">Given an input of [contentInfo](contentinfo.md) and [labelingOptions](labelingoptions.md), compute the set of actions require to apply the label.</span></span>                      |
| [<span data-ttu-id="5b339-119">evaluateClassificationResults</span><span class="sxs-lookup"><span data-stu-id="5b339-119">evaluateClassificationResults</span></span>](../api/informationprotectionlabel-evaluateclassificationresults.md) | <span data-ttu-id="5b339-120">coleção [informationProtectionAction](informationprotectionaction.md)</span><span class="sxs-lookup"><span data-stu-id="5b339-120">[informationProtectionAction](informationprotectionaction.md) collection</span></span>  | <span data-ttu-id="5b339-121">Dada uma entrada de [contentInfo](contentinfo.md) e resultados de classificação, COMPUTE o conjunto de ações necessárias para aplicar o rótulo.</span><span class="sxs-lookup"><span data-stu-id="5b339-121">Given an input of [contentInfo](contentinfo.md) and classification results, compute the set of actions require to apply the label.</span></span>                                  |
| [<span data-ttu-id="5b339-122">evaluateRemoval</span><span class="sxs-lookup"><span data-stu-id="5b339-122">evaluateRemoval</span></span>](../api/informationprotectionlabel-evaluateremoval.md)                             | <span data-ttu-id="5b339-123">coleção [informationProtectionAction](informationprotectionaction.md)</span><span class="sxs-lookup"><span data-stu-id="5b339-123">[informationProtectionAction](informationprotectionaction.md) collection</span></span>  | <span data-ttu-id="5b339-124">Dada uma entrada de [contentInfo](contentinfo.md) e [downgradeJustification](downgradejustification.md), calcule as ações que devem ser executadas para remover o rótulo.</span><span class="sxs-lookup"><span data-stu-id="5b339-124">Given an input of [contentInfo](contentinfo.md) and [downgradeJustification](downgradejustification.md), compute the actions that should be taken to remove the label.</span></span> |
| [<span data-ttu-id="5b339-125">extractLabel</span><span class="sxs-lookup"><span data-stu-id="5b339-125">extractLabel</span></span>](../api/informationprotectionlabel-extractlabel.md)                                   | [<span data-ttu-id="5b339-126">informationProtectionContentLabel</span><span class="sxs-lookup"><span data-stu-id="5b339-126">informationProtectionContentLabel</span></span>](informationprotectioncontentlabel.md) | <span data-ttu-id="5b339-127">Dada uma entrada de [contentInfo](contentinfo.md), detalhes de retorno no [informationProtectionLabel](informationprotectionlabel.md) que os metadados representam.</span><span class="sxs-lookup"><span data-stu-id="5b339-127">Given an input of [contentInfo](contentinfo.md), return details on the [informationProtectionLabel](informationprotectionlabel.md) that the metadata represents.</span></span>       |

## <a name="properties"></a><span data-ttu-id="5b339-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5b339-128">Properties</span></span>

| <span data-ttu-id="5b339-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5b339-129">Property</span></span>    | <span data-ttu-id="5b339-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="5b339-130">Type</span></span>    | <span data-ttu-id="5b339-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b339-131">Description</span></span>                                                                                     |
| :---------- | :------ | :---------------------------------------------------------------------------------------------- |
| <span data-ttu-id="5b339-132">color</span><span class="sxs-lookup"><span data-stu-id="5b339-132">color</span></span>       | <span data-ttu-id="5b339-133">String</span><span class="sxs-lookup"><span data-stu-id="5b339-133">String</span></span>  | <span data-ttu-id="5b339-134">A cor que a interface do usuário deve exibir para o rótulo, se configurada.</span><span class="sxs-lookup"><span data-stu-id="5b339-134">The color that the UI should display for the label, if configured.</span></span>                              |
| <span data-ttu-id="5b339-135">description</span><span class="sxs-lookup"><span data-stu-id="5b339-135">description</span></span> | <span data-ttu-id="5b339-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5b339-136">String</span></span>  | <span data-ttu-id="5b339-137">A descrição definida pelo administrador para o rótulo.</span><span class="sxs-lookup"><span data-stu-id="5b339-137">The admin-defined description for the label.</span></span>                                                    |
| <span data-ttu-id="5b339-138">id</span><span class="sxs-lookup"><span data-stu-id="5b339-138">id</span></span>          | <span data-ttu-id="5b339-139">String</span><span class="sxs-lookup"><span data-stu-id="5b339-139">String</span></span>  | <span data-ttu-id="5b339-140">A ID do rótulo é um identificador global exclusivo (GUID)</span><span class="sxs-lookup"><span data-stu-id="5b339-140">The label ID is a globally unique identifier (GUID)</span></span>                                             |
| <span data-ttu-id="5b339-141">isActive</span><span class="sxs-lookup"><span data-stu-id="5b339-141">isActive</span></span>    | <span data-ttu-id="5b339-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="5b339-142">Boolean</span></span> | <span data-ttu-id="5b339-143">Indica se o rótulo está ativo ou não.</span><span class="sxs-lookup"><span data-stu-id="5b339-143">Indicates whether the label is active or not.</span></span> <span data-ttu-id="5b339-144">Os rótulos ativos devem ser ocultos ou desabilitados na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="5b339-144">Active labels should be hidden or disabled in UI.</span></span> |
| <span data-ttu-id="5b339-145">name</span><span class="sxs-lookup"><span data-stu-id="5b339-145">name</span></span>        | <span data-ttu-id="5b339-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5b339-146">String</span></span>  | <span data-ttu-id="5b339-147">O nome de texto não criptografado do rótulo.</span><span class="sxs-lookup"><span data-stu-id="5b339-147">The plaintext name of the label.</span></span>                                                                |
| <span data-ttu-id="5b339-148">sensitivity</span><span class="sxs-lookup"><span data-stu-id="5b339-148">sensitivity</span></span> | <span data-ttu-id="5b339-149">Int32</span><span class="sxs-lookup"><span data-stu-id="5b339-149">Int32</span></span>   | <span data-ttu-id="5b339-150">O valor de confidencialidade do rótulo, onde inferior é menos confidencial.</span><span class="sxs-lookup"><span data-stu-id="5b339-150">The sensitivity value of the label, where lower is less sensitive.</span></span>                              |
| <span data-ttu-id="5b339-151">tooltip</span><span class="sxs-lookup"><span data-stu-id="5b339-151">tooltip</span></span>     | <span data-ttu-id="5b339-152">String</span><span class="sxs-lookup"><span data-stu-id="5b339-152">String</span></span>  | <span data-ttu-id="5b339-153">A dica de ferramenta que deve ser exibida para o rótulo em uma interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="5b339-153">The tooltip that should be displayed for the label in a UI.</span></span>                                     |

## <a name="relationships"></a><span data-ttu-id="5b339-154">Relações</span><span class="sxs-lookup"><span data-stu-id="5b339-154">Relationships</span></span>

<span data-ttu-id="5b339-155">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5b339-155">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5b339-156">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5b339-156">JSON representation</span></span>

<span data-ttu-id="5b339-157">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5b339-157">The following is a JSON representation of the resource.</span></span>

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
