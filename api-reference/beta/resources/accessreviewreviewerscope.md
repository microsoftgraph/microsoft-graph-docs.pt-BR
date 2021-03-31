---
title: Tipo de recurso accessReviewReviewerScope
description: Representa quem revisará uma revisão de acesso.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 68f353b81b6a14292828d82929a0eeac81d67bc5
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469154"
---
# <a name="accessreviewreviewerscope-resource-type"></a><span data-ttu-id="39706-103">Tipo de recurso accessReviewReviewerScope</span><span class="sxs-lookup"><span data-stu-id="39706-103">accessReviewReviewerScope resource type</span></span>

<span data-ttu-id="39706-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39706-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="39706-105">O accessReviewReviewerScope define quem revisará instâncias de [um accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="39706-105">The accessReviewReviewerScope defines who will review instances of an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="39706-106">Isso é expresso como uma consulta OData, que permite que os revisadores sejam especificados como uma lista estática de usuários (ou seja, usuários específicos, proprietários de grupo, membros do grupo) ou dinamicamente (ou seja, o caso em que cada usuário é revisado por seu gerente).</span><span class="sxs-lookup"><span data-stu-id="39706-106">This is expressed as an OData query, which allows reviewers to be specified both as a static list of users (i.e., specific users, group owners, group members) or dynamically (i.e., the case where every user is reviewed by their manager).</span></span> <span data-ttu-id="39706-107">Para criar uma auto-revisão (onde os usuários analisam seu próprio acesso), não forneça aos revisores sobre a criação [accessReviewScheduleDefinition.](accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="39706-107">To create a self-review (where users review their own access), do not provide reviewers on [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) creation.</span></span>

<span data-ttu-id="39706-108">Herda de [accessReviewScope](../resources/accessreviewscope.md).</span><span class="sxs-lookup"><span data-stu-id="39706-108">Inherits from [accessReviewScope](../resources/accessreviewscope.md).</span></span>

## <a name="properties"></a><span data-ttu-id="39706-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="39706-109">Properties</span></span>
| <span data-ttu-id="39706-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="39706-110">Property</span></span> | <span data-ttu-id="39706-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="39706-111">Type</span></span> | <span data-ttu-id="39706-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="39706-112">Description</span></span> |
| :-------------------------| :---------- | :---------- |
| <span data-ttu-id="39706-113">consulta</span><span class="sxs-lookup"><span data-stu-id="39706-113">query</span></span> | <span data-ttu-id="39706-114">String</span><span class="sxs-lookup"><span data-stu-id="39706-114">String</span></span> | <span data-ttu-id="39706-115">A consulta especificando quem será o revistor.</span><span class="sxs-lookup"><span data-stu-id="39706-115">The query specifying who will be the reviewer.</span></span> <span data-ttu-id="39706-116">Consulte tabela para exemplos.</span><span class="sxs-lookup"><span data-stu-id="39706-116">See table for examples.</span></span> |
| <span data-ttu-id="39706-117">queryType</span><span class="sxs-lookup"><span data-stu-id="39706-117">queryType</span></span> | <span data-ttu-id="39706-118">String</span><span class="sxs-lookup"><span data-stu-id="39706-118">String</span></span> | <span data-ttu-id="39706-119">O tipo de consulta.</span><span class="sxs-lookup"><span data-stu-id="39706-119">The type of query.</span></span> <span data-ttu-id="39706-120">Exemplos incluem `MicrosoftGraph` `ARM` e .</span><span class="sxs-lookup"><span data-stu-id="39706-120">Examples include `MicrosoftGraph` and `ARM`.</span></span> |
| <span data-ttu-id="39706-121">queryRoot</span><span class="sxs-lookup"><span data-stu-id="39706-121">queryRoot</span></span> | <span data-ttu-id="39706-122">String</span><span class="sxs-lookup"><span data-stu-id="39706-122">String</span></span> | <span data-ttu-id="39706-123">No cenário em que os revisadores precisam ser especificados dinamicamente, essa propriedade é usada para indicar a fonte relativa da consulta.</span><span class="sxs-lookup"><span data-stu-id="39706-123">In the scenario where reviewers need to be specified dynamically, this property is used to indicate the relative source of the query.</span></span> <span data-ttu-id="39706-124">Essa propriedade só será necessária se uma consulta relativa (ou seja, ./manager) for especificada.</span><span class="sxs-lookup"><span data-stu-id="39706-124">This property is only required if a relative query (i.e., ./manager) is specified.</span></span> |

