---
title: Tipo de recurso plannerExternalReference
description: O recurso de **plannerExternalReference** representa os metadados de uma referência (anexos como arquivo, URL). É o valor de pares de valor da propriedade no objeto externalReferences.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: f95c6661dd179a7078980894b87184059598319d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952171"
---
# <a name="plannerexternalreference-resource-type"></a><span data-ttu-id="be3b8-104">Tipo de recurso plannerExternalReference</span><span class="sxs-lookup"><span data-stu-id="be3b8-104">plannerExternalReference resource type</span></span>

<span data-ttu-id="be3b8-p102">O recurso **plannerExternalReference** representa os metadados de uma referência (anexos como arquivo, URL). É o valor de pares propriedade-valor no [objeto externalReferences](plannerexternalreferences.md).</span><span class="sxs-lookup"><span data-stu-id="be3b8-p102">The **plannerExternalReference** resource represents the metadata of a reference (attachments such as file, URL). It is the value of property-value pairs in the [externalReferences object](plannerexternalreferences.md).</span></span>



## <a name="properties"></a><span data-ttu-id="be3b8-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="be3b8-107">Properties</span></span>
| <span data-ttu-id="be3b8-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="be3b8-108">Property</span></span>     | <span data-ttu-id="be3b8-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="be3b8-109">Type</span></span>   |<span data-ttu-id="be3b8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="be3b8-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="be3b8-111">alias</span><span class="sxs-lookup"><span data-stu-id="be3b8-111">alias</span></span>|<span data-ttu-id="be3b8-112">String</span><span class="sxs-lookup"><span data-stu-id="be3b8-112">String</span></span>|<span data-ttu-id="be3b8-113">Um alias de nome para descrever a referência.</span><span class="sxs-lookup"><span data-stu-id="be3b8-113">A name alias to describe the reference.</span></span>|
|<span data-ttu-id="be3b8-114">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="be3b8-114">lastModifiedBy</span></span>|[<span data-ttu-id="be3b8-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="be3b8-115">identitySet</span></span>](identityset.md)|<span data-ttu-id="be3b8-p103">Somente leitura. A identificação de usuário pela qual isso foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="be3b8-p103">Read-only. User ID by which this is last modified.</span></span>|
|<span data-ttu-id="be3b8-118">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="be3b8-118">lastModifiedDateTime</span></span>|<span data-ttu-id="be3b8-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be3b8-119">DateTimeOffset</span></span>|<span data-ttu-id="be3b8-p104">Somente leitura. A data e a hora pelas quais isso foi modificado pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="be3b8-p104">Read-only. Date and time at which this is last modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="be3b8-124">previewPriority</span><span class="sxs-lookup"><span data-stu-id="be3b8-124">previewPriority</span></span>|<span data-ttu-id="be3b8-125">String</span><span class="sxs-lookup"><span data-stu-id="be3b8-125">String</span></span>|<span data-ttu-id="be3b8-126">Usado para definir a ordem de prioridade relativa na qual a referência será mostrada como uma visualização na tarefa.</span><span class="sxs-lookup"><span data-stu-id="be3b8-126">Used to set the relative priority order in which the reference will be shown as a preview on the task.</span></span>|
|<span data-ttu-id="be3b8-127">type</span><span class="sxs-lookup"><span data-stu-id="be3b8-127">type</span></span>|<span data-ttu-id="be3b8-128">String</span><span class="sxs-lookup"><span data-stu-id="be3b8-128">String</span></span>|<span data-ttu-id="be3b8-p105">Usado para descrever o tipo da referência. Os tipos incluem: `PowerPoint`, `Word`, `Excel`, `Other`.</span><span class="sxs-lookup"><span data-stu-id="be3b8-p105">Used to describe the type of the reference. Types include: `PowerPoint`, `Word`, `Excel`, `Other`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="be3b8-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="be3b8-131">JSON representation</span></span>
<span data-ttu-id="be3b8-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="be3b8-132">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerExternalReference"
}-->

```json
{
  "alias": "String",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "previewPriority": "String",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerExternalReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
