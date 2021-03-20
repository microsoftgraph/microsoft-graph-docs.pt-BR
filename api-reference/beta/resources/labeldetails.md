---
title: Tipo de recurso labelDetails
description: Representa os detalhes do rótulo de um rótulo de proteção de informações.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 214589dfcb26497b5271008f8a358d06a4fb700f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950300"
---
# <a name="labeldetails-resource-type"></a><span data-ttu-id="51a24-103">Tipo de recurso labelDetails</span><span class="sxs-lookup"><span data-stu-id="51a24-103">labelDetails resource type</span></span>

<span data-ttu-id="51a24-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51a24-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51a24-105">Representa os detalhes do rótulo de um rótulo de proteção de informações.</span><span class="sxs-lookup"><span data-stu-id="51a24-105">Represents the label details of an information protection label.</span></span> <span data-ttu-id="51a24-106">**labelDetails** fornece informações sobre um único rótulo de proteção de informações.</span><span class="sxs-lookup"><span data-stu-id="51a24-106">**labelDetails** provides information about a single information protection label.</span></span> <span data-ttu-id="51a24-107">Pode ser retornado [por evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md), [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md)e [extractLabel](../api/informationprotectionlabel-extractLabel.md)</span><span class="sxs-lookup"><span data-stu-id="51a24-107">Can be returned by [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md), [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), and [extractLabel](../api/informationprotectionlabel-extractLabel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="51a24-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="51a24-108">Properties</span></span>

| <span data-ttu-id="51a24-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="51a24-109">Property</span></span>    | <span data-ttu-id="51a24-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="51a24-110">Type</span></span>    | <span data-ttu-id="51a24-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="51a24-111">Description</span></span>                                                                                                  |
| :---------- | :------ | :----------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="51a24-112">color</span><span class="sxs-lookup"><span data-stu-id="51a24-112">color</span></span>       | <span data-ttu-id="51a24-113">String</span><span class="sxs-lookup"><span data-stu-id="51a24-113">String</span></span>  | <span data-ttu-id="51a24-114">A cor que a interface do usuário deve exibir para o rótulo, se configurada.</span><span class="sxs-lookup"><span data-stu-id="51a24-114">The color that the user interface should display for the label, if configured.</span></span>                               |
| <span data-ttu-id="51a24-115">description</span><span class="sxs-lookup"><span data-stu-id="51a24-115">description</span></span> | <span data-ttu-id="51a24-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51a24-116">String</span></span>  | <span data-ttu-id="51a24-117">A descrição definida pelo administrador para o rótulo.</span><span class="sxs-lookup"><span data-stu-id="51a24-117">The admin-defined description for the label.</span></span>                                                                 |
| <span data-ttu-id="51a24-118">id</span><span class="sxs-lookup"><span data-stu-id="51a24-118">id</span></span>          | <span data-ttu-id="51a24-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51a24-119">String</span></span>  | <span data-ttu-id="51a24-120">A ID do rótulo é um identificador global exclusivo (GUID).</span><span class="sxs-lookup"><span data-stu-id="51a24-120">The label ID is a globally unique identifier (GUID).</span></span>                                                          |
| <span data-ttu-id="51a24-121">isActive</span><span class="sxs-lookup"><span data-stu-id="51a24-121">isActive</span></span>    | <span data-ttu-id="51a24-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="51a24-122">Boolean</span></span> | <span data-ttu-id="51a24-123">Indica se o rótulo está ativo ou não.</span><span class="sxs-lookup"><span data-stu-id="51a24-123">Indicates whether the label is active or not.</span></span> <span data-ttu-id="51a24-124">Os rótulos ativos devem ser ocultos ou desabilitados nas interfaces do usuário.</span><span class="sxs-lookup"><span data-stu-id="51a24-124">Active labels should be hidden or disabled in user interfaces.</span></span> |
| <span data-ttu-id="51a24-125">nome</span><span class="sxs-lookup"><span data-stu-id="51a24-125">name</span></span>        | <span data-ttu-id="51a24-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51a24-126">String</span></span>  | <span data-ttu-id="51a24-127">O nome do texto sem formatção do rótulo.</span><span class="sxs-lookup"><span data-stu-id="51a24-127">The plaintext name of the label.</span></span>                                                                             |
| <span data-ttu-id="51a24-128">sensibilidade</span><span class="sxs-lookup"><span data-stu-id="51a24-128">sensitivity</span></span> | <span data-ttu-id="51a24-129">Int32</span><span class="sxs-lookup"><span data-stu-id="51a24-129">Int32</span></span>   | <span data-ttu-id="51a24-130">O valor de sensibilidade do rótulo, onde menor é menos sensível.</span><span class="sxs-lookup"><span data-stu-id="51a24-130">The sensitivity value of the label, where lower is less sensitive.</span></span>                                           |
| <span data-ttu-id="51a24-131">tooltip</span><span class="sxs-lookup"><span data-stu-id="51a24-131">tooltip</span></span>     | <span data-ttu-id="51a24-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51a24-132">String</span></span>  | <span data-ttu-id="51a24-133">A dica de ferramenta que deve ser exibida para o rótulo em uma interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="51a24-133">The tooltip that should be displayed for the label in a user interface.</span></span>                                      |

## <a name="json-representation"></a><span data-ttu-id="51a24-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="51a24-134">JSON representation</span></span>

<span data-ttu-id="51a24-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="51a24-135">The following is a JSON representation of the resource.</span></span>

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

