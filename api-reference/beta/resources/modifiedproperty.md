---
title: Tipo de recurso modifiedProperty
description: Descreve as alterações realizadas no sistema de destino.
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 49c2af65022d6fddef394423b6d615dba9f20efc
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136175"
---
# <a name="modifiedproperty-resource-type"></a><span data-ttu-id="86168-103">Tipo de recurso modifiedProperty</span><span class="sxs-lookup"><span data-stu-id="86168-103">modifiedProperty resource type</span></span>

<span data-ttu-id="86168-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86168-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86168-105">Descreve as alterações realizadas no sistema de destino.</span><span class="sxs-lookup"><span data-stu-id="86168-105">Describes the changes performed in the target system.</span></span> 

## <a name="properties"></a><span data-ttu-id="86168-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="86168-106">Properties</span></span>

| <span data-ttu-id="86168-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="86168-107">Property</span></span>     | <span data-ttu-id="86168-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="86168-108">Type</span></span>        | <span data-ttu-id="86168-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="86168-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="86168-110">displayName</span><span class="sxs-lookup"><span data-stu-id="86168-110">displayName</span></span>|<span data-ttu-id="86168-111">String</span><span class="sxs-lookup"><span data-stu-id="86168-111">String</span></span>|<span data-ttu-id="86168-112">Nome da propriedade que foi modificada.</span><span class="sxs-lookup"><span data-stu-id="86168-112">Name of property that was modified.</span></span>|
|<span data-ttu-id="86168-113">newValue</span><span class="sxs-lookup"><span data-stu-id="86168-113">newValue</span></span>|<span data-ttu-id="86168-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="86168-114">String</span></span>|<span data-ttu-id="86168-115">Novo valor de propriedade.</span><span class="sxs-lookup"><span data-stu-id="86168-115">New property value.</span></span>|
|<span data-ttu-id="86168-116">oldValue</span><span class="sxs-lookup"><span data-stu-id="86168-116">oldValue</span></span>|<span data-ttu-id="86168-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="86168-117">String</span></span>|<span data-ttu-id="86168-118">Valor antigo da propriedade.</span><span class="sxs-lookup"><span data-stu-id="86168-118">Old property value.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="86168-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="86168-119">JSON representation</span></span>

<span data-ttu-id="86168-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="86168-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.modifiedProperty",
  "baseType": null
}-->

```json
{
  "displayName": "String",
  "newValue": "String",
  "oldValue": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "modifiedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


