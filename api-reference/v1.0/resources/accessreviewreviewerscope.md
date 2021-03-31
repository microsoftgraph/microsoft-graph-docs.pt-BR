---
title: Tipo de recurso accessReviewReviewerScope
description: Representa quem revisará uma revisão de acesso.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 55f881ff1bcb1b08cc66938fd8a7b4d28f540687
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469514"
---
# <a name="accessreviewreviewerscope-resource-type"></a><span data-ttu-id="99da7-103">Tipo de recurso accessReviewReviewerScope</span><span class="sxs-lookup"><span data-stu-id="99da7-103">accessReviewReviewerScope resource type</span></span>

<span data-ttu-id="99da7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99da7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="99da7-105">O accessReviewReviewerScope define quem é especificado no [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) para revisar [appConsentRequests](../resources/appconsentrequest.md) e [userConsentRequests](../resources/appconsentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="99da7-105">The accessReviewReviewerScope defines who is specified in the [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) to review [appConsentRequests](../resources/appconsentrequest.md) and [userConsentRequests](../resources/appconsentrequest.md).</span></span> <span data-ttu-id="99da7-106">Isso é expresso como uma consulta OData, que permite que os revisadores sejam especificados como uma lista estática de usuários (ou seja, usuários específicos, proprietários de grupo, membros do grupo) ou dinamicamente (ou seja, o caso em que cada usuário é revisado por seu gerente).</span><span class="sxs-lookup"><span data-stu-id="99da7-106">This is expressed as an OData query, which allows reviewers to be specified both as a static list of users (i.e., specific users, group owners, group members) or dynamically (i.e., the case where every user is reviewed by their manager).</span></span>

## <a name="properties"></a><span data-ttu-id="99da7-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="99da7-107">Properties</span></span>

|<span data-ttu-id="99da7-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="99da7-108">Property</span></span>|<span data-ttu-id="99da7-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="99da7-109">Type</span></span>|<span data-ttu-id="99da7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="99da7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99da7-111">consulta</span><span class="sxs-lookup"><span data-stu-id="99da7-111">query</span></span>|<span data-ttu-id="99da7-112">String</span><span class="sxs-lookup"><span data-stu-id="99da7-112">String</span></span>|<span data-ttu-id="99da7-113">A consulta especificando quem será o revistor.</span><span class="sxs-lookup"><span data-stu-id="99da7-113">The query specifying who will be the reviewer.</span></span> <span data-ttu-id="99da7-114">Consulte tabela para exemplos.</span><span class="sxs-lookup"><span data-stu-id="99da7-114">See table for examples.</span></span> |
|<span data-ttu-id="99da7-115">queryRoot</span><span class="sxs-lookup"><span data-stu-id="99da7-115">queryRoot</span></span>|<span data-ttu-id="99da7-116">String</span><span class="sxs-lookup"><span data-stu-id="99da7-116">String</span></span>|<span data-ttu-id="99da7-117">O tipo de consulta.</span><span class="sxs-lookup"><span data-stu-id="99da7-117">The type of query.</span></span> <span data-ttu-id="99da7-118">Exemplos incluem `MicrosoftGraph` `ARM` e .</span><span class="sxs-lookup"><span data-stu-id="99da7-118">Examples include `MicrosoftGraph` and `ARM`.</span></span>|
|<span data-ttu-id="99da7-119">queryType</span><span class="sxs-lookup"><span data-stu-id="99da7-119">queryType</span></span>|<span data-ttu-id="99da7-120">String</span><span class="sxs-lookup"><span data-stu-id="99da7-120">String</span></span>|<span data-ttu-id="99da7-121">No cenário em que os revisadores precisam ser especificados dinamicamente, essa propriedade é usada para indicar a fonte relativa da consulta.</span><span class="sxs-lookup"><span data-stu-id="99da7-121">In the scenario where reviewers need to be specified dynamically, this property is used to indicate the relative source of the query.</span></span> <span data-ttu-id="99da7-122">Essa propriedade só será necessária se uma consulta relativa (ou seja, `./manager` ) for especificada.</span><span class="sxs-lookup"><span data-stu-id="99da7-122">This property is only required if a relative query (i.e., `./manager`) is specified.</span></span>|

### <a name="supported-queries-for-accessreviewreviewerscope"></a><span data-ttu-id="99da7-123">Consultas com suporte para accessReviewReviewerScope</span><span class="sxs-lookup"><span data-stu-id="99da7-123">Supported queries for accessReviewReviewerScope</span></span>

|<span data-ttu-id="99da7-124">Cenário</span><span class="sxs-lookup"><span data-stu-id="99da7-124">Scenario</span></span>| <span data-ttu-id="99da7-125">consulta</span><span class="sxs-lookup"><span data-stu-id="99da7-125">query</span></span> | <span data-ttu-id="99da7-126">queryType</span><span class="sxs-lookup"><span data-stu-id="99da7-126">queryType</span></span> | <span data-ttu-id="99da7-127">queryRoot</span><span class="sxs-lookup"><span data-stu-id="99da7-127">queryRoot</span></span> |
|--|--|--|--|
| <span data-ttu-id="99da7-128">Proprietário do grupo como revistor</span><span class="sxs-lookup"><span data-stu-id="99da7-128">Group owner as reviewer</span></span> | <span data-ttu-id="99da7-129">/groups/{group id}/owners</span><span class="sxs-lookup"><span data-stu-id="99da7-129">/groups/{group id}/owners</span></span> |<span data-ttu-id="99da7-130">MicrosoftGraph</span><span class="sxs-lookup"><span data-stu-id="99da7-130">MicrosoftGraph</span></span>||
| <span data-ttu-id="99da7-131">Usuário específico como revistor</span><span class="sxs-lookup"><span data-stu-id="99da7-131">Specific user as reviewer</span></span> | <span data-ttu-id="99da7-132">/users/{user id}</span><span class="sxs-lookup"><span data-stu-id="99da7-132">/users/{user id}</span></span> |<span data-ttu-id="99da7-133">MicrosoftGraph</span><span class="sxs-lookup"><span data-stu-id="99da7-133">MicrosoftGraph</span></span>||
| <span data-ttu-id="99da7-134">Gerente do usuário que está sendo revisado como revistor</span><span class="sxs-lookup"><span data-stu-id="99da7-134">Manager of user being reviewed as reviewer</span></span> | <span data-ttu-id="99da7-135">./manager</span><span class="sxs-lookup"><span data-stu-id="99da7-135">./manager</span></span> | <span data-ttu-id="99da7-136">MicrosoftGraph</span><span class="sxs-lookup"><span data-stu-id="99da7-136">MicrosoftGraph</span></span> |<span data-ttu-id="99da7-137">decisions</span><span class="sxs-lookup"><span data-stu-id="99da7-137">decisions</span></span>|

## <a name="relationships"></a><span data-ttu-id="99da7-138">Relações</span><span class="sxs-lookup"><span data-stu-id="99da7-138">Relationships</span></span>

<span data-ttu-id="99da7-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="99da7-139">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="99da7-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="99da7-140">JSON representation</span></span>

<span data-ttu-id="99da7-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="99da7-141">The following is a JSON representation of the resource.</span></span>
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
