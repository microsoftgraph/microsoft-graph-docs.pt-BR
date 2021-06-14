---
title: Tipo de recurso educationAssignmentGrade
description: Representa o objeto Grade em um Envio.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ea25bb723249878637d98d91d8c91e14891f8465
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912123"
---
# <a name="educationassignmentgrade-resource-type"></a><span data-ttu-id="668b0-103">Tipo de recurso educationAssignmentGrade</span><span class="sxs-lookup"><span data-stu-id="668b0-103">educationAssignmentGrade resource type</span></span>

<span data-ttu-id="668b0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="668b0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="668b0-105">Representa o **objeto Grade** em um Envio.</span><span class="sxs-lookup"><span data-stu-id="668b0-105">Represents the **Grade** object on a Submission.</span></span> 

<span data-ttu-id="668b0-106">Esse é um tipo abstrato que nunca será instaurou; no entanto, todos os tipos de classificação (pontos, passagem/falha e assim por diante) são subclasses desse tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="668b0-106">This is an abstract type that will never be instantiated; however, all types of grading (points, pass/fail, and so on) are subclasses of this resource type.</span></span> <span data-ttu-id="668b0-107">Esse objeto também rastreia quem está fazendo a classificação.</span><span class="sxs-lookup"><span data-stu-id="668b0-107">This object also tracks who is doing the grading.</span></span> <span data-ttu-id="668b0-108">Isso é usado na **propriedade submission.grade.**</span><span class="sxs-lookup"><span data-stu-id="668b0-108">This is used in the **submission.grade** property.</span></span>


## <a name="properties"></a><span data-ttu-id="668b0-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="668b0-109">Properties</span></span>
| <span data-ttu-id="668b0-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="668b0-110">Property</span></span>     | <span data-ttu-id="668b0-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="668b0-111">Type</span></span>   |<span data-ttu-id="668b0-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="668b0-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="668b0-113">gradedBy</span><span class="sxs-lookup"><span data-stu-id="668b0-113">gradedBy</span></span>|[<span data-ttu-id="668b0-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="668b0-114">identitySet</span></span>](identityset.md)| <span data-ttu-id="668b0-115">Usuário que fez a classificação.</span><span class="sxs-lookup"><span data-stu-id="668b0-115">User who did the grading.</span></span> |
|<span data-ttu-id="668b0-116">gradedDateTime</span><span class="sxs-lookup"><span data-stu-id="668b0-116">gradedDateTime</span></span>|<span data-ttu-id="668b0-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="668b0-117">DateTimeOffset</span></span>| <span data-ttu-id="668b0-118">Momento no tempo em que a nota foi aplicada a esse objeto de envio.</span><span class="sxs-lookup"><span data-stu-id="668b0-118">Moment in time when the grade was applied to this submission object.</span></span> <span data-ttu-id="668b0-119">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="668b0-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="668b0-120">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="668b0-120">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="668b0-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="668b0-121">JSON representation</span></span>

<span data-ttu-id="668b0-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="668b0-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentGrade"
}-->

```json
{
  "gradedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "gradedDateTime": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentGrade resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


