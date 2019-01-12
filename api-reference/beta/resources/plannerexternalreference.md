---
title: Tipo de recurso plannerExternalReference
description: O recurso de **plannerExternalReference** representa os metadados de uma referência (anexos como arquivo, URL). É o valor de pares de valor da propriedade no objeto externalReferences.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: d484c22d18ffb501cccbd731fa5c3ad4788a8667
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27944660"
---
# <a name="plannerexternalreference-resource-type"></a><span data-ttu-id="09b99-104">Tipo de recurso plannerExternalReference</span><span class="sxs-lookup"><span data-stu-id="09b99-104">plannerExternalReference resource type</span></span>

> <span data-ttu-id="09b99-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="09b99-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="09b99-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="09b99-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="09b99-p103">O recurso **plannerExternalReference** representa os metadados de uma referência (anexos como arquivo, URL). É o valor de pares propriedade-valor no [objeto externalReferences](plannerexternalreferences.md).</span><span class="sxs-lookup"><span data-stu-id="09b99-p103">The **plannerExternalReference** resource represents the metadata of a reference (attachments such as file, URL). It is the value of property-value pairs in the [externalReferences object](plannerexternalreferences.md).</span></span>



## <a name="properties"></a><span data-ttu-id="09b99-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="09b99-109">Properties</span></span>
| <span data-ttu-id="09b99-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="09b99-110">Property</span></span>     | <span data-ttu-id="09b99-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="09b99-111">Type</span></span>   |<span data-ttu-id="09b99-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="09b99-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="09b99-113">alias</span><span class="sxs-lookup"><span data-stu-id="09b99-113">alias</span></span>|<span data-ttu-id="09b99-114">String</span><span class="sxs-lookup"><span data-stu-id="09b99-114">String</span></span>|<span data-ttu-id="09b99-115">Um alias de nome para descrever a referência.</span><span class="sxs-lookup"><span data-stu-id="09b99-115">A name alias to describe the reference.</span></span>|
|<span data-ttu-id="09b99-116">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="09b99-116">lastModifiedBy</span></span>|[<span data-ttu-id="09b99-117">identitySet</span><span class="sxs-lookup"><span data-stu-id="09b99-117">identitySet</span></span>](identityset.md)|<span data-ttu-id="09b99-p104">Somente leitura. A identificação de usuário pela qual isso foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="09b99-p104">Read-only. User ID by which this is last modified.</span></span>|
|<span data-ttu-id="09b99-120">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="09b99-120">lastModifiedDateTime</span></span>|<span data-ttu-id="09b99-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09b99-121">DateTimeOffset</span></span>|<span data-ttu-id="09b99-p105">Somente leitura. A data e a hora pelas quais isso foi modificado pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="09b99-p105">Read-only. Date and time at which this is last modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="09b99-126">previewPriority</span><span class="sxs-lookup"><span data-stu-id="09b99-126">previewPriority</span></span>|<span data-ttu-id="09b99-127">String</span><span class="sxs-lookup"><span data-stu-id="09b99-127">String</span></span>|<span data-ttu-id="09b99-128">Usado para definir a ordem de prioridade relativa na qual a referência será mostrada como uma visualização na tarefa.</span><span class="sxs-lookup"><span data-stu-id="09b99-128">Used to set the relative priority order in which the reference will be shown as a preview on the task.</span></span>|
|<span data-ttu-id="09b99-129">type</span><span class="sxs-lookup"><span data-stu-id="09b99-129">type</span></span>|<span data-ttu-id="09b99-130">String</span><span class="sxs-lookup"><span data-stu-id="09b99-130">String</span></span>|<span data-ttu-id="09b99-p106">Usado para descrever o tipo da referência. Os tipos incluem: `PowerPoint`, `Word`, `Excel`, `Other`.</span><span class="sxs-lookup"><span data-stu-id="09b99-p106">Used to describe the type of the reference. Types include: `PowerPoint`, `Word`, `Excel`, `Other`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="09b99-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="09b99-133">JSON representation</span></span>
<span data-ttu-id="09b99-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="09b99-134">Here is a JSON representation of the resource.</span></span>

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