### <a name="supported-queries-for-accessreviewreviewerscope"></a><span data-ttu-id="39706-125">Consultas com suporte para accessReviewReviewerScope</span><span class="sxs-lookup"><span data-stu-id="39706-125">Supported queries for accessReviewReviewerScope</span></span>

|<span data-ttu-id="39706-126">Cenário</span><span class="sxs-lookup"><span data-stu-id="39706-126">Scenario</span></span>| <span data-ttu-id="39706-127">consulta</span><span class="sxs-lookup"><span data-stu-id="39706-127">query</span></span> | <span data-ttu-id="39706-128">queryType</span><span class="sxs-lookup"><span data-stu-id="39706-128">queryType</span></span> | <span data-ttu-id="39706-129">queryRoot</span><span class="sxs-lookup"><span data-stu-id="39706-129">queryRoot</span></span> |
|--|--|--|--|
| <span data-ttu-id="39706-130">Proprietário do grupo como revistor</span><span class="sxs-lookup"><span data-stu-id="39706-130">Group owner as reviewer</span></span> | <span data-ttu-id="39706-131">/groups/{group id}/owners</span><span class="sxs-lookup"><span data-stu-id="39706-131">/groups/{group id}/owners</span></span> |<span data-ttu-id="39706-132">MicrosoftGraph</span><span class="sxs-lookup"><span data-stu-id="39706-132">MicrosoftGraph</span></span>||
| <span data-ttu-id="39706-133">Usuário específico como revistor</span><span class="sxs-lookup"><span data-stu-id="39706-133">Specific user as reviewer</span></span> | <span data-ttu-id="39706-134">/users/{user id}</span><span class="sxs-lookup"><span data-stu-id="39706-134">/users/{user id}</span></span> |<span data-ttu-id="39706-135">MicrosoftGraph</span><span class="sxs-lookup"><span data-stu-id="39706-135">MicrosoftGraph</span></span>||
| <span data-ttu-id="39706-136">Gerente do usuário que está sendo revisado como revistor</span><span class="sxs-lookup"><span data-stu-id="39706-136">Manager of user being reviewed as reviewer</span></span> | <span data-ttu-id="39706-137">./manager</span><span class="sxs-lookup"><span data-stu-id="39706-137">./manager</span></span> | <span data-ttu-id="39706-138">MicrosoftGraph</span><span class="sxs-lookup"><span data-stu-id="39706-138">MicrosoftGraph</span></span> |<span data-ttu-id="39706-139">decisions</span><span class="sxs-lookup"><span data-stu-id="39706-139">decisions</span></span>|
| <span data-ttu-id="39706-140">Autoavaliação</span><span class="sxs-lookup"><span data-stu-id="39706-140">Self Review</span></span> | <span data-ttu-id="39706-141">Lista vazia(Sem revistores)</span><span class="sxs-lookup"><span data-stu-id="39706-141">Empty list(No reviewers)</span></span> | <span data-ttu-id="39706-142">MicrosoftGraph</span><span class="sxs-lookup"><span data-stu-id="39706-142">MicrosoftGraph</span></span>  |


## <a name="relationships"></a><span data-ttu-id="39706-143">Relações</span><span class="sxs-lookup"><span data-stu-id="39706-143">Relationships</span></span>
<span data-ttu-id="39706-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="39706-144">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="39706-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="39706-145">JSON representation</span></span>
<span data-ttu-id="39706-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="39706-146">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewReviewerScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewReviewerScope",
  "query": "String",
  "queryType": "String",
  "queryRoot": "String"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewReviewerScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
