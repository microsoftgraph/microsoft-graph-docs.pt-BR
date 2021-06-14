---
title: tipo de recurso educationAssignmentIndividualRecipient
description: Usado dentro da propriedade assignment.assignTo.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 147697685f58723d940102333abd9ffc378bee28
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912185"
---
# <a name="educationassignmentindividualrecipient-resource-type"></a><span data-ttu-id="0f6f6-103">tipo de recurso educationAssignmentIndividualRecipient</span><span class="sxs-lookup"><span data-stu-id="0f6f6-103">educationAssignmentIndividualRecipient resource type</span></span>

<span data-ttu-id="0f6f6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f6f6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0f6f6-105">Usado dentro da [propriedade assignment.assignTo.](educationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="0f6f6-105">Used inside the [assignment.assignTo](educationassignment.md) property.</span></span> <span data-ttu-id="0f6f6-106">Quando definido como lista de destinatários individuais, os alunos selecionados na classe receberão um objeto de envio quando a atribuição for publicada.</span><span class="sxs-lookup"><span data-stu-id="0f6f6-106">When set to individual recipient list, selected students in the class will receive a submission object when the assignment is published.</span></span>

<span data-ttu-id="0f6f6-107">Esse recurso é uma subclasse [de educationAssignmentRecipient](educationassignmentrecipient.md).</span><span class="sxs-lookup"><span data-stu-id="0f6f6-107">This resource is a subclass of [educationAssignmentRecipient](educationassignmentrecipient.md).</span></span>

## <a name="properties"></a><span data-ttu-id="0f6f6-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0f6f6-108">Properties</span></span>
| <span data-ttu-id="0f6f6-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0f6f6-109">Property</span></span>     | <span data-ttu-id="0f6f6-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="0f6f6-110">Type</span></span>   |<span data-ttu-id="0f6f6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f6f6-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0f6f6-112">destinatários</span><span class="sxs-lookup"><span data-stu-id="0f6f6-112">recipients</span></span>|<span data-ttu-id="0f6f6-113">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f6f6-113">String collection</span></span>|<span data-ttu-id="0f6f6-114">Uma coleção de IDs dos destinatários.</span><span class="sxs-lookup"><span data-stu-id="0f6f6-114">A collection of IDs of the recipients.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0f6f6-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0f6f6-115">JSON representation</span></span>

<span data-ttu-id="0f6f6-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0f6f6-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentIndividualRecipient"
}-->

```json
{
  "recipients": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentIndividualRecipient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


