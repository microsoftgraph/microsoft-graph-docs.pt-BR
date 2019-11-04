---
title: tipo de recurso informationProtectionContentLabel
description: Descreve o objeto informationProtectionContentLabel que define metadados MIP em um objeto.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4f615655110ffdc6b76469d3d29cd4d13663d511
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938825"
---
# <a name="informationprotectioncontentlabel-resource-type"></a><span data-ttu-id="79b23-103">tipo de recurso informationProtectionContentLabel</span><span class="sxs-lookup"><span data-stu-id="79b23-103">informationProtectionContentLabel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79b23-104">Descreve o objeto informationProtectionContentLabel que define metadados MIP em um objeto.</span><span class="sxs-lookup"><span data-stu-id="79b23-104">Describes the informationProtectionContentLabel object that defines MIP metadata on an object.</span></span> <span data-ttu-id="79b23-105">**informationProtectionContentLabel** é retornado pela API [extractLabel](../api/informationprotectionlabel-extractLabel.md) resolvida para o rótulo atualmente aplicado a um arquivo.</span><span class="sxs-lookup"><span data-stu-id="79b23-105">**informationProtectionContentLabel** is returned by the [extractLabel](../api/informationprotectionlabel-extractLabel.md) API resolve to the label that is currently applied to a file.</span></span> 

## <a name="properties"></a><span data-ttu-id="79b23-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="79b23-106">Properties</span></span>

| <span data-ttu-id="79b23-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="79b23-107">Property</span></span>     | <span data-ttu-id="79b23-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="79b23-108">Type</span></span>        | <span data-ttu-id="79b23-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="79b23-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="79b23-110">AssignmentMethod for utilizado</span><span class="sxs-lookup"><span data-stu-id="79b23-110">assignmentMethod</span></span>|<span data-ttu-id="79b23-111">String</span><span class="sxs-lookup"><span data-stu-id="79b23-111">String</span></span>| <span data-ttu-id="79b23-112">Os valores possíveis são: `standard`, `privileged`, `auto`.</span><span class="sxs-lookup"><span data-stu-id="79b23-112">Possible values are: `standard`, `privileged`, `auto`.</span></span>|
|<span data-ttu-id="79b23-113">creationDatetime</span><span class="sxs-lookup"><span data-stu-id="79b23-113">creationDateTime</span></span>|<span data-ttu-id="79b23-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79b23-114">DateTimeOffset</span></span>|<span data-ttu-id="79b23-p102">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="79b23-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="79b23-117">rótulo</span><span class="sxs-lookup"><span data-stu-id="79b23-117">label</span></span>|[<span data-ttu-id="79b23-118">labelDetails</span><span class="sxs-lookup"><span data-stu-id="79b23-118">labelDetails</span></span>](labeldetails.md)| <span data-ttu-id="79b23-119">Detalhes sobre o rótulo que é aplicado atualmente ao arquivo.</span><span class="sxs-lookup"><span data-stu-id="79b23-119">Details on the label that is currently applied to the file.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="79b23-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="79b23-120">JSON representation</span></span>

<span data-ttu-id="79b23-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="79b23-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.informationProtectionContentLabel",
  "baseType": null
}-->

```json
{
  "assignmentMethod": "String",
  "creationDateTime": "String (timestamp)",
  "label": {"@odata.type": "microsoft.graph.labelDetails"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "informationProtectionContentLabel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->