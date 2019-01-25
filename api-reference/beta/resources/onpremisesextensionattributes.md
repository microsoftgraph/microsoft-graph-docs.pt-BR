---
title: tipo de recurso de onPremisesExtensionAttributes
description: A propriedade **onPremisesExtensionAttributes** da entidade do usuário contém quinze propriedades de atributo de extensão personalizada. Para um usuário onPremisesSyncEnabled, esse conjunto de propriedades é masterizado no Active Directory local e sincronizado com o Azure Active Directory e é somente leitura. Para um usuário somente na nuvem (onde onPremisesSyncEnabled é falso), essas propriedades podem ser definidas durante a criação ou atualização.
localization_priority: Normal
ms.openlocfilehash: f44f71fdcd86d2165289282568a2d7153ccc99b1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518237"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="11742-105">tipo de recurso de onPremisesExtensionAttributes</span><span class="sxs-lookup"><span data-stu-id="11742-105">onPremisesExtensionAttributes resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11742-106">A propriedade **onPremisesExtensionAttributes** da entidade do [usuário](user.md) contém quinze propriedades de atributo de extensão personalizada.</span><span class="sxs-lookup"><span data-stu-id="11742-106">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="11742-107">Para um usuário onPremisesSyncEnabled, esse conjunto de propriedades é masterizado no Active Directory local e sincronizado com o Azure Active Directory e é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="11742-107">For an **onPremisesSyncEnabled** user, this set of properties is mastered in on-premises Active Directory and synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="11742-108">Para um usuário somente na nuvem (onde onPremisesSyncEnabled é falso), essas propriedades podem ser definidas durante a criação ou atualização.</span><span class="sxs-lookup"><span data-stu-id="11742-108">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties may be set during creation or update.</span></span>


## <a name="properties"></a><span data-ttu-id="11742-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="11742-109">Properties</span></span>
| <span data-ttu-id="11742-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="11742-110">Property</span></span>     | <span data-ttu-id="11742-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="11742-111">Type</span></span>   |<span data-ttu-id="11742-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="11742-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="11742-113">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="11742-113">extensionAttribute1</span></span>|<span data-ttu-id="11742-114">String</span><span class="sxs-lookup"><span data-stu-id="11742-114">String</span></span>| <span data-ttu-id="11742-115">Primeiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="11742-115">First customizable extension attribute.</span></span> |
|<span data-ttu-id="11742-116">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="11742-116">extensionAttribute2</span></span>|<span data-ttu-id="11742-117">String</span><span class="sxs-lookup"><span data-stu-id="11742-117">String</span></span>| <span data-ttu-id="11742-118">Segundo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="11742-118">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="11742-119">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="11742-119">extensionAttribute3</span></span>|<span data-ttu-id="11742-120">String</span><span class="sxs-lookup"><span data-stu-id="11742-120">String</span></span>| <span data-ttu-id="11742-121">Atributo do terceiro extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="11742-121">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="11742-122">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="11742-122">extensionAttribute4</span></span>|<span data-ttu-id="11742-123">String</span><span class="sxs-lookup"><span data-stu-id="11742-123">String</span></span>| <span data-ttu-id="11742-124">Quarto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="11742-124">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="11742-125">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="11742-125">extensionAttribute5</span></span>|<span data-ttu-id="11742-126">String</span><span class="sxs-lookup"><span data-stu-id="11742-126">String</span></span>| <span data-ttu-id="11742-127">Atributo do quinto extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="11742-127">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="11742-128">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="11742-128">extensionAttribute6</span></span>|<span data-ttu-id="11742-129">String</span><span class="sxs-lookup"><span data-stu-id="11742-129">String</span></span>| <span data-ttu-id="11742-130">Sexto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="11742-130">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="11742-131">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="11742-131">extensionAttribute7</span></span>|<span data-ttu-id="11742-132">String</span><span class="sxs-lookup"><span data-stu-id="11742-132">String</span></span>| <span data-ttu-id="11742-133">Sétimo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="11742-133">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="11742-134">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="11742-134">extensionAttribute8</span></span>|<span data-ttu-id="11742-135">String</span><span class="sxs-lookup"><span data-stu-id="11742-135">String</span></span>| <span data-ttu-id="11742-136">Oitavo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="11742-136">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="11742-137">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="11742-137">extensionAttribute9</span></span>|<span data-ttu-id="11742-138">String</span><span class="sxs-lookup"><span data-stu-id="11742-138">String</span></span>| <span data-ttu-id="11742-139">Nono atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="11742-139">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="11742-140">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="11742-140">extensionAttribute10</span></span>|<span data-ttu-id="11742-141">String</span><span class="sxs-lookup"><span data-stu-id="11742-141">String</span></span>| <span data-ttu-id="11742-142">Décimo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="11742-142">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="11742-143">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="11742-143">extensionAttribute11</span></span>|<span data-ttu-id="11742-144">String</span><span class="sxs-lookup"><span data-stu-id="11742-144">String</span></span>| <span data-ttu-id="11742-145">Atributo de extensão Décima primeira personalizável.</span><span class="sxs-lookup"><span data-stu-id="11742-145">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="11742-146">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="11742-146">extensionAttribute12</span></span>|<span data-ttu-id="11742-147">String</span><span class="sxs-lookup"><span data-stu-id="11742-147">String</span></span>| <span data-ttu-id="11742-148">Atributo de extensão Décima segunda personalizável.</span><span class="sxs-lookup"><span data-stu-id="11742-148">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="11742-149">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="11742-149">extensionAttribute13</span></span>|<span data-ttu-id="11742-150">String</span><span class="sxs-lookup"><span data-stu-id="11742-150">String</span></span>| <span data-ttu-id="11742-151">Atributo de extensão Décima terceira personalizável.</span><span class="sxs-lookup"><span data-stu-id="11742-151">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="11742-152">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="11742-152">extensionAttribute14</span></span>|<span data-ttu-id="11742-153">String</span><span class="sxs-lookup"><span data-stu-id="11742-153">String</span></span>| <span data-ttu-id="11742-154">Atributo de extensão décima quarta personalizável.</span><span class="sxs-lookup"><span data-stu-id="11742-154">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="11742-155">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="11742-155">extensionAttribute15</span></span>|<span data-ttu-id="11742-156">String</span><span class="sxs-lookup"><span data-stu-id="11742-156">String</span></span>| <span data-ttu-id="11742-157">Atributo de extensão Décima quinta personalizável.</span><span class="sxs-lookup"><span data-stu-id="11742-157">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="11742-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="11742-158">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesExtensionAttributes"
}-->


```json
{
      "extensionAttribute1": "string",
      "extensionAttribute2": "string",
      "extensionAttribute3": "string",
      "extensionAttribute4": "string",
      "extensionAttribute5": "string",
      "extensionAttribute6": "string",
      "extensionAttribute7": "string",
      "extensionAttribute8": "string",
      "extensionAttribute9": "string",
      "extensionAttribute10": "string",
      "extensionAttribute11": "string",
      "extensionAttribute12": "string",
      "extensionAttribute13": "string",
      "extensionAttribute14": "string",
      "extensionAttribute15": "string"
  }

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onPremisesExtensionAttributes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onpremisesextensionattributes.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
