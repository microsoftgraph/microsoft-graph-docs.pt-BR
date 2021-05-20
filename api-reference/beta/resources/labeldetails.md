---
title: Tipo de recurso labelDetails
description: Representa os detalhes do rótulo de um rótulo de proteção de informações.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: eb66e395d18b7887942753abdebd91d398844290
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579288"
---
# <a name="labeldetails-resource-type"></a><span data-ttu-id="99fdb-103">Tipo de recurso labelDetails</span><span class="sxs-lookup"><span data-stu-id="99fdb-103">labelDetails resource type</span></span>

<span data-ttu-id="99fdb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99fdb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99fdb-105">Representa os detalhes do rótulo de um rótulo de proteção de informações.</span><span class="sxs-lookup"><span data-stu-id="99fdb-105">Represents the label details of an information protection label.</span></span> <span data-ttu-id="99fdb-106">**labelDetails** fornece informações sobre um único rótulo de proteção de informações.</span><span class="sxs-lookup"><span data-stu-id="99fdb-106">**labelDetails** provides information about a single information protection label.</span></span> <span data-ttu-id="99fdb-107">Herda do [parentLabelDetails](parentlabeldetails.md).</span><span class="sxs-lookup"><span data-stu-id="99fdb-107">Inherits from the [parentLabelDetails](parentlabeldetails.md).</span></span> <span data-ttu-id="99fdb-108">Pode ser retornado [por evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md), [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md)e [extractLabel](../api/informationprotectionlabel-extractLabel.md)</span><span class="sxs-lookup"><span data-stu-id="99fdb-108">Can be returned by [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md), [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), and [extractLabel](../api/informationprotectionlabel-extractLabel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="99fdb-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="99fdb-109">Properties</span></span>

| <span data-ttu-id="99fdb-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="99fdb-110">Property</span></span>    | <span data-ttu-id="99fdb-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="99fdb-111">Type</span></span>                                         | <span data-ttu-id="99fdb-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="99fdb-112">Description</span></span>                                                                                                  |
| :---------- | :------------------------------------------- | :----------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="99fdb-113">color</span><span class="sxs-lookup"><span data-stu-id="99fdb-113">color</span></span>       | <span data-ttu-id="99fdb-114">String</span><span class="sxs-lookup"><span data-stu-id="99fdb-114">String</span></span>                                       | <span data-ttu-id="99fdb-115">A cor que a interface do usuário deve exibir para o rótulo, se configurada.</span><span class="sxs-lookup"><span data-stu-id="99fdb-115">The color that the user interface should display for the label, if configured.</span></span>                               |
| <span data-ttu-id="99fdb-116">descrição</span><span class="sxs-lookup"><span data-stu-id="99fdb-116">description</span></span> | <span data-ttu-id="99fdb-117">String</span><span class="sxs-lookup"><span data-stu-id="99fdb-117">String</span></span>                                       | <span data-ttu-id="99fdb-118">A descrição definida pelo administrador para o rótulo.</span><span class="sxs-lookup"><span data-stu-id="99fdb-118">The admin-defined description for the label.</span></span>                                                                 |
| <span data-ttu-id="99fdb-119">id</span><span class="sxs-lookup"><span data-stu-id="99fdb-119">id</span></span>          | <span data-ttu-id="99fdb-120">String</span><span class="sxs-lookup"><span data-stu-id="99fdb-120">String</span></span>                                       | <span data-ttu-id="99fdb-121">A ID do rótulo é um identificador global exclusivo (GUID).</span><span class="sxs-lookup"><span data-stu-id="99fdb-121">The label ID is a globally unique identifier (GUID).</span></span>                                                         |
| <span data-ttu-id="99fdb-122">isActive</span><span class="sxs-lookup"><span data-stu-id="99fdb-122">isActive</span></span>    | <span data-ttu-id="99fdb-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="99fdb-123">Boolean</span></span>                                      | <span data-ttu-id="99fdb-124">Indica se o rótulo está ativo ou não.</span><span class="sxs-lookup"><span data-stu-id="99fdb-124">Indicates whether the label is active or not.</span></span> <span data-ttu-id="99fdb-125">Os rótulos ativos devem ser ocultos ou desabilitados nas interfaces do usuário.</span><span class="sxs-lookup"><span data-stu-id="99fdb-125">Active labels should be hidden or disabled in user interfaces.</span></span> |
| <span data-ttu-id="99fdb-126">nome</span><span class="sxs-lookup"><span data-stu-id="99fdb-126">name</span></span>        | <span data-ttu-id="99fdb-127">String</span><span class="sxs-lookup"><span data-stu-id="99fdb-127">String</span></span>                                       | <span data-ttu-id="99fdb-128">O nome do texto sem formatção do rótulo.</span><span class="sxs-lookup"><span data-stu-id="99fdb-128">The plaintext name of the label.</span></span>                                                                             |
| <span data-ttu-id="99fdb-129">sensitivity</span><span class="sxs-lookup"><span data-stu-id="99fdb-129">sensitivity</span></span> | <span data-ttu-id="99fdb-130">Int32</span><span class="sxs-lookup"><span data-stu-id="99fdb-130">Int32</span></span>                                        | <span data-ttu-id="99fdb-131">O valor de sensibilidade do rótulo, onde menor é menos sensível.</span><span class="sxs-lookup"><span data-stu-id="99fdb-131">The sensitivity value of the label, where lower is less sensitive.</span></span>                                           |
| <span data-ttu-id="99fdb-132">tooltip</span><span class="sxs-lookup"><span data-stu-id="99fdb-132">tooltip</span></span>     | <span data-ttu-id="99fdb-133">String</span><span class="sxs-lookup"><span data-stu-id="99fdb-133">String</span></span>                                       | <span data-ttu-id="99fdb-134">A dica de ferramenta que deve ser exibida para o rótulo em uma interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="99fdb-134">The tooltip that should be displayed for the label in a user interface.</span></span>                                      |
| <span data-ttu-id="99fdb-135">primário</span><span class="sxs-lookup"><span data-stu-id="99fdb-135">parent</span></span>      | <span data-ttu-id="99fdb-136">parentLabelDetails</span><span class="sxs-lookup"><span data-stu-id="99fdb-136">parentLabelDetails</span></span> | <span data-ttu-id="99fdb-137">O rótulo pai associado a um rótulo filho.</span><span class="sxs-lookup"><span data-stu-id="99fdb-137">The parent label associated with a child label.</span></span>                                                              |

## <a name="json-representation"></a><span data-ttu-id="99fdb-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="99fdb-138">JSON representation</span></span>

<span data-ttu-id="99fdb-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="99fdb-139">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.labelDetails",
  "baseType": null
}-->

```json
{
  "color": "String",
  "description": "String",
  "id": "String",
  "isActive": true,
  "name": "String",
  "sensitivity": 1024,
  "tooltip": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "labelDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

