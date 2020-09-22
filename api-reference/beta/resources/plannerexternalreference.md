---
title: tipo de recurso plannerExternalReference
description: O recurso **plannerExternalReference** representa os metadados de uma referência (anexos como arquivo, URL). É o valor dos pares propriedade-valor no objeto externalReferences.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: ce9cb16c73871289f7bd80058a80c8e61530a894
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029124"
---
# <a name="plannerexternalreference-resource-type"></a><span data-ttu-id="3f042-104">tipo de recurso plannerExternalReference</span><span class="sxs-lookup"><span data-stu-id="3f042-104">plannerExternalReference resource type</span></span>

<span data-ttu-id="3f042-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f042-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f042-106">O recurso **plannerExternalReference** representa os metadados de uma referência (anexos como arquivo, URL).</span><span class="sxs-lookup"><span data-stu-id="3f042-106">The **plannerExternalReference** resource represents the metadata of a reference (attachments such as file, URL).</span></span> <span data-ttu-id="3f042-107">É o valor dos pares propriedade-valor no [objeto externalReferences](plannerexternalreferences.md).</span><span class="sxs-lookup"><span data-stu-id="3f042-107">It is the value of property-value pairs in the [externalReferences object](plannerexternalreferences.md).</span></span>



## <a name="properties"></a><span data-ttu-id="3f042-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3f042-108">Properties</span></span>
| <span data-ttu-id="3f042-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3f042-109">Property</span></span>     | <span data-ttu-id="3f042-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3f042-110">Type</span></span>   |<span data-ttu-id="3f042-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f042-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3f042-112">alias</span><span class="sxs-lookup"><span data-stu-id="3f042-112">alias</span></span>|<span data-ttu-id="3f042-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3f042-113">String</span></span>|<span data-ttu-id="3f042-114">Um alias de nome para descrever a referência.</span><span class="sxs-lookup"><span data-stu-id="3f042-114">A name alias to describe the reference.</span></span>|
|<span data-ttu-id="3f042-115">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="3f042-115">lastModifiedBy</span></span>|[<span data-ttu-id="3f042-116">identitySet</span><span class="sxs-lookup"><span data-stu-id="3f042-116">identitySet</span></span>](identityset.md)|<span data-ttu-id="3f042-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3f042-117">Read-only.</span></span> <span data-ttu-id="3f042-118">ID de usuário pela qual esta foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="3f042-118">User ID by which this is last modified.</span></span>|
|<span data-ttu-id="3f042-119">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3f042-119">lastModifiedDateTime</span></span>|<span data-ttu-id="3f042-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f042-120">DateTimeOffset</span></span>|<span data-ttu-id="3f042-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3f042-121">Read-only.</span></span> <span data-ttu-id="3f042-122">Data e hora da última modificação.</span><span class="sxs-lookup"><span data-stu-id="3f042-122">Date and time at which this is last modified.</span></span> <span data-ttu-id="3f042-123">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="3f042-123">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3f042-124">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="3f042-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="3f042-125">previewPriority</span><span class="sxs-lookup"><span data-stu-id="3f042-125">previewPriority</span></span>|<span data-ttu-id="3f042-126">String</span><span class="sxs-lookup"><span data-stu-id="3f042-126">String</span></span>|<span data-ttu-id="3f042-127">Usado para definir a ordem de prioridade relativa na qual a referência será mostrada como uma visualização na tarefa.</span><span class="sxs-lookup"><span data-stu-id="3f042-127">Used to set the relative priority order in which the reference will be shown as a preview on the task.</span></span>|
|<span data-ttu-id="3f042-128">tipo</span><span class="sxs-lookup"><span data-stu-id="3f042-128">type</span></span>|<span data-ttu-id="3f042-129">String</span><span class="sxs-lookup"><span data-stu-id="3f042-129">String</span></span>|<span data-ttu-id="3f042-130">Usado para descrever o tipo da referência.</span><span class="sxs-lookup"><span data-stu-id="3f042-130">Used to describe the type of the reference.</span></span> <span data-ttu-id="3f042-131">Os tipos incluem: `PowerPoint` , `Word` , `Excel` , `Other` .</span><span class="sxs-lookup"><span data-stu-id="3f042-131">Types include: `PowerPoint`, `Word`, `Excel`, `Other`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3f042-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3f042-132">JSON representation</span></span>
<span data-ttu-id="3f042-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3f042-133">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerExternalReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


