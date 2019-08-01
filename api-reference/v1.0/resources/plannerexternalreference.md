---
title: tipo de recurso plannerExternalReference
description: O recurso **plannerExternalReference** representa os metadados de uma referência (anexos como arquivo, URL). É o valor dos pares propriedade-valor no objeto externalReferences.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: d13af293defb09630f23c3be193020eed053ca21
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035263"
---
# <a name="plannerexternalreference-resource-type"></a><span data-ttu-id="eb3ea-104">tipo de recurso plannerExternalReference</span><span class="sxs-lookup"><span data-stu-id="eb3ea-104">plannerExternalReference resource type</span></span>

<span data-ttu-id="eb3ea-105">O recurso **plannerExternalReference** representa os metadados de uma referência (anexos como arquivo, URL).</span><span class="sxs-lookup"><span data-stu-id="eb3ea-105">The **plannerExternalReference** resource represents the metadata of a reference (attachments such as file, URL).</span></span> <span data-ttu-id="eb3ea-106">É o valor dos pares propriedade-valor no [objeto externalReferences](plannerexternalreferences.md).</span><span class="sxs-lookup"><span data-stu-id="eb3ea-106">It is the value of property-value pairs in the [externalReferences object](plannerexternalreferences.md).</span></span>



## <a name="properties"></a><span data-ttu-id="eb3ea-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eb3ea-107">Properties</span></span>
| <span data-ttu-id="eb3ea-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eb3ea-108">Property</span></span>     | <span data-ttu-id="eb3ea-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="eb3ea-109">Type</span></span>   |<span data-ttu-id="eb3ea-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb3ea-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eb3ea-111">alias</span><span class="sxs-lookup"><span data-stu-id="eb3ea-111">alias</span></span>|<span data-ttu-id="eb3ea-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eb3ea-112">String</span></span>|<span data-ttu-id="eb3ea-113">Um alias de nome para descrever a referência.</span><span class="sxs-lookup"><span data-stu-id="eb3ea-113">A name alias to describe the reference.</span></span>|
|<span data-ttu-id="eb3ea-114">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="eb3ea-114">lastModifiedBy</span></span>|[<span data-ttu-id="eb3ea-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="eb3ea-115">identitySet</span></span>](identityset.md)|<span data-ttu-id="eb3ea-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="eb3ea-116">Read-only.</span></span> <span data-ttu-id="eb3ea-117">ID de usuário pela qual esta foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="eb3ea-117">User ID by which this is last modified.</span></span>|
|<span data-ttu-id="eb3ea-118">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="eb3ea-118">lastModifiedDateTime</span></span>|<span data-ttu-id="eb3ea-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb3ea-119">DateTimeOffset</span></span>|<span data-ttu-id="eb3ea-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="eb3ea-120">Read-only.</span></span> <span data-ttu-id="eb3ea-121">Data e hora da última modificação.</span><span class="sxs-lookup"><span data-stu-id="eb3ea-121">Date and time at which this is last modified.</span></span> <span data-ttu-id="eb3ea-122">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="eb3ea-122">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="eb3ea-123">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="eb3ea-123">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="eb3ea-124">previewPriority</span><span class="sxs-lookup"><span data-stu-id="eb3ea-124">previewPriority</span></span>|<span data-ttu-id="eb3ea-125">String</span><span class="sxs-lookup"><span data-stu-id="eb3ea-125">String</span></span>|<span data-ttu-id="eb3ea-126">Usado para definir a ordem de prioridade relativa na qual a referência será mostrada como uma visualização na tarefa.</span><span class="sxs-lookup"><span data-stu-id="eb3ea-126">Used to set the relative priority order in which the reference will be shown as a preview on the task.</span></span>|
|<span data-ttu-id="eb3ea-127">type</span><span class="sxs-lookup"><span data-stu-id="eb3ea-127">type</span></span>|<span data-ttu-id="eb3ea-128">String</span><span class="sxs-lookup"><span data-stu-id="eb3ea-128">String</span></span>|<span data-ttu-id="eb3ea-129">Usado para descrever o tipo da referência.</span><span class="sxs-lookup"><span data-stu-id="eb3ea-129">Used to describe the type of the reference.</span></span> <span data-ttu-id="eb3ea-130">Os tipos incluem `PowerPoint`: `Word`, `Excel`, `Other`,.</span><span class="sxs-lookup"><span data-stu-id="eb3ea-130">Types include: `PowerPoint`, `Word`, `Excel`, `Other`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="eb3ea-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eb3ea-131">JSON representation</span></span>
<span data-ttu-id="eb3ea-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eb3ea-132">Here is a JSON representation of the resource.</span></span>

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
