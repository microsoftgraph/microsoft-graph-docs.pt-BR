---
title: tipo de recurso de onPremisesExtensionAttributes
description: A propriedade **onPremisesExtensionAttributes** da entidade do usuário contém quinze propriedades de atributo de extensão personalizada. Um usuário **onPremisesSyncEnabled** , esse conjunto de propriedades é administrado no Active Directory no local e sincronizado com o Azure AD e é somente leitura. Para um usuário somente na nuvem (onde **onPremisesSyncEnabled** é false), essas propriedades podem ser definida durante a criação ou atualização.
localization_priority: Normal
ms.openlocfilehash: c0cb765efe9e94c8254e45eaa9d55bc16382f6d2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824742"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="a9171-105">tipo de recurso de onPremisesExtensionAttributes</span><span class="sxs-lookup"><span data-stu-id="a9171-105">onPremisesExtensionAttributes resource type</span></span>

<span data-ttu-id="a9171-106">A propriedade **onPremisesExtensionAttributes** da entidade do [usuário](user.md) contém quinze propriedades de atributo de extensão personalizada.</span><span class="sxs-lookup"><span data-stu-id="a9171-106">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="a9171-107">Um usuário **onPremisesSyncEnabled** , esse conjunto de propriedades é administrado no Active Directory no local e sincronizado com o Azure AD e é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a9171-107">For an **onPremisesSyncEnabled** user, this set of properties is mastered in on-premises Active Directory and synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="a9171-108">Para um usuário somente na nuvem (onde **onPremisesSyncEnabled** é false), essas propriedades podem ser definida durante a criação ou atualização.</span><span class="sxs-lookup"><span data-stu-id="a9171-108">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties may be set during creation or update.</span></span>


## <a name="properties"></a><span data-ttu-id="a9171-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a9171-109">Properties</span></span>
| <span data-ttu-id="a9171-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a9171-110">Property</span></span>     | <span data-ttu-id="a9171-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="a9171-111">Type</span></span>   |<span data-ttu-id="a9171-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9171-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a9171-113">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="a9171-113">extensionAttribute1</span></span>|<span data-ttu-id="a9171-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a9171-114">String</span></span>| <span data-ttu-id="a9171-115">Primeiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="a9171-115">First customizable extension attribute.</span></span> |
|<span data-ttu-id="a9171-116">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="a9171-116">extensionAttribute2</span></span>|<span data-ttu-id="a9171-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a9171-117">String</span></span>| <span data-ttu-id="a9171-118">Segundo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="a9171-118">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="a9171-119">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="a9171-119">extensionAttribute3</span></span>|<span data-ttu-id="a9171-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a9171-120">String</span></span>| <span data-ttu-id="a9171-121">Atributo do terceiro extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="a9171-121">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="a9171-122">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="a9171-122">extensionAttribute4</span></span>|<span data-ttu-id="a9171-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a9171-123">String</span></span>| <span data-ttu-id="a9171-124">Quarto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="a9171-124">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="a9171-125">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="a9171-125">extensionAttribute5</span></span>|<span data-ttu-id="a9171-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a9171-126">String</span></span>| <span data-ttu-id="a9171-127">Atributo do quinto extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="a9171-127">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="a9171-128">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="a9171-128">extensionAttribute6</span></span>|<span data-ttu-id="a9171-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a9171-129">String</span></span>| <span data-ttu-id="a9171-130">Sexto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="a9171-130">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="a9171-131">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="a9171-131">extensionAttribute7</span></span>|<span data-ttu-id="a9171-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a9171-132">String</span></span>| <span data-ttu-id="a9171-133">Sétimo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="a9171-133">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="a9171-134">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="a9171-134">extensionAttribute8</span></span>|<span data-ttu-id="a9171-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a9171-135">String</span></span>| <span data-ttu-id="a9171-136">Oitavo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="a9171-136">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="a9171-137">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="a9171-137">extensionAttribute9</span></span>|<span data-ttu-id="a9171-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a9171-138">String</span></span>| <span data-ttu-id="a9171-139">Nono atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="a9171-139">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="a9171-140">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="a9171-140">extensionAttribute10</span></span>|<span data-ttu-id="a9171-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a9171-141">String</span></span>| <span data-ttu-id="a9171-142">Décimo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="a9171-142">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="a9171-143">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="a9171-143">extensionAttribute11</span></span>|<span data-ttu-id="a9171-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a9171-144">String</span></span>| <span data-ttu-id="a9171-145">Atributo de extensão Décima primeira personalizável.</span><span class="sxs-lookup"><span data-stu-id="a9171-145">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="a9171-146">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="a9171-146">extensionAttribute12</span></span>|<span data-ttu-id="a9171-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a9171-147">String</span></span>| <span data-ttu-id="a9171-148">Atributo de extensão Décima segunda personalizável.</span><span class="sxs-lookup"><span data-stu-id="a9171-148">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="a9171-149">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="a9171-149">extensionAttribute13</span></span>|<span data-ttu-id="a9171-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a9171-150">String</span></span>| <span data-ttu-id="a9171-151">Atributo de extensão Décima terceira personalizável.</span><span class="sxs-lookup"><span data-stu-id="a9171-151">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="a9171-152">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="a9171-152">extensionAttribute14</span></span>|<span data-ttu-id="a9171-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a9171-153">String</span></span>| <span data-ttu-id="a9171-154">Atributo de extensão décima quarta personalizável.</span><span class="sxs-lookup"><span data-stu-id="a9171-154">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="a9171-155">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="a9171-155">extensionAttribute15</span></span>|<span data-ttu-id="a9171-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a9171-156">String</span></span>| <span data-ttu-id="a9171-157">Atributo de extensão Décima quinta personalizável.</span><span class="sxs-lookup"><span data-stu-id="a9171-157">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a9171-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a9171-158">JSON representation</span></span>

<span data-ttu-id="a9171-159">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="a9171-159">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesExtensionAttributes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
