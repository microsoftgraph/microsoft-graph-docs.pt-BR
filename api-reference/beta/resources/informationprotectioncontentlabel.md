---
title: tipo de recurso informationProtectionContentLabel
description: Descreve o objeto informationProtectionContentLabel que define metadados MIP em um objeto.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8422f83db0c94eed74d5690343c51b70e2d87d82
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016447"
---
# <a name="informationprotectioncontentlabel-resource-type"></a><span data-ttu-id="28e34-103">tipo de recurso informationProtectionContentLabel</span><span class="sxs-lookup"><span data-stu-id="28e34-103">informationProtectionContentLabel resource type</span></span>

<span data-ttu-id="28e34-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28e34-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28e34-105">Descreve o objeto informationProtectionContentLabel que define metadados MIP em um objeto.</span><span class="sxs-lookup"><span data-stu-id="28e34-105">Describes the informationProtectionContentLabel object that defines MIP metadata on an object.</span></span> <span data-ttu-id="28e34-106">**informationProtectionContentLabel** é retornado pela API [extractLabel](../api/informationprotectionlabel-extractLabel.md) resolvida para o rótulo atualmente aplicado a um arquivo.</span><span class="sxs-lookup"><span data-stu-id="28e34-106">**informationProtectionContentLabel** is returned by the [extractLabel](../api/informationprotectionlabel-extractLabel.md) API resolve to the label that is currently applied to a file.</span></span> 

## <a name="properties"></a><span data-ttu-id="28e34-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="28e34-107">Properties</span></span>

| <span data-ttu-id="28e34-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="28e34-108">Property</span></span>     | <span data-ttu-id="28e34-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="28e34-109">Type</span></span>        | <span data-ttu-id="28e34-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="28e34-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="28e34-111">AssignmentMethod for utilizado</span><span class="sxs-lookup"><span data-stu-id="28e34-111">assignmentMethod</span></span>|<span data-ttu-id="28e34-112">String</span><span class="sxs-lookup"><span data-stu-id="28e34-112">String</span></span>| <span data-ttu-id="28e34-113">Os valores possíveis são: `standard`, `privileged`, `auto`.</span><span class="sxs-lookup"><span data-stu-id="28e34-113">Possible values are: `standard`, `privileged`, `auto`.</span></span>|
|<span data-ttu-id="28e34-114">creationDatetime</span><span class="sxs-lookup"><span data-stu-id="28e34-114">creationDateTime</span></span>|<span data-ttu-id="28e34-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28e34-115">DateTimeOffset</span></span>|<span data-ttu-id="28e34-p102">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="28e34-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="28e34-118">rótulo</span><span class="sxs-lookup"><span data-stu-id="28e34-118">label</span></span>|[<span data-ttu-id="28e34-119">labelDetails</span><span class="sxs-lookup"><span data-stu-id="28e34-119">labelDetails</span></span>](labeldetails.md)| <span data-ttu-id="28e34-120">Detalhes sobre o rótulo que é aplicado atualmente ao arquivo.</span><span class="sxs-lookup"><span data-stu-id="28e34-120">Details on the label that is currently applied to the file.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="28e34-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="28e34-121">JSON representation</span></span>

<span data-ttu-id="28e34-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="28e34-122">The following is a JSON representation of the resource.</span></span>

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

