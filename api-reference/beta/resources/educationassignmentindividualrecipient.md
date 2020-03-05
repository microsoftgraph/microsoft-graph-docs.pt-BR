---
title: tipo de recurso educationAssignmentIndividualRecipient
description: 'Usada dentro da propriedade assignment. assignTo. Quando definido como lista de destinatários individuais, os alunos selecionados na classe serão '
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b5bccdf98bbba4c0965daf5d5aba93cf1a34b758
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42502547"
---
# <a name="educationassignmentindividualrecipient-resource-type"></a><span data-ttu-id="81faa-104">tipo de recurso educationAssignmentIndividualRecipient</span><span class="sxs-lookup"><span data-stu-id="81faa-104">educationAssignmentIndividualRecipient resource type</span></span>

<span data-ttu-id="81faa-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="81faa-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81faa-106">Usada dentro da propriedade [assignment. assignTo](educationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="81faa-106">Used inside the [assignment.assignTo](educationassignment.md) property.</span></span> <span data-ttu-id="81faa-107">Quando definido como lista de destinatários individuais, os alunos selecionados na classe receberão um objeto de envio quando a atribuição for publicada.</span><span class="sxs-lookup"><span data-stu-id="81faa-107">When set to individual recipient list, selected students in the class will receive a submission object when the assignment is published.</span></span>

<span data-ttu-id="81faa-108">Esse recurso é uma subclasse de [educationAssignmentRecipient](educationassignmentrecipient.md).</span><span class="sxs-lookup"><span data-stu-id="81faa-108">This resource is a subclass of [educationAssignmentRecipient](educationassignmentrecipient.md).</span></span>

## <a name="properties"></a><span data-ttu-id="81faa-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="81faa-109">Properties</span></span>
| <span data-ttu-id="81faa-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="81faa-110">Property</span></span>     | <span data-ttu-id="81faa-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="81faa-111">Type</span></span>   |<span data-ttu-id="81faa-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="81faa-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="81faa-113">destinatários</span><span class="sxs-lookup"><span data-stu-id="81faa-113">recipients</span></span>|<span data-ttu-id="81faa-114">String collection</span><span class="sxs-lookup"><span data-stu-id="81faa-114">String collection</span></span>|<span data-ttu-id="81faa-115">Uma coleção de IDs dos destinatários.</span><span class="sxs-lookup"><span data-stu-id="81faa-115">A collection of ids of the recipients.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="81faa-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="81faa-116">JSON representation</span></span>

<span data-ttu-id="81faa-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="81faa-117">The following is a JSON representation of the resource.</span></span>

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
