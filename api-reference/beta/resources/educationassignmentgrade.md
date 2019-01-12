---
title: tipo de recurso de educationAssignmentGrade
description: " No entanto, todos os tipos de classificação (pontos, aprovação/reprovação e assim por diante) são subclasses isso"
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: ecdd92c84399ee17d2808301d997830725fb5642
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982355"
---
# <a name="educationassignmentgrade-resource-type"></a><span data-ttu-id="4d11c-103">tipo de recurso de educationAssignmentGrade</span><span class="sxs-lookup"><span data-stu-id="4d11c-103">educationAssignmentGrade resource type</span></span>

> <span data-ttu-id="4d11c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4d11c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4d11c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4d11c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4d11c-106">Representa o objeto de **nível** em um envio.</span><span class="sxs-lookup"><span data-stu-id="4d11c-106">Represents the **Grade** object on a Submission.</span></span> <span data-ttu-id="4d11c-107">Este é um tipo abstrato que nunca será instanciado; No entanto, todos os tipos de classificação (pontos, aprovação/reprovação e assim por diante) são subclasses desse tipo de recurso.</span><span class="sxs-lookup"><span data-stu-id="4d11c-107">This is an abstract type that will never be instantiated; however, all types of grading (points, pass/fail, and so on) are subclasses of this resource type.</span></span> <span data-ttu-id="4d11c-108">Este objeto também controla quem está fazendo a classificação.</span><span class="sxs-lookup"><span data-stu-id="4d11c-108">This object also tracks who is doing the grading.</span></span> <span data-ttu-id="4d11c-109">Isso é usado na propriedade **submission.grade** .</span><span class="sxs-lookup"><span data-stu-id="4d11c-109">This is used in the **submission.grade** property.</span></span>


## <a name="properties"></a><span data-ttu-id="4d11c-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4d11c-110">Properties</span></span>
| <span data-ttu-id="4d11c-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4d11c-111">Property</span></span>     | <span data-ttu-id="4d11c-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="4d11c-112">Type</span></span>   |<span data-ttu-id="4d11c-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d11c-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4d11c-114">gradedBy</span><span class="sxs-lookup"><span data-stu-id="4d11c-114">gradedBy</span></span>|[<span data-ttu-id="4d11c-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="4d11c-115">identitySet</span></span>](identityset.md)| <span data-ttu-id="4d11c-116">Usuário que fez a classificação.</span><span class="sxs-lookup"><span data-stu-id="4d11c-116">User who did the grading.</span></span> |
|<span data-ttu-id="4d11c-117">gradedDateTime</span><span class="sxs-lookup"><span data-stu-id="4d11c-117">gradedDateTime</span></span>|<span data-ttu-id="4d11c-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d11c-118">DateTimeOffset</span></span>| <span data-ttu-id="4d11c-119">Momento específico quando o nível foi aplicada a este objeto de envio.</span><span class="sxs-lookup"><span data-stu-id="4d11c-119">Moment in time when the grade was applied to this submission object.</span></span> <span data-ttu-id="4d11c-120">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="4d11c-120">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4d11c-121">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="4d11c-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4d11c-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4d11c-122">JSON representation</span></span>

<span data-ttu-id="4d11c-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4d11c-123">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationAssignmentGrade resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
