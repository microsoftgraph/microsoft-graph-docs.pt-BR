---
title: tipo de recurso referenciouobject
description: Descreve uma referência a outro objeto definido na mesma definição de diretório.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9ea400e40074b30943412cf7b5fbae75f9037ca1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023881"
---
# <a name="referencedobject-resource-type"></a><span data-ttu-id="49de6-103">tipo de recurso referenciouobject</span><span class="sxs-lookup"><span data-stu-id="49de6-103">referencedObject resource type</span></span>

<span data-ttu-id="49de6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49de6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49de6-105">Descreve uma referência a outro objeto definido na mesma [definição de diretório](synchronization-directorydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="49de6-105">Describes a reference to another object defined in the same [directory definition](synchronization-directorydefinition.md).</span></span>

## <a name="properties"></a><span data-ttu-id="49de6-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="49de6-106">Properties</span></span>

| <span data-ttu-id="49de6-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="49de6-107">Property</span></span>                   | <span data-ttu-id="49de6-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="49de6-108">Type</span></span>                      | <span data-ttu-id="49de6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="49de6-109">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="49de6-110">referencedObjectName</span><span class="sxs-lookup"><span data-stu-id="49de6-110">referencedObjectName</span></span>        |<span data-ttu-id="49de6-111">String</span><span class="sxs-lookup"><span data-stu-id="49de6-111">String</span></span>                     |<span data-ttu-id="49de6-112">Nome do objeto referenciado.</span><span class="sxs-lookup"><span data-stu-id="49de6-112">Name of the referenced object.</span></span> <span data-ttu-id="49de6-113">Deve corresponder a um dos objetos na [definição de diretório](synchronization-directorydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="49de6-113">Must match one of the objects in the [directory definition](synchronization-directorydefinition.md).</span></span>|
|<span data-ttu-id="49de6-114">referenciouproperty</span><span class="sxs-lookup"><span data-stu-id="49de6-114">referencedProperty</span></span>          |<span data-ttu-id="49de6-115">String</span><span class="sxs-lookup"><span data-stu-id="49de6-115">String</span></span>                     |<span data-ttu-id="49de6-116">**Não suportado no momento**.</span><span class="sxs-lookup"><span data-stu-id="49de6-116">**Currently not supported**.</span></span> <span data-ttu-id="49de6-117">Nome da propriedade no objeto referenciado, o valor para o qual é usado como a referência.</span><span class="sxs-lookup"><span data-stu-id="49de6-117">Name of the property in the referenced object, the value for which is used as the reference.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="49de6-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="49de6-118">JSON representation</span></span>

<span data-ttu-id="49de6-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="49de6-119">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "referencedObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
            


