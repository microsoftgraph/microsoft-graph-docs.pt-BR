---
title: tipo de recurso accessReviewReviewerScope
description: Representa quem irá revisar uma revisão do Access.
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: edc25e19a51f787dd0799fbd9e6e6c2a1b45787e
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000775"
---
# <a name="accessreviewreviewerscope-resource-type"></a><span data-ttu-id="da175-103">tipo de recurso accessReviewReviewerScope</span><span class="sxs-lookup"><span data-stu-id="da175-103">accessReviewReviewerScope resource type</span></span>

<span data-ttu-id="da175-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da175-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da175-105">O accessReviewReviewerScope define quem irá revisar instâncias de um [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="da175-105">The accessReviewReviewerScope defines who will review instances of an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="da175-106">Isso é expresso como uma consulta OData, que permite que os revisores sejam especificados como uma lista estática de usuários (ou seja, usuários específicos, proprietários de grupo, membros do grupo) ou dinamicamente (ou seja, o caso em que cada usuário é revisado por seu gerente).</span><span class="sxs-lookup"><span data-stu-id="da175-106">This is expressed as an OData query, which allows reviewers to be specified both as a static list of users (i.e., specific users, group owners, group members) or dynamically (i.e., the case where every user is reviewed by their manager).</span></span> <span data-ttu-id="da175-107">Para criar uma autoanálise (onde os usuários revisam seu próprio acesso), não forneça revisores na criação do [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="da175-107">To create a self-review (where users review their own access), do not provide reviewers on [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) creation.</span></span>


## <a name="properties"></a><span data-ttu-id="da175-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="da175-108">Properties</span></span>
| <span data-ttu-id="da175-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="da175-109">Property</span></span> | <span data-ttu-id="da175-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="da175-110">Type</span></span> | <span data-ttu-id="da175-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="da175-111">Description</span></span> |
| :-------------------------| :---------- | :---------- |
| <span data-ttu-id="da175-112">consulta</span><span class="sxs-lookup"><span data-stu-id="da175-112">query</span></span> | <span data-ttu-id="da175-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="da175-113">String</span></span> | <span data-ttu-id="da175-114">A consulta especificando quem será o revisor.</span><span class="sxs-lookup"><span data-stu-id="da175-114">The query specifying who will be the reviewer.</span></span> <span data-ttu-id="da175-115">Consulte a tabela para obter exemplos.</span><span class="sxs-lookup"><span data-stu-id="da175-115">See table for examples.</span></span> |
| <span data-ttu-id="da175-116">queryType</span><span class="sxs-lookup"><span data-stu-id="da175-116">queryType</span></span> | <span data-ttu-id="da175-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="da175-117">String</span></span> | <span data-ttu-id="da175-118">O tipo de consulta.</span><span class="sxs-lookup"><span data-stu-id="da175-118">The type of query.</span></span> <span data-ttu-id="da175-119">Os exemplos incluem `MicrosoftGraph` e `ARM` .</span><span class="sxs-lookup"><span data-stu-id="da175-119">Examples include `MicrosoftGraph` and `ARM`.</span></span> |
| <span data-ttu-id="da175-120">queryRoot</span><span class="sxs-lookup"><span data-stu-id="da175-120">queryRoot</span></span> | <span data-ttu-id="da175-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="da175-121">String</span></span> | <span data-ttu-id="da175-122">No cenário em que os revisores precisam ser especificados dinamicamente, essa propriedade é usada para indicar a fonte relativa da consulta.</span><span class="sxs-lookup"><span data-stu-id="da175-122">In the scenario where reviewers need to be specified dynamically, this property is used to indicate the relative source of the query.</span></span> <span data-ttu-id="da175-123">Essa propriedade só será necessária se uma consulta relativa (ou seja,./Manager) for especificada.</span><span class="sxs-lookup"><span data-stu-id="da175-123">This property is only required if a relative query (i.e., ./manager) is specified.</span></span> |

### <a name="supported-queries-for-accessreviewreviewerscope"></a><span data-ttu-id="da175-124">Consultas com suporte para o accessReviewReviewerScope</span><span class="sxs-lookup"><span data-stu-id="da175-124">Supported queries for accessReviewReviewerScope</span></span>

|<span data-ttu-id="da175-125">Cenário</span><span class="sxs-lookup"><span data-stu-id="da175-125">Scenario</span></span>| <span data-ttu-id="da175-126">consulta</span><span class="sxs-lookup"><span data-stu-id="da175-126">query</span></span> | <span data-ttu-id="da175-127">queryType</span><span class="sxs-lookup"><span data-stu-id="da175-127">queryType</span></span> | <span data-ttu-id="da175-128">queryRoot</span><span class="sxs-lookup"><span data-stu-id="da175-128">queryRoot</span></span> |
|--|--|--|--|
| <span data-ttu-id="da175-129">Proprietário do grupo como revisor</span><span class="sxs-lookup"><span data-stu-id="da175-129">Group owner as reviewer</span></span> | <span data-ttu-id="da175-130">/groups/{Group ID}/Owners</span><span class="sxs-lookup"><span data-stu-id="da175-130">/groups/{group id}/owners</span></span> |<span data-ttu-id="da175-131">MicrosoftGraph</span><span class="sxs-lookup"><span data-stu-id="da175-131">MicrosoftGraph</span></span>||
| <span data-ttu-id="da175-132">Usuário específico como revisor</span><span class="sxs-lookup"><span data-stu-id="da175-132">Specific user as reviewer</span></span> | <span data-ttu-id="da175-133">ID/Users/{User}</span><span class="sxs-lookup"><span data-stu-id="da175-133">/users/{user id}</span></span> |<span data-ttu-id="da175-134">MicrosoftGraph</span><span class="sxs-lookup"><span data-stu-id="da175-134">MicrosoftGraph</span></span>||
| <span data-ttu-id="da175-135">Gerente do usuário que está sendo revisado como revisor</span><span class="sxs-lookup"><span data-stu-id="da175-135">Manager of user being reviewed as reviewer</span></span> | <span data-ttu-id="da175-136">./manager</span><span class="sxs-lookup"><span data-stu-id="da175-136">./manager</span></span> | <span data-ttu-id="da175-137">MicrosoftGraph</span><span class="sxs-lookup"><span data-stu-id="da175-137">MicrosoftGraph</span></span> |<span data-ttu-id="da175-138">correta</span><span class="sxs-lookup"><span data-stu-id="da175-138">decisions</span></span>|

## <a name="relationships"></a><span data-ttu-id="da175-139">Relações</span><span class="sxs-lookup"><span data-stu-id="da175-139">Relationships</span></span>
<span data-ttu-id="da175-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="da175-140">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="da175-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="da175-141">JSON representation</span></span>
<span data-ttu-id="da175-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="da175-142">The following is a JSON representation of the resource.</span></span>
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
