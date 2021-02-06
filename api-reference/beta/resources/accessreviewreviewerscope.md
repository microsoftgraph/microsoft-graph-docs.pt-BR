---
title: Tipo de recurso accessReviewReviewerScope
description: Representa quem revisará uma revisão de acesso.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7c8a0644699daf7e204226d89bdd6cab6048888d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133487"
---
# <a name="accessreviewreviewerscope-resource-type"></a><span data-ttu-id="d8b4b-103">Tipo de recurso accessReviewReviewerScope</span><span class="sxs-lookup"><span data-stu-id="d8b4b-103">accessReviewReviewerScope resource type</span></span>

<span data-ttu-id="d8b4b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8b4b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8b4b-105">O accessReviewReviewerScope define quem revisará instâncias de um [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="d8b4b-105">The accessReviewReviewerScope defines who will review instances of an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="d8b4b-106">Isso é expresso como uma consulta OData, que permite que os revisadores sejam especificados como uma lista estática de usuários (ou seja, usuários específicos, proprietários de grupos, membros do grupo) ou dinamicamente (ou seja, o caso em que cada usuário é revisado por seu gerente).</span><span class="sxs-lookup"><span data-stu-id="d8b4b-106">This is expressed as an OData query, which allows reviewers to be specified both as a static list of users (i.e., specific users, group owners, group members) or dynamically (i.e., the case where every user is reviewed by their manager).</span></span> <span data-ttu-id="d8b4b-107">Para criar uma auto-revisão (onde os usuários revisam seu próprio acesso), não forneça aos revisores sobre a criação [de accessReviewScheduleDefinition.](accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d8b4b-107">To create a self-review (where users review their own access), do not provide reviewers on [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) creation.</span></span>


## <a name="properties"></a><span data-ttu-id="d8b4b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d8b4b-108">Properties</span></span>
| <span data-ttu-id="d8b4b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d8b4b-109">Property</span></span> | <span data-ttu-id="d8b4b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8b4b-110">Type</span></span> | <span data-ttu-id="d8b4b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8b4b-111">Description</span></span> |
| :-------------------------| :---------- | :---------- |
| <span data-ttu-id="d8b4b-112">consulta</span><span class="sxs-lookup"><span data-stu-id="d8b4b-112">query</span></span> | <span data-ttu-id="d8b4b-113">String</span><span class="sxs-lookup"><span data-stu-id="d8b4b-113">String</span></span> | <span data-ttu-id="d8b4b-114">A consulta especificando quem será o revistor.</span><span class="sxs-lookup"><span data-stu-id="d8b4b-114">The query specifying who will be the reviewer.</span></span> <span data-ttu-id="d8b4b-115">Consulte a tabela para ver exemplos.</span><span class="sxs-lookup"><span data-stu-id="d8b4b-115">See table for examples.</span></span> |
| <span data-ttu-id="d8b4b-116">queryType</span><span class="sxs-lookup"><span data-stu-id="d8b4b-116">queryType</span></span> | <span data-ttu-id="d8b4b-117">String</span><span class="sxs-lookup"><span data-stu-id="d8b4b-117">String</span></span> | <span data-ttu-id="d8b4b-118">O tipo de consulta.</span><span class="sxs-lookup"><span data-stu-id="d8b4b-118">The type of query.</span></span> <span data-ttu-id="d8b4b-119">Exemplos incluem `MicrosoftGraph` e `ARM` .</span><span class="sxs-lookup"><span data-stu-id="d8b4b-119">Examples include `MicrosoftGraph` and `ARM`.</span></span> |
| <span data-ttu-id="d8b4b-120">queryRoot</span><span class="sxs-lookup"><span data-stu-id="d8b4b-120">queryRoot</span></span> | <span data-ttu-id="d8b4b-121">String</span><span class="sxs-lookup"><span data-stu-id="d8b4b-121">String</span></span> | <span data-ttu-id="d8b4b-122">No cenário em que os revisadores precisam ser especificados dinamicamente, essa propriedade é usada para indicar a fonte relativa da consulta.</span><span class="sxs-lookup"><span data-stu-id="d8b4b-122">In the scenario where reviewers need to be specified dynamically, this property is used to indicate the relative source of the query.</span></span> <span data-ttu-id="d8b4b-123">Essa propriedade só será necessária se uma consulta relativa (ou seja, ./manager) for especificada.</span><span class="sxs-lookup"><span data-stu-id="d8b4b-123">This property is only required if a relative query (i.e., ./manager) is specified.</span></span> |

### <a name="supported-queries-for-accessreviewreviewerscope"></a><span data-ttu-id="d8b4b-124">Consultas com suporte para accessReviewReviewerScope</span><span class="sxs-lookup"><span data-stu-id="d8b4b-124">Supported queries for accessReviewReviewerScope</span></span>

|<span data-ttu-id="d8b4b-125">Cenário</span><span class="sxs-lookup"><span data-stu-id="d8b4b-125">Scenario</span></span>| <span data-ttu-id="d8b4b-126">consulta</span><span class="sxs-lookup"><span data-stu-id="d8b4b-126">query</span></span> | <span data-ttu-id="d8b4b-127">queryType</span><span class="sxs-lookup"><span data-stu-id="d8b4b-127">queryType</span></span> | <span data-ttu-id="d8b4b-128">queryRoot</span><span class="sxs-lookup"><span data-stu-id="d8b4b-128">queryRoot</span></span> |
|--|--|--|--|
| <span data-ttu-id="d8b4b-129">Proprietário do grupo como revistor</span><span class="sxs-lookup"><span data-stu-id="d8b4b-129">Group owner as reviewer</span></span> | <span data-ttu-id="d8b4b-130">/groups/{group id}/owners</span><span class="sxs-lookup"><span data-stu-id="d8b4b-130">/groups/{group id}/owners</span></span> |<span data-ttu-id="d8b4b-131">MicrosoftGraph</span><span class="sxs-lookup"><span data-stu-id="d8b4b-131">MicrosoftGraph</span></span>||
| <span data-ttu-id="d8b4b-132">Usuário específico como revistor</span><span class="sxs-lookup"><span data-stu-id="d8b4b-132">Specific user as reviewer</span></span> | <span data-ttu-id="d8b4b-133">/users/{user id}</span><span class="sxs-lookup"><span data-stu-id="d8b4b-133">/users/{user id}</span></span> |<span data-ttu-id="d8b4b-134">MicrosoftGraph</span><span class="sxs-lookup"><span data-stu-id="d8b4b-134">MicrosoftGraph</span></span>||
| <span data-ttu-id="d8b4b-135">Gerente do usuário que está sendo revisado como revistor</span><span class="sxs-lookup"><span data-stu-id="d8b4b-135">Manager of user being reviewed as reviewer</span></span> | <span data-ttu-id="d8b4b-136">./manager</span><span class="sxs-lookup"><span data-stu-id="d8b4b-136">./manager</span></span> | <span data-ttu-id="d8b4b-137">MicrosoftGraph</span><span class="sxs-lookup"><span data-stu-id="d8b4b-137">MicrosoftGraph</span></span> |<span data-ttu-id="d8b4b-138">decisões</span><span class="sxs-lookup"><span data-stu-id="d8b4b-138">decisions</span></span>|

## <a name="relationships"></a><span data-ttu-id="d8b4b-139">Relações</span><span class="sxs-lookup"><span data-stu-id="d8b4b-139">Relationships</span></span>
<span data-ttu-id="d8b4b-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d8b4b-140">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d8b4b-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d8b4b-141">JSON representation</span></span>
<span data-ttu-id="d8b4b-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d8b4b-142">The following is a JSON representation of the resource.</span></span>
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
