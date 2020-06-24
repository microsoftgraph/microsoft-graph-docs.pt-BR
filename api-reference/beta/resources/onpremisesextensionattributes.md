---
title: tipo de recurso Onpremisesextensionattributes à
description: A propriedade **onpremisesextensionattributes à** da entidade de usuário contém quinze Propriedades de atributos de extensões personalizadas.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: users
author: krbain
ms.openlocfilehash: 1035674a6ce5d9f2c0a1a8b2cd35896c92ec7147
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863751"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="22722-103">tipo de recurso Onpremisesextensionattributes à</span><span class="sxs-lookup"><span data-stu-id="22722-103">onPremisesExtensionAttributes resource type</span></span>

<span data-ttu-id="22722-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22722-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22722-105">A propriedade **onpremisesextensionattributes à** da entidade de [usuário](user.md) contém quinze Propriedades de atributos de extensões personalizadas.</span><span class="sxs-lookup"><span data-stu-id="22722-105">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="22722-106">Para um usuário do **onPremisesSyncEnabled** , a fonte de autoridade desse conjunto de propriedades é o Active Directory local que é sincronizado com o Azure AD e é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="22722-106">For an **onPremisesSyncEnabled** user, the source of authority for this set of properties is the on-premises Active Directory which is synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="22722-107">Para um usuário somente na nuvem (onde **onPremisesSyncEnabled** é false), essas propriedades podem ser definidas durante a criação ou atualização.</span><span class="sxs-lookup"><span data-stu-id="22722-107">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties may be set during creation or update.</span></span>

> <span data-ttu-id="22722-108">**Observação:** Esses atributos de extensão também são conhecidos como atributos personalizados do Exchange 1-15.</span><span class="sxs-lookup"><span data-stu-id="22722-108">**Note:** These extension attributes are also known as Exchange custom attributes 1-15.</span></span>


## <a name="properties"></a><span data-ttu-id="22722-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="22722-109">Properties</span></span>
| <span data-ttu-id="22722-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="22722-110">Property</span></span>     | <span data-ttu-id="22722-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="22722-111">Type</span></span>   |<span data-ttu-id="22722-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="22722-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="22722-113">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="22722-113">extensionAttribute1</span></span>|<span data-ttu-id="22722-114">String</span><span class="sxs-lookup"><span data-stu-id="22722-114">String</span></span>| <span data-ttu-id="22722-115">Primeiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="22722-115">First customizable extension attribute.</span></span> |
|<span data-ttu-id="22722-116">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="22722-116">extensionAttribute2</span></span>|<span data-ttu-id="22722-117">String</span><span class="sxs-lookup"><span data-stu-id="22722-117">String</span></span>| <span data-ttu-id="22722-118">Segundo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="22722-118">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="22722-119">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="22722-119">extensionAttribute3</span></span>|<span data-ttu-id="22722-120">String</span><span class="sxs-lookup"><span data-stu-id="22722-120">String</span></span>| <span data-ttu-id="22722-121">Terceiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="22722-121">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="22722-122">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="22722-122">extensionAttribute4</span></span>|<span data-ttu-id="22722-123">String</span><span class="sxs-lookup"><span data-stu-id="22722-123">String</span></span>| <span data-ttu-id="22722-124">Quarto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="22722-124">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="22722-125">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="22722-125">extensionAttribute5</span></span>|<span data-ttu-id="22722-126">String</span><span class="sxs-lookup"><span data-stu-id="22722-126">String</span></span>| <span data-ttu-id="22722-127">Quinto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="22722-127">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="22722-128">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="22722-128">extensionAttribute6</span></span>|<span data-ttu-id="22722-129">String</span><span class="sxs-lookup"><span data-stu-id="22722-129">String</span></span>| <span data-ttu-id="22722-130">Sexto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="22722-130">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="22722-131">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="22722-131">extensionAttribute7</span></span>|<span data-ttu-id="22722-132">String</span><span class="sxs-lookup"><span data-stu-id="22722-132">String</span></span>| <span data-ttu-id="22722-133">Sétimo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="22722-133">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="22722-134">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="22722-134">extensionAttribute8</span></span>|<span data-ttu-id="22722-135">String</span><span class="sxs-lookup"><span data-stu-id="22722-135">String</span></span>| <span data-ttu-id="22722-136">Oitavo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="22722-136">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="22722-137">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="22722-137">extensionAttribute9</span></span>|<span data-ttu-id="22722-138">String</span><span class="sxs-lookup"><span data-stu-id="22722-138">String</span></span>| <span data-ttu-id="22722-139">Nono atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="22722-139">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="22722-140">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="22722-140">extensionAttribute10</span></span>|<span data-ttu-id="22722-141">String</span><span class="sxs-lookup"><span data-stu-id="22722-141">String</span></span>| <span data-ttu-id="22722-142">Décimo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="22722-142">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="22722-143">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="22722-143">extensionAttribute11</span></span>|<span data-ttu-id="22722-144">String</span><span class="sxs-lookup"><span data-stu-id="22722-144">String</span></span>| <span data-ttu-id="22722-145">Décimo primeiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="22722-145">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="22722-146">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="22722-146">extensionAttribute12</span></span>|<span data-ttu-id="22722-147">String</span><span class="sxs-lookup"><span data-stu-id="22722-147">String</span></span>| <span data-ttu-id="22722-148">Décimo segundo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="22722-148">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="22722-149">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="22722-149">extensionAttribute13</span></span>|<span data-ttu-id="22722-150">String</span><span class="sxs-lookup"><span data-stu-id="22722-150">String</span></span>| <span data-ttu-id="22722-151">Décimo terceiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="22722-151">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="22722-152">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="22722-152">extensionAttribute14</span></span>|<span data-ttu-id="22722-153">String</span><span class="sxs-lookup"><span data-stu-id="22722-153">String</span></span>| <span data-ttu-id="22722-154">Atributo de extensão personalizável décimo quarto.</span><span class="sxs-lookup"><span data-stu-id="22722-154">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="22722-155">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="22722-155">extensionAttribute15</span></span>|<span data-ttu-id="22722-156">String</span><span class="sxs-lookup"><span data-stu-id="22722-156">String</span></span>| <span data-ttu-id="22722-157">Atributo de extensão personalizável décimo quinto.</span><span class="sxs-lookup"><span data-stu-id="22722-157">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="22722-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="22722-158">JSON representation</span></span>

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
