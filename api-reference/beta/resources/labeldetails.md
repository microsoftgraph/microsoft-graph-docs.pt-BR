---
title: tipo de recurso labelDetails
description: Representa os detalhes do rótulo de um rótulo de proteção de informações.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7f2ff99f6f7548e9176358219d70cd55e1232a05
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939170"
---
# <a name="labeldetails-resource-type"></a><span data-ttu-id="c9369-103">tipo de recurso labelDetails</span><span class="sxs-lookup"><span data-stu-id="c9369-103">labelDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9369-104">Representa os detalhes do rótulo de um rótulo de proteção de informações.</span><span class="sxs-lookup"><span data-stu-id="c9369-104">Represents the label details of an information protection label.</span></span> <span data-ttu-id="c9369-105">**labelDetails** fornece informações sobre um único rótulo de proteção de informações.</span><span class="sxs-lookup"><span data-stu-id="c9369-105">**labelDetails** provides information about a single information protection label.</span></span> <span data-ttu-id="c9369-106">Pode ser retornado por [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md), [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md)e [extractLabel](../api/informationprotectionlabel-extractLabel.md)</span><span class="sxs-lookup"><span data-stu-id="c9369-106">Can be returned by [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md), [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), and [extractLabel](../api/informationprotectionlabel-extractLabel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c9369-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c9369-107">Properties</span></span>

| <span data-ttu-id="c9369-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c9369-108">Property</span></span>    | <span data-ttu-id="c9369-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="c9369-109">Type</span></span>    | <span data-ttu-id="c9369-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9369-110">Description</span></span>                                                                                                  |
| :---------- | :------ | :----------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="c9369-111">color</span><span class="sxs-lookup"><span data-stu-id="c9369-111">color</span></span>       | <span data-ttu-id="c9369-112">String</span><span class="sxs-lookup"><span data-stu-id="c9369-112">String</span></span>  | <span data-ttu-id="c9369-113">A cor que a interface do usuário deve exibir para o rótulo, se configurada.</span><span class="sxs-lookup"><span data-stu-id="c9369-113">The color that the user interface should display for the label, if configured.</span></span>                               |
| <span data-ttu-id="c9369-114">description</span><span class="sxs-lookup"><span data-stu-id="c9369-114">description</span></span> | <span data-ttu-id="c9369-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c9369-115">String</span></span>  | <span data-ttu-id="c9369-116">A descrição definida pelo administrador para o rótulo.</span><span class="sxs-lookup"><span data-stu-id="c9369-116">The admin-defined description for the label.</span></span>                                                                 |
| <span data-ttu-id="c9369-117">id</span><span class="sxs-lookup"><span data-stu-id="c9369-117">id</span></span>          | <span data-ttu-id="c9369-118">String</span><span class="sxs-lookup"><span data-stu-id="c9369-118">String</span></span>  | <span data-ttu-id="c9369-119">A ID do rótulo é um identificador global exclusivo (GUID).</span><span class="sxs-lookup"><span data-stu-id="c9369-119">The label ID is a globally unique identifier (GUID).</span></span>                                                          |
| <span data-ttu-id="c9369-120">isActive</span><span class="sxs-lookup"><span data-stu-id="c9369-120">isActive</span></span>    | <span data-ttu-id="c9369-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="c9369-121">Boolean</span></span> | <span data-ttu-id="c9369-122">Indica se o rótulo está ativo ou não.</span><span class="sxs-lookup"><span data-stu-id="c9369-122">Indicates whether the label is active or not.</span></span> <span data-ttu-id="c9369-123">Os rótulos ativos devem ser ocultos ou desabilitados nas interfaces de usuário.</span><span class="sxs-lookup"><span data-stu-id="c9369-123">Active labels should be hidden or disabled in user interfaces.</span></span> |
| <span data-ttu-id="c9369-124">name</span><span class="sxs-lookup"><span data-stu-id="c9369-124">name</span></span>        | <span data-ttu-id="c9369-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c9369-125">String</span></span>  | <span data-ttu-id="c9369-126">O nome de texto não criptografado do rótulo.</span><span class="sxs-lookup"><span data-stu-id="c9369-126">The plaintext name of the label.</span></span>                                                                             |
| <span data-ttu-id="c9369-127">sensitivity</span><span class="sxs-lookup"><span data-stu-id="c9369-127">sensitivity</span></span> | <span data-ttu-id="c9369-128">Int32</span><span class="sxs-lookup"><span data-stu-id="c9369-128">Int32</span></span>   | <span data-ttu-id="c9369-129">O valor de confidencialidade do rótulo, onde inferior é menos confidencial.</span><span class="sxs-lookup"><span data-stu-id="c9369-129">The sensitivity value of the label, where lower is less sensitive.</span></span>                                           |
| <span data-ttu-id="c9369-130">tooltip</span><span class="sxs-lookup"><span data-stu-id="c9369-130">tooltip</span></span>     | <span data-ttu-id="c9369-131">String</span><span class="sxs-lookup"><span data-stu-id="c9369-131">String</span></span>  | <span data-ttu-id="c9369-132">A dica de ferramenta que deve ser exibida para o rótulo em uma interface de usuário.</span><span class="sxs-lookup"><span data-stu-id="c9369-132">The tooltip that should be displayed for the label in a user interface.</span></span>                                      |

## <a name="json-representation"></a><span data-ttu-id="c9369-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c9369-133">JSON representation</span></span>

<span data-ttu-id="c9369-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c9369-134">The following is a JSON representation of the resource.</span></span>

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