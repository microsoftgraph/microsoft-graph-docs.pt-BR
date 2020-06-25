---
title: tipo de recurso Onpremisesextensionattributes à
description: A propriedade **onpremisesextensionattributes à** da entidade de usuário contém quinze Propriedades de atributos de extensões personalizadas. Para um usuário do **onPremisesSyncEnabled** , esse conjunto de propriedades é Mastered no Active Directory local e sincronizado com o Azure AD e é somente leitura. Para um usuário somente na nuvem (onde **onPremisesSyncEnabled** é false), essas propriedades podem ser definidas durante a criação ou atualização.
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 84929229c18b905ff66b4a1bbbbf765771180a06
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2020
ms.locfileid: "44864088"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="5aaa5-105">tipo de recurso Onpremisesextensionattributes à</span><span class="sxs-lookup"><span data-stu-id="5aaa5-105">onPremisesExtensionAttributes resource type</span></span>

<span data-ttu-id="5aaa5-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5aaa5-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5aaa5-107">A propriedade **onpremisesextensionattributes à** da entidade de [usuário](user.md) contém quinze Propriedades de atributos de extensões personalizadas.</span><span class="sxs-lookup"><span data-stu-id="5aaa5-107">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="5aaa5-108">Para um usuário do **onPremisesSyncEnabled** , a fonte de autoridade desse conjunto de propriedades é o Active Directory local que é sincronizado com o Azure AD e é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5aaa5-108">For an **onPremisesSyncEnabled** user, the source of authority for this set of properties is the on-premises Active Directory which is synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="5aaa5-109">Para um usuário somente na nuvem (onde **onPremisesSyncEnabled** é false), essas propriedades podem ser definidas durante a criação ou atualização.</span><span class="sxs-lookup"><span data-stu-id="5aaa5-109">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties may be set during creation or update.</span></span>

> <span data-ttu-id="5aaa5-110">**Observação:** Esses atributos de extensão também são conhecidos como atributos personalizados do Exchange 1-15.</span><span class="sxs-lookup"><span data-stu-id="5aaa5-110">**Note:** These extension attributes are also known as Exchange custom attributes 1-15.</span></span>

## <a name="properties"></a><span data-ttu-id="5aaa5-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5aaa5-111">Properties</span></span>
| <span data-ttu-id="5aaa5-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5aaa5-112">Property</span></span>     | <span data-ttu-id="5aaa5-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="5aaa5-113">Type</span></span>   |<span data-ttu-id="5aaa5-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="5aaa5-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5aaa5-115">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="5aaa5-115">extensionAttribute1</span></span>|<span data-ttu-id="5aaa5-116">String</span><span class="sxs-lookup"><span data-stu-id="5aaa5-116">String</span></span>| <span data-ttu-id="5aaa5-117">Primeiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="5aaa5-117">First customizable extension attribute.</span></span> |
|<span data-ttu-id="5aaa5-118">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="5aaa5-118">extensionAttribute2</span></span>|<span data-ttu-id="5aaa5-119">String</span><span class="sxs-lookup"><span data-stu-id="5aaa5-119">String</span></span>| <span data-ttu-id="5aaa5-120">Segundo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="5aaa5-120">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="5aaa5-121">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="5aaa5-121">extensionAttribute3</span></span>|<span data-ttu-id="5aaa5-122">String</span><span class="sxs-lookup"><span data-stu-id="5aaa5-122">String</span></span>| <span data-ttu-id="5aaa5-123">Terceiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="5aaa5-123">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="5aaa5-124">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="5aaa5-124">extensionAttribute4</span></span>|<span data-ttu-id="5aaa5-125">String</span><span class="sxs-lookup"><span data-stu-id="5aaa5-125">String</span></span>| <span data-ttu-id="5aaa5-126">Quarto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="5aaa5-126">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="5aaa5-127">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="5aaa5-127">extensionAttribute5</span></span>|<span data-ttu-id="5aaa5-128">String</span><span class="sxs-lookup"><span data-stu-id="5aaa5-128">String</span></span>| <span data-ttu-id="5aaa5-129">Quinto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="5aaa5-129">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="5aaa5-130">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="5aaa5-130">extensionAttribute6</span></span>|<span data-ttu-id="5aaa5-131">String</span><span class="sxs-lookup"><span data-stu-id="5aaa5-131">String</span></span>| <span data-ttu-id="5aaa5-132">Sexto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="5aaa5-132">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="5aaa5-133">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="5aaa5-133">extensionAttribute7</span></span>|<span data-ttu-id="5aaa5-134">String</span><span class="sxs-lookup"><span data-stu-id="5aaa5-134">String</span></span>| <span data-ttu-id="5aaa5-135">Sétimo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="5aaa5-135">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="5aaa5-136">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="5aaa5-136">extensionAttribute8</span></span>|<span data-ttu-id="5aaa5-137">String</span><span class="sxs-lookup"><span data-stu-id="5aaa5-137">String</span></span>| <span data-ttu-id="5aaa5-138">Oitavo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="5aaa5-138">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="5aaa5-139">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="5aaa5-139">extensionAttribute9</span></span>|<span data-ttu-id="5aaa5-140">String</span><span class="sxs-lookup"><span data-stu-id="5aaa5-140">String</span></span>| <span data-ttu-id="5aaa5-141">Nono atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="5aaa5-141">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="5aaa5-142">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="5aaa5-142">extensionAttribute10</span></span>|<span data-ttu-id="5aaa5-143">String</span><span class="sxs-lookup"><span data-stu-id="5aaa5-143">String</span></span>| <span data-ttu-id="5aaa5-144">Décimo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="5aaa5-144">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="5aaa5-145">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="5aaa5-145">extensionAttribute11</span></span>|<span data-ttu-id="5aaa5-146">String</span><span class="sxs-lookup"><span data-stu-id="5aaa5-146">String</span></span>| <span data-ttu-id="5aaa5-147">Décimo primeiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="5aaa5-147">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="5aaa5-148">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="5aaa5-148">extensionAttribute12</span></span>|<span data-ttu-id="5aaa5-149">String</span><span class="sxs-lookup"><span data-stu-id="5aaa5-149">String</span></span>| <span data-ttu-id="5aaa5-150">Décimo segundo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="5aaa5-150">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="5aaa5-151">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="5aaa5-151">extensionAttribute13</span></span>|<span data-ttu-id="5aaa5-152">String</span><span class="sxs-lookup"><span data-stu-id="5aaa5-152">String</span></span>| <span data-ttu-id="5aaa5-153">Décimo terceiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="5aaa5-153">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="5aaa5-154">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="5aaa5-154">extensionAttribute14</span></span>|<span data-ttu-id="5aaa5-155">String</span><span class="sxs-lookup"><span data-stu-id="5aaa5-155">String</span></span>| <span data-ttu-id="5aaa5-156">Atributo de extensão personalizável décimo quarto.</span><span class="sxs-lookup"><span data-stu-id="5aaa5-156">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="5aaa5-157">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="5aaa5-157">extensionAttribute15</span></span>|<span data-ttu-id="5aaa5-158">String</span><span class="sxs-lookup"><span data-stu-id="5aaa5-158">String</span></span>| <span data-ttu-id="5aaa5-159">Atributo de extensão personalizável décimo quinto.</span><span class="sxs-lookup"><span data-stu-id="5aaa5-159">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5aaa5-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5aaa5-160">JSON representation</span></span>

<span data-ttu-id="5aaa5-161">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="5aaa5-161">Here is a JSON representation of the resource</span></span>

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
