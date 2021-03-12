---
title: Tipo de recurso onPremisesExtensionAttributes
description: A **propriedade onPremisesExtensionAttributes** da entidade do usuário contém quinze propriedades de atributo de extensão personalizadas. Para um usuário **onPremisesSyncEnabled,** esse conjunto de propriedades é mestre no Active Directory local e sincronizado com o Azure AD, e é somente leitura. Para um usuário somente na nuvem (onde **onPremisesSyncEnabled** é false), essas propriedades podem ser definidas durante a criação ou atualização.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: c8e44879b3248cab502ee2aeabdaa732a2b35e1f
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50718954"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="5756a-105">Tipo de recurso onPremisesExtensionAttributes</span><span class="sxs-lookup"><span data-stu-id="5756a-105">onPremisesExtensionAttributes resource type</span></span>

<span data-ttu-id="5756a-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5756a-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5756a-107">A **propriedade onPremisesExtensionAttributes** da entidade do usuário contém quinze propriedades de atributo de extensão personalizadas. [](user.md)</span><span class="sxs-lookup"><span data-stu-id="5756a-107">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="5756a-108">Para um usuário **onPremisesSyncEnabled,** a fonte de autoridade para esse conjunto de propriedades é o Active Directory local que é sincronizado com o Azure AD e é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5756a-108">For an **onPremisesSyncEnabled** user, the source of authority for this set of properties is the on-premises Active Directory which is synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="5756a-109">Para um usuário somente na nuvem (onde **onPremisesSyncEnabled** é false), essas propriedades podem ser definidas durante a criação ou atualização.</span><span class="sxs-lookup"><span data-stu-id="5756a-109">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties may be set during creation or update.</span></span>

> <span data-ttu-id="5756a-110">**Observação:** Esses atributos de extensão também são conhecidos como atributos personalizados do Exchange 1-15.</span><span class="sxs-lookup"><span data-stu-id="5756a-110">**Note:** These extension attributes are also known as Exchange custom attributes 1-15.</span></span>

## <a name="properties"></a><span data-ttu-id="5756a-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5756a-111">Properties</span></span>
| <span data-ttu-id="5756a-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5756a-112">Property</span></span>     | <span data-ttu-id="5756a-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="5756a-113">Type</span></span>   |<span data-ttu-id="5756a-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="5756a-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5756a-115">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="5756a-115">extensionAttribute1</span></span>|<span data-ttu-id="5756a-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5756a-116">String</span></span>| <span data-ttu-id="5756a-117">Primeiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="5756a-117">First customizable extension attribute.</span></span> |
|<span data-ttu-id="5756a-118">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="5756a-118">extensionAttribute2</span></span>|<span data-ttu-id="5756a-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5756a-119">String</span></span>| <span data-ttu-id="5756a-120">Segundo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="5756a-120">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="5756a-121">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="5756a-121">extensionAttribute3</span></span>|<span data-ttu-id="5756a-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5756a-122">String</span></span>| <span data-ttu-id="5756a-123">Terceiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="5756a-123">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="5756a-124">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="5756a-124">extensionAttribute4</span></span>|<span data-ttu-id="5756a-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5756a-125">String</span></span>| <span data-ttu-id="5756a-126">Quarto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="5756a-126">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="5756a-127">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="5756a-127">extensionAttribute5</span></span>|<span data-ttu-id="5756a-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5756a-128">String</span></span>| <span data-ttu-id="5756a-129">Quinto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="5756a-129">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="5756a-130">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="5756a-130">extensionAttribute6</span></span>|<span data-ttu-id="5756a-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5756a-131">String</span></span>| <span data-ttu-id="5756a-132">Sexto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="5756a-132">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="5756a-133">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="5756a-133">extensionAttribute7</span></span>|<span data-ttu-id="5756a-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5756a-134">String</span></span>| <span data-ttu-id="5756a-135">Sétimo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="5756a-135">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="5756a-136">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="5756a-136">extensionAttribute8</span></span>|<span data-ttu-id="5756a-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5756a-137">String</span></span>| <span data-ttu-id="5756a-138">Oitavo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="5756a-138">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="5756a-139">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="5756a-139">extensionAttribute9</span></span>|<span data-ttu-id="5756a-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5756a-140">String</span></span>| <span data-ttu-id="5756a-141">Nono atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="5756a-141">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="5756a-142">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="5756a-142">extensionAttribute10</span></span>|<span data-ttu-id="5756a-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5756a-143">String</span></span>| <span data-ttu-id="5756a-144">Décimo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="5756a-144">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="5756a-145">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="5756a-145">extensionAttribute11</span></span>|<span data-ttu-id="5756a-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5756a-146">String</span></span>| <span data-ttu-id="5756a-147">Décimo primeiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="5756a-147">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="5756a-148">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="5756a-148">extensionAttribute12</span></span>|<span data-ttu-id="5756a-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5756a-149">String</span></span>| <span data-ttu-id="5756a-150">Décimo segundo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="5756a-150">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="5756a-151">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="5756a-151">extensionAttribute13</span></span>|<span data-ttu-id="5756a-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5756a-152">String</span></span>| <span data-ttu-id="5756a-153">Décimo terceiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="5756a-153">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="5756a-154">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="5756a-154">extensionAttribute14</span></span>|<span data-ttu-id="5756a-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5756a-155">String</span></span>| <span data-ttu-id="5756a-156">Décimo quarto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="5756a-156">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="5756a-157">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="5756a-157">extensionAttribute15</span></span>|<span data-ttu-id="5756a-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5756a-158">String</span></span>| <span data-ttu-id="5756a-159">Décimo quinto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="5756a-159">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5756a-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5756a-160">JSON representation</span></span>

<span data-ttu-id="5756a-161">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="5756a-161">Here is a JSON representation of the resource</span></span>

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

