---
title: Tipo de recurso onPremisesExtensionAttributes
description: A **propriedade onPremisesExtensionAttributes** da entidade do usuário contém quinze propriedades de atributo de extensão personalizadas.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: users
author: jpettere
ms.openlocfilehash: 95d777140210070471c9578399e26e0eda3620d7
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720582"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="c814d-103">Tipo de recurso onPremisesExtensionAttributes</span><span class="sxs-lookup"><span data-stu-id="c814d-103">onPremisesExtensionAttributes resource type</span></span>

<span data-ttu-id="c814d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c814d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c814d-105">A **propriedade onPremisesExtensionAttributes** da entidade do usuário contém quinze propriedades de atributo de extensão personalizadas. [](user.md)</span><span class="sxs-lookup"><span data-stu-id="c814d-105">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="c814d-106">Para um usuário **onPremisesSyncEnabled,** a fonte de autoridade para esse conjunto de propriedades é o Active Directory local que é sincronizado com o Azure AD e é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c814d-106">For an **onPremisesSyncEnabled** user, the source of authority for this set of properties is the on-premises Active Directory which is synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="c814d-107">Para um usuário somente na nuvem (onde **onPremisesSyncEnabled** é false), essas propriedades podem ser definidas durante a criação ou atualização.</span><span class="sxs-lookup"><span data-stu-id="c814d-107">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties may be set during creation or update.</span></span>

> <span data-ttu-id="c814d-108">**Observação:** Esses atributos de extensão também são conhecidos como atributos personalizados do Exchange 1-15.</span><span class="sxs-lookup"><span data-stu-id="c814d-108">**Note:** These extension attributes are also known as Exchange custom attributes 1-15.</span></span>


## <a name="properties"></a><span data-ttu-id="c814d-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c814d-109">Properties</span></span>
| <span data-ttu-id="c814d-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c814d-110">Property</span></span>     | <span data-ttu-id="c814d-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="c814d-111">Type</span></span>   |<span data-ttu-id="c814d-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="c814d-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c814d-113">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="c814d-113">extensionAttribute1</span></span>|<span data-ttu-id="c814d-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c814d-114">String</span></span>| <span data-ttu-id="c814d-115">Primeiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="c814d-115">First customizable extension attribute.</span></span> |
|<span data-ttu-id="c814d-116">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="c814d-116">extensionAttribute2</span></span>|<span data-ttu-id="c814d-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c814d-117">String</span></span>| <span data-ttu-id="c814d-118">Segundo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="c814d-118">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="c814d-119">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="c814d-119">extensionAttribute3</span></span>|<span data-ttu-id="c814d-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c814d-120">String</span></span>| <span data-ttu-id="c814d-121">Terceiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="c814d-121">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="c814d-122">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="c814d-122">extensionAttribute4</span></span>|<span data-ttu-id="c814d-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c814d-123">String</span></span>| <span data-ttu-id="c814d-124">Quarto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="c814d-124">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="c814d-125">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="c814d-125">extensionAttribute5</span></span>|<span data-ttu-id="c814d-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c814d-126">String</span></span>| <span data-ttu-id="c814d-127">Quinto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="c814d-127">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="c814d-128">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="c814d-128">extensionAttribute6</span></span>|<span data-ttu-id="c814d-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c814d-129">String</span></span>| <span data-ttu-id="c814d-130">Sexto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="c814d-130">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="c814d-131">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="c814d-131">extensionAttribute7</span></span>|<span data-ttu-id="c814d-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c814d-132">String</span></span>| <span data-ttu-id="c814d-133">Sétimo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="c814d-133">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="c814d-134">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="c814d-134">extensionAttribute8</span></span>|<span data-ttu-id="c814d-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c814d-135">String</span></span>| <span data-ttu-id="c814d-136">Oitavo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="c814d-136">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="c814d-137">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="c814d-137">extensionAttribute9</span></span>|<span data-ttu-id="c814d-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c814d-138">String</span></span>| <span data-ttu-id="c814d-139">Nono atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="c814d-139">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="c814d-140">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="c814d-140">extensionAttribute10</span></span>|<span data-ttu-id="c814d-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c814d-141">String</span></span>| <span data-ttu-id="c814d-142">Décimo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="c814d-142">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="c814d-143">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="c814d-143">extensionAttribute11</span></span>|<span data-ttu-id="c814d-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c814d-144">String</span></span>| <span data-ttu-id="c814d-145">Décimo primeiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="c814d-145">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="c814d-146">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="c814d-146">extensionAttribute12</span></span>|<span data-ttu-id="c814d-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c814d-147">String</span></span>| <span data-ttu-id="c814d-148">Décimo segundo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="c814d-148">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="c814d-149">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="c814d-149">extensionAttribute13</span></span>|<span data-ttu-id="c814d-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c814d-150">String</span></span>| <span data-ttu-id="c814d-151">Décimo terceiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="c814d-151">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="c814d-152">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="c814d-152">extensionAttribute14</span></span>|<span data-ttu-id="c814d-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c814d-153">String</span></span>| <span data-ttu-id="c814d-154">Décimo quarto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="c814d-154">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="c814d-155">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="c814d-155">extensionAttribute15</span></span>|<span data-ttu-id="c814d-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c814d-156">String</span></span>| <span data-ttu-id="c814d-157">Décimo quinto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="c814d-157">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c814d-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c814d-158">JSON representation</span></span>

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
  "suppressions": []
}
-->


