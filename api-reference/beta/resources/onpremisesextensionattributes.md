---
title: Tipo de recurso onPremisesExtensionAttributes
description: A **propriedade onPremisesExtensionAttributes** da entidade do usuário contém quinze propriedades de atributo de extensão personalizadas.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: users
author: jpettere
ms.openlocfilehash: 902ebfa8efe11613d6622d93ec0d39becc9e9bae
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912100"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="3b057-103">Tipo de recurso onPremisesExtensionAttributes</span><span class="sxs-lookup"><span data-stu-id="3b057-103">onPremisesExtensionAttributes resource type</span></span>

<span data-ttu-id="3b057-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b057-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b057-105">A **propriedade onPremisesExtensionAttributes** da entidade do usuário contém quinze propriedades de atributo de extensão personalizadas. [](user.md)</span><span class="sxs-lookup"><span data-stu-id="3b057-105">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="3b057-106">Para um usuário **onPremisesSyncEnabled,** a fonte de autoridade para esse conjunto de propriedades é o Active Directory local que é sincronizado com o Azure AD e é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3b057-106">For an **onPremisesSyncEnabled** user, the source of authority for this set of properties is the on-premises Active Directory which is synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="3b057-107">Para um usuário somente na nuvem (onde **onPremisesSyncEnabled** está ), essas propriedades podem ser definidas durante a `false` [criação](../api/user-post-users.md) ou [atualização.](../api/user-update.md)</span><span class="sxs-lookup"><span data-stu-id="3b057-107">For a cloud-only user (where **onPremisesSyncEnabled** is `false`), these properties may be set during [creation](../api/user-post-users.md) or [update](../api/user-update.md).</span></span>

> <span data-ttu-id="3b057-108">**Observação:** Esses atributos de extensão também são conhecidos como Exchange atributos personalizados 1-15.</span><span class="sxs-lookup"><span data-stu-id="3b057-108">**Note:** These extension attributes are also known as Exchange custom attributes 1-15.</span></span>


## <a name="properties"></a><span data-ttu-id="3b057-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3b057-109">Properties</span></span>
| <span data-ttu-id="3b057-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3b057-110">Property</span></span>     | <span data-ttu-id="3b057-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="3b057-111">Type</span></span>   |<span data-ttu-id="3b057-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b057-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3b057-113">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="3b057-113">extensionAttribute1</span></span>|<span data-ttu-id="3b057-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b057-114">String</span></span>| <span data-ttu-id="3b057-115">Primeiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="3b057-115">First customizable extension attribute.</span></span> |
|<span data-ttu-id="3b057-116">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="3b057-116">extensionAttribute2</span></span>|<span data-ttu-id="3b057-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b057-117">String</span></span>| <span data-ttu-id="3b057-118">Segundo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="3b057-118">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="3b057-119">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="3b057-119">extensionAttribute3</span></span>|<span data-ttu-id="3b057-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b057-120">String</span></span>| <span data-ttu-id="3b057-121">Terceiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="3b057-121">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="3b057-122">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="3b057-122">extensionAttribute4</span></span>|<span data-ttu-id="3b057-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b057-123">String</span></span>| <span data-ttu-id="3b057-124">Quarto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="3b057-124">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="3b057-125">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="3b057-125">extensionAttribute5</span></span>|<span data-ttu-id="3b057-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b057-126">String</span></span>| <span data-ttu-id="3b057-127">Quinto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="3b057-127">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="3b057-128">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="3b057-128">extensionAttribute6</span></span>|<span data-ttu-id="3b057-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b057-129">String</span></span>| <span data-ttu-id="3b057-130">Sexto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="3b057-130">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="3b057-131">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="3b057-131">extensionAttribute7</span></span>|<span data-ttu-id="3b057-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b057-132">String</span></span>| <span data-ttu-id="3b057-133">Sétimo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="3b057-133">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="3b057-134">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="3b057-134">extensionAttribute8</span></span>|<span data-ttu-id="3b057-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b057-135">String</span></span>| <span data-ttu-id="3b057-136">Oitavo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="3b057-136">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="3b057-137">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="3b057-137">extensionAttribute9</span></span>|<span data-ttu-id="3b057-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b057-138">String</span></span>| <span data-ttu-id="3b057-139">Nono atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="3b057-139">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="3b057-140">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="3b057-140">extensionAttribute10</span></span>|<span data-ttu-id="3b057-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b057-141">String</span></span>| <span data-ttu-id="3b057-142">Décimo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="3b057-142">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="3b057-143">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="3b057-143">extensionAttribute11</span></span>|<span data-ttu-id="3b057-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b057-144">String</span></span>| <span data-ttu-id="3b057-145">Décimo primeiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="3b057-145">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="3b057-146">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="3b057-146">extensionAttribute12</span></span>|<span data-ttu-id="3b057-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b057-147">String</span></span>| <span data-ttu-id="3b057-148">Décimo segundo atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="3b057-148">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="3b057-149">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="3b057-149">extensionAttribute13</span></span>|<span data-ttu-id="3b057-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b057-150">String</span></span>| <span data-ttu-id="3b057-151">Décimo terceiro atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="3b057-151">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="3b057-152">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="3b057-152">extensionAttribute14</span></span>|<span data-ttu-id="3b057-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b057-153">String</span></span>| <span data-ttu-id="3b057-154">Décimo quarto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="3b057-154">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="3b057-155">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="3b057-155">extensionAttribute15</span></span>|<span data-ttu-id="3b057-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b057-156">String</span></span>| <span data-ttu-id="3b057-157">Décimo quinto atributo de extensão personalizável.</span><span class="sxs-lookup"><span data-stu-id="3b057-157">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3b057-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3b057-158">JSON representation</span></span>

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


