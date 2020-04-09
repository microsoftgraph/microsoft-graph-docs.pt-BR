---
title: tipo de recurso Onpremisesextensionattributes à
description: A propriedade **onpremisesextensionattributes à** da entidade de usuário contém quinze Propriedades de atributos de extensões personalizadas. Para um usuário do **onPremisesSyncEnabled** , esse conjunto de propriedades é Mastered no Active Directory local e sincronizado com o Azure AD e é somente leitura. Para um usuário somente na nuvem (onde **onPremisesSyncEnabled** é false), essas propriedades podem ser definidas durante a criação ou atualização.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: japere
ms.openlocfilehash: 06f1fb9fea5338a93c92a2bce2e31098046528bc
ms.sourcegitcommit: ee41ba9ec6001716f1a9d575741bbeef577e2473
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/09/2020
ms.locfileid: "43200226"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="66e1a-105">tipo de recurso Onpremisesextensionattributes à</span><span class="sxs-lookup"><span data-stu-id="66e1a-105">onPremisesExtensionAttributes resource type</span></span>

<span data-ttu-id="66e1a-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66e1a-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66e1a-107">A propriedade **onpremisesextensionattributes à** da entidade de [usuário](user.md) contém quinze Propriedades de atributos de extensões personalizadas.</span><span class="sxs-lookup"><span data-stu-id="66e1a-107">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="66e1a-108">Para um usuário do **onPremisesSyncEnabled** , esse conjunto de propriedades é Mastered no Active Directory local e sincronizado com o Azure AD e é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="66e1a-108">For an **onPremisesSyncEnabled** user, this set of properties is mastered in on-premises Active Directory and synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="66e1a-109">Para um usuário somente na nuvem (onde **onPremisesSyncEnabled** é false), essas propriedades podem ser definidas durante a criação ou atualização.</span><span class="sxs-lookup"><span data-stu-id="66e1a-109">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties may be set during creation or update.</span></span>


## <a name="properties"></a><span data-ttu-id="66e1a-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="66e1a-110">Properties</span></span>
| <span data-ttu-id="66e1a-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="66e1a-111">Property</span></span>     | <span data-ttu-id="66e1a-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="66e1a-112">Type</span></span>   |<span data-ttu-id="66e1a-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="66e1a-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="66e1a-114">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="66e1a-114">extensionAttribute1</span></span>|<span data-ttu-id="66e1a-115">String</span><span class="sxs-lookup"><span data-stu-id="66e1a-115">String</span></span>| <span data-ttu-id="66e1a-116">Primeiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="66e1a-116">First customizable extension attribute.</span></span> |
|<span data-ttu-id="66e1a-117">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="66e1a-117">extensionAttribute2</span></span>|<span data-ttu-id="66e1a-118">String</span><span class="sxs-lookup"><span data-stu-id="66e1a-118">String</span></span>| <span data-ttu-id="66e1a-119">Segundo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="66e1a-119">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="66e1a-120">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="66e1a-120">extensionAttribute3</span></span>|<span data-ttu-id="66e1a-121">String</span><span class="sxs-lookup"><span data-stu-id="66e1a-121">String</span></span>| <span data-ttu-id="66e1a-122">Terceiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="66e1a-122">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="66e1a-123">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="66e1a-123">extensionAttribute4</span></span>|<span data-ttu-id="66e1a-124">String</span><span class="sxs-lookup"><span data-stu-id="66e1a-124">String</span></span>| <span data-ttu-id="66e1a-125">Quarto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="66e1a-125">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="66e1a-126">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="66e1a-126">extensionAttribute5</span></span>|<span data-ttu-id="66e1a-127">String</span><span class="sxs-lookup"><span data-stu-id="66e1a-127">String</span></span>| <span data-ttu-id="66e1a-128">Quinto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="66e1a-128">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="66e1a-129">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="66e1a-129">extensionAttribute6</span></span>|<span data-ttu-id="66e1a-130">String</span><span class="sxs-lookup"><span data-stu-id="66e1a-130">String</span></span>| <span data-ttu-id="66e1a-131">Sexto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="66e1a-131">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="66e1a-132">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="66e1a-132">extensionAttribute7</span></span>|<span data-ttu-id="66e1a-133">String</span><span class="sxs-lookup"><span data-stu-id="66e1a-133">String</span></span>| <span data-ttu-id="66e1a-134">Sétimo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="66e1a-134">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="66e1a-135">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="66e1a-135">extensionAttribute8</span></span>|<span data-ttu-id="66e1a-136">String</span><span class="sxs-lookup"><span data-stu-id="66e1a-136">String</span></span>| <span data-ttu-id="66e1a-137">Oitavo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="66e1a-137">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="66e1a-138">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="66e1a-138">extensionAttribute9</span></span>|<span data-ttu-id="66e1a-139">String</span><span class="sxs-lookup"><span data-stu-id="66e1a-139">String</span></span>| <span data-ttu-id="66e1a-140">Nono atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="66e1a-140">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="66e1a-141">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="66e1a-141">extensionAttribute10</span></span>|<span data-ttu-id="66e1a-142">String</span><span class="sxs-lookup"><span data-stu-id="66e1a-142">String</span></span>| <span data-ttu-id="66e1a-143">Décimo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="66e1a-143">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="66e1a-144">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="66e1a-144">extensionAttribute11</span></span>|<span data-ttu-id="66e1a-145">String</span><span class="sxs-lookup"><span data-stu-id="66e1a-145">String</span></span>| <span data-ttu-id="66e1a-146">Décimo primeiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="66e1a-146">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="66e1a-147">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="66e1a-147">extensionAttribute12</span></span>|<span data-ttu-id="66e1a-148">String</span><span class="sxs-lookup"><span data-stu-id="66e1a-148">String</span></span>| <span data-ttu-id="66e1a-149">Décimo segundo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="66e1a-149">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="66e1a-150">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="66e1a-150">extensionAttribute13</span></span>|<span data-ttu-id="66e1a-151">String</span><span class="sxs-lookup"><span data-stu-id="66e1a-151">String</span></span>| <span data-ttu-id="66e1a-152">Décimo terceiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="66e1a-152">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="66e1a-153">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="66e1a-153">extensionAttribute14</span></span>|<span data-ttu-id="66e1a-154">String</span><span class="sxs-lookup"><span data-stu-id="66e1a-154">String</span></span>| <span data-ttu-id="66e1a-155">Atributo de extensão personalizável décimo quarto.</span><span class="sxs-lookup"><span data-stu-id="66e1a-155">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="66e1a-156">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="66e1a-156">extensionAttribute15</span></span>|<span data-ttu-id="66e1a-157">String</span><span class="sxs-lookup"><span data-stu-id="66e1a-157">String</span></span>| <span data-ttu-id="66e1a-158">Atributo de extensão personalizável décimo quinto.</span><span class="sxs-lookup"><span data-stu-id="66e1a-158">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="66e1a-159">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="66e1a-159">JSON representation</span></span>

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
