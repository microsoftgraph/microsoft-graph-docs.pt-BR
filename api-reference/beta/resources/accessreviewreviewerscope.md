---
title: Tipo de recurso accessReviewReviewerScope
description: Representa quem revisará uma revisão de acesso.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 58abda6c89e484336b34d546edc68ebbfe432162
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579250"
---
# <a name="accessreviewreviewerscope-resource-type"></a><span data-ttu-id="303a0-103">Tipo de recurso accessReviewReviewerScope</span><span class="sxs-lookup"><span data-stu-id="303a0-103">accessReviewReviewerScope resource type</span></span>

<span data-ttu-id="303a0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="303a0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="303a0-105">O accessReviewReviewerScope define quem revisará instâncias de [um accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="303a0-105">The accessReviewReviewerScope defines who will review instances of an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="303a0-106">É uma consulta OData que permite que os revisadores sejam especificados como uma lista estática de usuários (ou seja, usuários específicos, proprietários de grupos e membros do grupo) ou dinamicamente em que cada usuário é revisado por seu gerente ou por proprietários de grupo.</span><span class="sxs-lookup"><span data-stu-id="303a0-106">It is an OData query that allows reviewers to be specified both as a static list of users (that is, specific users, group owners, and group members) or dynamically in which every user is reviewed by their manager or by group owners.</span></span> <span data-ttu-id="303a0-107">Para criar uma auto-revisão (onde os usuários analisam seu próprio acesso), não forneça aos revisores sobre a criação [accessReviewScheduleDefinition.](accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="303a0-107">To create a self-review (where users review their own access), do not provide reviewers on [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) creation.</span></span>

<span data-ttu-id="303a0-108">Herda de [accessReviewScope](../resources/accessreviewscope.md).</span><span class="sxs-lookup"><span data-stu-id="303a0-108">Inherits from [accessReviewScope](../resources/accessreviewscope.md).</span></span>

## <a name="properties"></a><span data-ttu-id="303a0-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="303a0-109">Properties</span></span>
| <span data-ttu-id="303a0-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="303a0-110">Property</span></span> | <span data-ttu-id="303a0-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="303a0-111">Type</span></span> | <span data-ttu-id="303a0-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="303a0-112">Description</span></span> |
| :-------------------------| :---------- | :---------- |
| <span data-ttu-id="303a0-113">consulta</span><span class="sxs-lookup"><span data-stu-id="303a0-113">query</span></span> | <span data-ttu-id="303a0-114">String</span><span class="sxs-lookup"><span data-stu-id="303a0-114">String</span></span> | <span data-ttu-id="303a0-115">A consulta especificando quem será o revistor.</span><span class="sxs-lookup"><span data-stu-id="303a0-115">The query specifying who will be the reviewer.</span></span> <span data-ttu-id="303a0-116">Consulte tabela para exemplos.</span><span class="sxs-lookup"><span data-stu-id="303a0-116">See table for examples.</span></span> |
| <span data-ttu-id="303a0-117">queryType</span><span class="sxs-lookup"><span data-stu-id="303a0-117">queryType</span></span> | <span data-ttu-id="303a0-118">String</span><span class="sxs-lookup"><span data-stu-id="303a0-118">String</span></span> | <span data-ttu-id="303a0-119">O tipo de consulta.</span><span class="sxs-lookup"><span data-stu-id="303a0-119">The type of query.</span></span> <span data-ttu-id="303a0-120">Exemplos incluem `MicrosoftGraph` `ARM` e .</span><span class="sxs-lookup"><span data-stu-id="303a0-120">Examples include `MicrosoftGraph` and `ARM`.</span></span> |
| <span data-ttu-id="303a0-121">queryRoot</span><span class="sxs-lookup"><span data-stu-id="303a0-121">queryRoot</span></span> | <span data-ttu-id="303a0-122">String</span><span class="sxs-lookup"><span data-stu-id="303a0-122">String</span></span> | <span data-ttu-id="303a0-123">No cenário em que os revisadores precisam ser especificados dinamicamente, essa propriedade é usada para indicar a fonte relativa da consulta.</span><span class="sxs-lookup"><span data-stu-id="303a0-123">In the scenario where reviewers need to be specified dynamically, this property is used to indicate the relative source of the query.</span></span> <span data-ttu-id="303a0-124">Essa propriedade só será necessária se uma consulta relativa, por exemplo, `./manager` , for especificada.</span><span class="sxs-lookup"><span data-stu-id="303a0-124">This property is only required if a relative query, for example, `./manager`, is specified.</span></span> <span data-ttu-id="303a0-125">Valor possível: `decisions` .</span><span class="sxs-lookup"><span data-stu-id="303a0-125">Possible value: `decisions`.</span></span> |

<span data-ttu-id="303a0-126">Para obter mais informações sobre opções de configuração para revisadores, consulte Atribuir revisadores à sua definição de revisão de acesso [usando a API do Microsoft Graph](/graph/accessreviews-reviewers-concept).</span><span class="sxs-lookup"><span data-stu-id="303a0-126">For more about configuration options for **reviewers**, see [Assign reviewers to your access review definition using the Microsoft Graph API](/graph/accessreviews-reviewers-concept).</span></span>


## <a name="relationships"></a><span data-ttu-id="303a0-127">Relações</span><span class="sxs-lookup"><span data-stu-id="303a0-127">Relationships</span></span>
<span data-ttu-id="303a0-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="303a0-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="303a0-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="303a0-129">JSON representation</span></span>
<span data-ttu-id="303a0-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="303a0-130">The following is a JSON representation of the resource.</span></span>
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
