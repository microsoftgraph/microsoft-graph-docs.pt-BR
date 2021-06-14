---
title: Tipo de recurso onPremisesExtensionAttributes
description: A **propriedade onPremisesExtensionAttributes** da entidade do usuário contém quinze propriedades de atributo de extensão personalizadas. Para um usuário **onPremisesSyncEnabled,** esse conjunto de propriedades é mestre no Active Directory local e sincronizado com o Azure AD, e é somente leitura. Para um usuário somente na nuvem (onde **onPremisesSyncEnabled** é false), essas propriedades podem ser definidas sobre Exchange Online. Os atributos são lidos somente no Microsoft Graph.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 3081b377a30bbf09131650517dcee61597dea597
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912044"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="85594-106">Tipo de recurso onPremisesExtensionAttributes</span><span class="sxs-lookup"><span data-stu-id="85594-106">onPremisesExtensionAttributes resource type</span></span>

<span data-ttu-id="85594-107">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85594-107">Namespace: microsoft.graph</span></span>

<span data-ttu-id="85594-108">A **propriedade onPremisesExtensionAttributes** da entidade do usuário contém quinze propriedades de atributo de extensão personalizadas. [](user.md)</span><span class="sxs-lookup"><span data-stu-id="85594-108">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="85594-109">Para um usuário **onPremisesSyncEnabled,** a fonte de autoridade para esse conjunto de propriedades é o Active Directory local que é sincronizado com o Azure AD e é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="85594-109">For an **onPremisesSyncEnabled** user, the source of authority for this set of properties is the on-premises Active Directory which is synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="85594-110">Para um usuário somente na nuvem (onde **onPremisesSyncEnabled** está ), essas propriedades podem ser definidas durante a `false` [criação](../api/user-post-users.md) ou [atualização.](../api/user-update.md)</span><span class="sxs-lookup"><span data-stu-id="85594-110">For a cloud-only user (where **onPremisesSyncEnabled** is `false`), these properties may be set during [creation](../api/user-post-users.md) or [update](../api/user-update.md).</span></span>

> <span data-ttu-id="85594-111">**Observação:** Esses atributos de extensão também são conhecidos como Exchange atributos personalizados 1-15.</span><span class="sxs-lookup"><span data-stu-id="85594-111">**Note:** These extension attributes are also known as Exchange custom attributes 1-15.</span></span>

## <a name="properties"></a><span data-ttu-id="85594-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="85594-112">Properties</span></span>
| <span data-ttu-id="85594-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="85594-113">Property</span></span>     | <span data-ttu-id="85594-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="85594-114">Type</span></span>   |<span data-ttu-id="85594-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="85594-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="85594-116">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="85594-116">extensionAttribute1</span></span>|<span data-ttu-id="85594-117">String</span><span class="sxs-lookup"><span data-stu-id="85594-117">String</span></span>| <span data-ttu-id="85594-118">Primeiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="85594-118">First customizable extension attribute.</span></span> |
|<span data-ttu-id="85594-119">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="85594-119">extensionAttribute2</span></span>|<span data-ttu-id="85594-120">String</span><span class="sxs-lookup"><span data-stu-id="85594-120">String</span></span>| <span data-ttu-id="85594-121">Segundo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="85594-121">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="85594-122">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="85594-122">extensionAttribute3</span></span>|<span data-ttu-id="85594-123">String</span><span class="sxs-lookup"><span data-stu-id="85594-123">String</span></span>| <span data-ttu-id="85594-124">Terceiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="85594-124">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="85594-125">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="85594-125">extensionAttribute4</span></span>|<span data-ttu-id="85594-126">String</span><span class="sxs-lookup"><span data-stu-id="85594-126">String</span></span>| <span data-ttu-id="85594-127">Quarto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="85594-127">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="85594-128">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="85594-128">extensionAttribute5</span></span>|<span data-ttu-id="85594-129">String</span><span class="sxs-lookup"><span data-stu-id="85594-129">String</span></span>| <span data-ttu-id="85594-130">Quinto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="85594-130">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="85594-131">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="85594-131">extensionAttribute6</span></span>|<span data-ttu-id="85594-132">String</span><span class="sxs-lookup"><span data-stu-id="85594-132">String</span></span>| <span data-ttu-id="85594-133">Sexto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="85594-133">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="85594-134">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="85594-134">extensionAttribute7</span></span>|<span data-ttu-id="85594-135">String</span><span class="sxs-lookup"><span data-stu-id="85594-135">String</span></span>| <span data-ttu-id="85594-136">Sétimo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="85594-136">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="85594-137">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="85594-137">extensionAttribute8</span></span>|<span data-ttu-id="85594-138">String</span><span class="sxs-lookup"><span data-stu-id="85594-138">String</span></span>| <span data-ttu-id="85594-139">Oitavo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="85594-139">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="85594-140">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="85594-140">extensionAttribute9</span></span>|<span data-ttu-id="85594-141">String</span><span class="sxs-lookup"><span data-stu-id="85594-141">String</span></span>| <span data-ttu-id="85594-142">Nono atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="85594-142">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="85594-143">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="85594-143">extensionAttribute10</span></span>|<span data-ttu-id="85594-144">String</span><span class="sxs-lookup"><span data-stu-id="85594-144">String</span></span>| <span data-ttu-id="85594-145">Décimo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="85594-145">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="85594-146">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="85594-146">extensionAttribute11</span></span>|<span data-ttu-id="85594-147">String</span><span class="sxs-lookup"><span data-stu-id="85594-147">String</span></span>| <span data-ttu-id="85594-148">Décimo primeiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="85594-148">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="85594-149">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="85594-149">extensionAttribute12</span></span>|<span data-ttu-id="85594-150">String</span><span class="sxs-lookup"><span data-stu-id="85594-150">String</span></span>| <span data-ttu-id="85594-151">Décimo segundo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="85594-151">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="85594-152">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="85594-152">extensionAttribute13</span></span>|<span data-ttu-id="85594-153">String</span><span class="sxs-lookup"><span data-stu-id="85594-153">String</span></span>| <span data-ttu-id="85594-154">Décimo terceiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="85594-154">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="85594-155">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="85594-155">extensionAttribute14</span></span>|<span data-ttu-id="85594-156">String</span><span class="sxs-lookup"><span data-stu-id="85594-156">String</span></span>| <span data-ttu-id="85594-157">Décimo quarto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="85594-157">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="85594-158">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="85594-158">extensionAttribute15</span></span>|<span data-ttu-id="85594-159">String</span><span class="sxs-lookup"><span data-stu-id="85594-159">String</span></span>| <span data-ttu-id="85594-160">Décimo quinto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="85594-160">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="85594-161">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="85594-161">JSON representation</span></span>

<span data-ttu-id="85594-162">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="85594-162">Here is a JSON representation of the resource</span></span>

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

