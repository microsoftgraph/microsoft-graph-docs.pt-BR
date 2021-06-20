---
title: Tipo de recurso accessReviewReviewerScope
description: Representa quem revisará uma revisão de acesso.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 85d602f72bc103b1588c3c9a76455fa2de0f8259
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030807"
---
# <a name="accessreviewreviewerscope-resource-type"></a><span data-ttu-id="369a3-103">Tipo de recurso accessReviewReviewerScope</span><span class="sxs-lookup"><span data-stu-id="369a3-103">accessReviewReviewerScope resource type</span></span>

<span data-ttu-id="369a3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="369a3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="369a3-105">O accessReviewReviewerScope define quem revisará instâncias de [um accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="369a3-105">The accessReviewReviewerScope defines who will review instances of an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="369a3-106">É uma consulta OData que permite que os revisadores sejam especificados como uma lista estática de usuários (ou seja, usuários específicos, proprietários de grupos e membros do grupo) ou dinamicamente em que cada usuário é revisado por seu gerente ou por proprietários de grupo.</span><span class="sxs-lookup"><span data-stu-id="369a3-106">It is an OData query that allows reviewers to be specified both as a static list of users (that is, specific users, group owners, and group members) or dynamically in which every user is reviewed by their manager or by group owners.</span></span> <span data-ttu-id="369a3-107">Para criar uma auto-revisão (onde os usuários analisam seu próprio acesso), não forneça aos revisores sobre a criação [accessReviewScheduleDefinition.](accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="369a3-107">To create a self-review (where users review their own access), do not provide reviewers on [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) creation.</span></span>

<span data-ttu-id="369a3-108">Herda de [accessReviewScope](../resources/accessreviewscope.md).</span><span class="sxs-lookup"><span data-stu-id="369a3-108">Inherits from [accessReviewScope](../resources/accessreviewscope.md).</span></span>

## <a name="properties"></a><span data-ttu-id="369a3-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="369a3-109">Properties</span></span>
| <span data-ttu-id="369a3-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="369a3-110">Property</span></span> | <span data-ttu-id="369a3-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="369a3-111">Type</span></span> | <span data-ttu-id="369a3-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="369a3-112">Description</span></span> |
| :-------------------------| :---------- | :---------- |
| <span data-ttu-id="369a3-113">consulta</span><span class="sxs-lookup"><span data-stu-id="369a3-113">query</span></span> | <span data-ttu-id="369a3-114">String</span><span class="sxs-lookup"><span data-stu-id="369a3-114">String</span></span> | <span data-ttu-id="369a3-115">A consulta especificando quem será o revistor.</span><span class="sxs-lookup"><span data-stu-id="369a3-115">The query specifying who will be the reviewer.</span></span> <span data-ttu-id="369a3-116">Consulte tabela para exemplos.</span><span class="sxs-lookup"><span data-stu-id="369a3-116">See table for examples.</span></span> |
| <span data-ttu-id="369a3-117">queryType</span><span class="sxs-lookup"><span data-stu-id="369a3-117">queryType</span></span> | <span data-ttu-id="369a3-118">String</span><span class="sxs-lookup"><span data-stu-id="369a3-118">String</span></span> | <span data-ttu-id="369a3-119">O tipo de consulta.</span><span class="sxs-lookup"><span data-stu-id="369a3-119">The type of query.</span></span> <span data-ttu-id="369a3-120">Exemplos incluem `MicrosoftGraph` `ARM` e .</span><span class="sxs-lookup"><span data-stu-id="369a3-120">Examples include `MicrosoftGraph` and `ARM`.</span></span> |
| <span data-ttu-id="369a3-121">queryRoot</span><span class="sxs-lookup"><span data-stu-id="369a3-121">queryRoot</span></span> | <span data-ttu-id="369a3-122">String</span><span class="sxs-lookup"><span data-stu-id="369a3-122">String</span></span> | <span data-ttu-id="369a3-123">No cenário em que os revisadores precisam ser especificados dinamicamente, essa propriedade é usada para indicar a fonte relativa da consulta.</span><span class="sxs-lookup"><span data-stu-id="369a3-123">In the scenario where reviewers need to be specified dynamically, this property is used to indicate the relative source of the query.</span></span> <span data-ttu-id="369a3-124">Essa propriedade só será necessária se uma consulta relativa, por exemplo, `./manager` , for especificada.</span><span class="sxs-lookup"><span data-stu-id="369a3-124">This property is only required if a relative query, for example, `./manager`, is specified.</span></span> <span data-ttu-id="369a3-125">Valor possível: `decisions` .</span><span class="sxs-lookup"><span data-stu-id="369a3-125">Possible value: `decisions`.</span></span> |

<span data-ttu-id="369a3-126">Para obter mais informações sobre opções de configuração para revisadores, consulte Atribuir revisadores à sua definição de revisão de acesso [usando a API do Microsoft Graph](/graph/accessreviews-reviewers-concept).</span><span class="sxs-lookup"><span data-stu-id="369a3-126">For more about configuration options for **reviewers**, see [Assign reviewers to your access review definition using the Microsoft Graph API](/graph/accessreviews-reviewers-concept).</span></span>


## <a name="relationships"></a><span data-ttu-id="369a3-127">Relações</span><span class="sxs-lookup"><span data-stu-id="369a3-127">Relationships</span></span>
<span data-ttu-id="369a3-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="369a3-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="369a3-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="369a3-129">JSON representation</span></span>
<span data-ttu-id="369a3-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="369a3-130">The following is a JSON representation of the resource.</span></span>
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
