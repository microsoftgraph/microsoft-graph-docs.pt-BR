---
title: Tipo de recurso onPremisesExtensionAttributes
description: A propriedade **onpremisesextensionattributes à** da entidade de usuário contém quinze Propriedades de atributos de extensões personalizadas. Para um usuário do **onPremisesSyncEnabled** , esse conjunto de propriedades é Mastered no Active Directory local e sincronizado com o Azure AD e é somente leitura. Para um usuário somente na nuvem (onde **onPremisesSyncEnabled** é false), essas propriedades podem ser definidas durante a criação ou atualização.
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 218bf0db4b615072ed3292311a26033279b1d803
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48056433"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="604cc-105">Tipo de recurso onPremisesExtensionAttributes</span><span class="sxs-lookup"><span data-stu-id="604cc-105">onPremisesExtensionAttributes resource type</span></span>

<span data-ttu-id="604cc-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="604cc-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="604cc-107">A propriedade **onpremisesextensionattributes à** da entidade de [usuário](user.md) contém quinze Propriedades de atributos de extensões personalizadas.</span><span class="sxs-lookup"><span data-stu-id="604cc-107">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="604cc-108">Para um usuário do **onPremisesSyncEnabled** , a fonte de autoridade desse conjunto de propriedades é o Active Directory local que é sincronizado com o Azure AD e é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="604cc-108">For an **onPremisesSyncEnabled** user, the source of authority for this set of properties is the on-premises Active Directory which is synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="604cc-109">Para um usuário somente na nuvem (onde **onPremisesSyncEnabled** é false), essas propriedades podem ser definidas durante a criação ou atualização.</span><span class="sxs-lookup"><span data-stu-id="604cc-109">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties may be set during creation or update.</span></span>

> <span data-ttu-id="604cc-110">**Observação:** Esses atributos de extensão também são conhecidos como atributos personalizados do Exchange 1-15.</span><span class="sxs-lookup"><span data-stu-id="604cc-110">**Note:** These extension attributes are also known as Exchange custom attributes 1-15.</span></span>

## <a name="properties"></a><span data-ttu-id="604cc-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="604cc-111">Properties</span></span>
| <span data-ttu-id="604cc-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="604cc-112">Property</span></span>     | <span data-ttu-id="604cc-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="604cc-113">Type</span></span>   |<span data-ttu-id="604cc-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="604cc-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="604cc-115">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="604cc-115">extensionAttribute1</span></span>|<span data-ttu-id="604cc-116">String</span><span class="sxs-lookup"><span data-stu-id="604cc-116">String</span></span>| <span data-ttu-id="604cc-117">Primeiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="604cc-117">First customizable extension attribute.</span></span> |
|<span data-ttu-id="604cc-118">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="604cc-118">extensionAttribute2</span></span>|<span data-ttu-id="604cc-119">String</span><span class="sxs-lookup"><span data-stu-id="604cc-119">String</span></span>| <span data-ttu-id="604cc-120">Segundo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="604cc-120">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="604cc-121">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="604cc-121">extensionAttribute3</span></span>|<span data-ttu-id="604cc-122">String</span><span class="sxs-lookup"><span data-stu-id="604cc-122">String</span></span>| <span data-ttu-id="604cc-123">Terceiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="604cc-123">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="604cc-124">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="604cc-124">extensionAttribute4</span></span>|<span data-ttu-id="604cc-125">String</span><span class="sxs-lookup"><span data-stu-id="604cc-125">String</span></span>| <span data-ttu-id="604cc-126">Quarto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="604cc-126">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="604cc-127">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="604cc-127">extensionAttribute5</span></span>|<span data-ttu-id="604cc-128">String</span><span class="sxs-lookup"><span data-stu-id="604cc-128">String</span></span>| <span data-ttu-id="604cc-129">Quinto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="604cc-129">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="604cc-130">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="604cc-130">extensionAttribute6</span></span>|<span data-ttu-id="604cc-131">String</span><span class="sxs-lookup"><span data-stu-id="604cc-131">String</span></span>| <span data-ttu-id="604cc-132">Sexto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="604cc-132">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="604cc-133">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="604cc-133">extensionAttribute7</span></span>|<span data-ttu-id="604cc-134">String</span><span class="sxs-lookup"><span data-stu-id="604cc-134">String</span></span>| <span data-ttu-id="604cc-135">Sétimo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="604cc-135">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="604cc-136">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="604cc-136">extensionAttribute8</span></span>|<span data-ttu-id="604cc-137">String</span><span class="sxs-lookup"><span data-stu-id="604cc-137">String</span></span>| <span data-ttu-id="604cc-138">Oitavo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="604cc-138">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="604cc-139">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="604cc-139">extensionAttribute9</span></span>|<span data-ttu-id="604cc-140">String</span><span class="sxs-lookup"><span data-stu-id="604cc-140">String</span></span>| <span data-ttu-id="604cc-141">Nono atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="604cc-141">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="604cc-142">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="604cc-142">extensionAttribute10</span></span>|<span data-ttu-id="604cc-143">String</span><span class="sxs-lookup"><span data-stu-id="604cc-143">String</span></span>| <span data-ttu-id="604cc-144">Décimo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="604cc-144">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="604cc-145">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="604cc-145">extensionAttribute11</span></span>|<span data-ttu-id="604cc-146">String</span><span class="sxs-lookup"><span data-stu-id="604cc-146">String</span></span>| <span data-ttu-id="604cc-147">Décimo primeiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="604cc-147">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="604cc-148">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="604cc-148">extensionAttribute12</span></span>|<span data-ttu-id="604cc-149">String</span><span class="sxs-lookup"><span data-stu-id="604cc-149">String</span></span>| <span data-ttu-id="604cc-150">Décimo segundo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="604cc-150">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="604cc-151">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="604cc-151">extensionAttribute13</span></span>|<span data-ttu-id="604cc-152">String</span><span class="sxs-lookup"><span data-stu-id="604cc-152">String</span></span>| <span data-ttu-id="604cc-153">Décimo terceiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="604cc-153">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="604cc-154">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="604cc-154">extensionAttribute14</span></span>|<span data-ttu-id="604cc-155">String</span><span class="sxs-lookup"><span data-stu-id="604cc-155">String</span></span>| <span data-ttu-id="604cc-156">Atributo de extensão personalizável décimo quarto.</span><span class="sxs-lookup"><span data-stu-id="604cc-156">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="604cc-157">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="604cc-157">extensionAttribute15</span></span>|<span data-ttu-id="604cc-158">String</span><span class="sxs-lookup"><span data-stu-id="604cc-158">String</span></span>| <span data-ttu-id="604cc-159">Atributo de extensão personalizável décimo quinto.</span><span class="sxs-lookup"><span data-stu-id="604cc-159">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="604cc-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="604cc-160">JSON representation</span></span>

<span data-ttu-id="604cc-161">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="604cc-161">Here is a JSON representation of the resource</span></span>

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

