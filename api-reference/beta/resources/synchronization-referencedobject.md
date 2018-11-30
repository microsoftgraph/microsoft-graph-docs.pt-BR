---
title: tipo de recurso de referencedObject
description: Descreve uma referência a outro objeto definido na mesma definição de diretório.
ms.openlocfilehash: 63645048fd8ba6ad949da43baa261b2842ea4016
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040369"
---
# <a name="referencedobject-resource-type"></a><span data-ttu-id="c1d0b-103">tipo de recurso de referencedObject</span><span class="sxs-lookup"><span data-stu-id="c1d0b-103">referencedObject resource type</span></span>

> <span data-ttu-id="c1d0b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c1d0b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c1d0b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c1d0b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c1d0b-106">Descreve uma referência a outro objeto definido na mesma [definição de diretório](synchronization-directorydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c1d0b-106">Describes a reference to another object defined in the same [directory definition](synchronization-directorydefinition.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c1d0b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c1d0b-107">Properties</span></span>

| <span data-ttu-id="c1d0b-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c1d0b-108">Property</span></span>                   | <span data-ttu-id="c1d0b-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="c1d0b-109">Type</span></span>                      | <span data-ttu-id="c1d0b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1d0b-110">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="c1d0b-111">referencedObjectName</span><span class="sxs-lookup"><span data-stu-id="c1d0b-111">referencedObjectName</span></span>        |<span data-ttu-id="c1d0b-112">String</span><span class="sxs-lookup"><span data-stu-id="c1d0b-112">String</span></span>                     |<span data-ttu-id="c1d0b-113">Nome do objeto referenciado.</span><span class="sxs-lookup"><span data-stu-id="c1d0b-113">Name of the referenced object.</span></span> <span data-ttu-id="c1d0b-114">Deve corresponder a um dos objetos na [definição de diretório](synchronization-directorydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c1d0b-114">Must match one of the objects in the [directory definition](synchronization-directorydefinition.md).</span></span>|
|<span data-ttu-id="c1d0b-115">referencedProperty</span><span class="sxs-lookup"><span data-stu-id="c1d0b-115">referencedProperty</span></span>          |<span data-ttu-id="c1d0b-116">String</span><span class="sxs-lookup"><span data-stu-id="c1d0b-116">String</span></span>                     |<span data-ttu-id="c1d0b-117">**No momento não tem suporte**.</span><span class="sxs-lookup"><span data-stu-id="c1d0b-117">**Currently not supported**.</span></span> <span data-ttu-id="c1d0b-118">Nome da propriedade no objeto referenciado, o valor para o qual é usado como referência.</span><span class="sxs-lookup"><span data-stu-id="c1d0b-118">Name of the property in the referenced object, the value for which is used as the reference.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c1d0b-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c1d0b-119">JSON representation</span></span>

<span data-ttu-id="c1d0b-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c1d0b-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.referencedObject"
}-->

```json
{
  "referencedObjectName": "String",
  "referencedProperty": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "referencedObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
            