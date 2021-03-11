---
title: Tipo de recurso informationProtectionContentLabel
description: Descreve o objeto informationProtectionContentLabel que define metadados MIP em um objeto.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a7905a585b28832829d838db94344b28f691644d
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50718516"
---
# <a name="informationprotectioncontentlabel-resource-type"></a><span data-ttu-id="5338f-103">Tipo de recurso informationProtectionContentLabel</span><span class="sxs-lookup"><span data-stu-id="5338f-103">informationProtectionContentLabel resource type</span></span>

<span data-ttu-id="5338f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5338f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5338f-105">Descreve o objeto informationProtectionContentLabel que define metadados MIP em um objeto.</span><span class="sxs-lookup"><span data-stu-id="5338f-105">Describes the informationProtectionContentLabel object that defines MIP metadata on an object.</span></span> <span data-ttu-id="5338f-106">**informationProtectionContentLabel** é retornado pela solução da API [extractLabel](../api/informationprotectionlabel-extractLabel.md) para o rótulo que está atualmente aplicado a um arquivo.</span><span class="sxs-lookup"><span data-stu-id="5338f-106">**informationProtectionContentLabel** is returned by the [extractLabel](../api/informationprotectionlabel-extractLabel.md) API resolve to the label that is currently applied to a file.</span></span> 

## <a name="properties"></a><span data-ttu-id="5338f-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5338f-107">Properties</span></span>

| <span data-ttu-id="5338f-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5338f-108">Property</span></span>     | <span data-ttu-id="5338f-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="5338f-109">Type</span></span>        | <span data-ttu-id="5338f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5338f-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5338f-111">assignmentMethod</span><span class="sxs-lookup"><span data-stu-id="5338f-111">assignmentMethod</span></span>|<span data-ttu-id="5338f-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5338f-112">String</span></span>| <span data-ttu-id="5338f-113">Os valores possíveis são: `standard`, `privileged`, `auto`.</span><span class="sxs-lookup"><span data-stu-id="5338f-113">Possible values are: `standard`, `privileged`, `auto`.</span></span>|
|<span data-ttu-id="5338f-114">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="5338f-114">creationDateTime</span></span>|<span data-ttu-id="5338f-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5338f-115">DateTimeOffset</span></span>|<span data-ttu-id="5338f-116">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="5338f-116">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5338f-117">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="5338f-117">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="5338f-118">rótulo</span><span class="sxs-lookup"><span data-stu-id="5338f-118">label</span></span>|[<span data-ttu-id="5338f-119">labelDetails</span><span class="sxs-lookup"><span data-stu-id="5338f-119">labelDetails</span></span>](labeldetails.md)| <span data-ttu-id="5338f-120">Detalhes sobre o rótulo que é aplicado no momento ao arquivo.</span><span class="sxs-lookup"><span data-stu-id="5338f-120">Details on the label that is currently applied to the file.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5338f-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5338f-121">JSON representation</span></span>

<span data-ttu-id="5338f-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5338f-122">The following is a JSON representation of the resource.</span></span>

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

