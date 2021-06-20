---
title: Tipo de recurso accessReviewQueryScope
description: Define o que precisa ser revisado em uma revisão de acesso.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 5217524105fd5dcca0248b331f5cc5d0584784aa
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030977"
---
# <a name="accessreviewqueryscope-resource-type"></a><span data-ttu-id="5a4f6-103">Tipo de recurso accessReviewQueryScope</span><span class="sxs-lookup"><span data-stu-id="5a4f6-103">accessReviewQueryScope resource type</span></span>

<span data-ttu-id="5a4f6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a4f6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5a4f6-105">Um objeto accessReviewQueryScope define o que é revisado em uma revisão [de acesso.](../resources/accessreviewsv2-root.md)</span><span class="sxs-lookup"><span data-stu-id="5a4f6-105">An accessReviewQueryScope object defines what is reviewed in an [access review](../resources/accessreviewsv2-root.md).</span></span> <span data-ttu-id="5a4f6-106">Para analisar o escopo de uma revisão de acesso a usuários inativos, consulte [accessReviewInactiveUserQueryScope](../resources/accessreviewinactiveusersqueryscope.md).</span><span class="sxs-lookup"><span data-stu-id="5a4f6-106">To scope an access review to inactive users, see [accessReviewInactiveUserQueryScope](../resources/accessreviewinactiveusersqueryscope.md).</span></span> 

<span data-ttu-id="5a4f6-107">Herda de [accessReviewScope](../resources/accessreviewscope.md).</span><span class="sxs-lookup"><span data-stu-id="5a4f6-107">Inherits from [accessReviewScope](../resources/accessreviewscope.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5a4f6-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5a4f6-108">Properties</span></span>
|<span data-ttu-id="5a4f6-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5a4f6-109">Property</span></span>|<span data-ttu-id="5a4f6-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="5a4f6-110">Type</span></span>|<span data-ttu-id="5a4f6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a4f6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a4f6-112">consulta</span><span class="sxs-lookup"><span data-stu-id="5a4f6-112">query</span></span>|<span data-ttu-id="5a4f6-113">String</span><span class="sxs-lookup"><span data-stu-id="5a4f6-113">String</span></span>|<span data-ttu-id="5a4f6-114">A consulta que representa o que será revisado em uma revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="5a4f6-114">The query representing what will be reviewed in an access review.</span></span>|
|<span data-ttu-id="5a4f6-115">queryRoot</span><span class="sxs-lookup"><span data-stu-id="5a4f6-115">queryRoot</span></span>|<span data-ttu-id="5a4f6-116">String</span><span class="sxs-lookup"><span data-stu-id="5a4f6-116">String</span></span>|<span data-ttu-id="5a4f6-117">No cenário em que os revisadores precisam ser especificados dinamicamente, essa propriedade é usada para indicar a fonte relativa da consulta.</span><span class="sxs-lookup"><span data-stu-id="5a4f6-117">In the scenario where reviewers need to be specified dynamically, this property is used to indicate the relative source of the query.</span></span> <span data-ttu-id="5a4f6-118">Essa propriedade só será necessária se uma consulta relativa for especificada.</span><span class="sxs-lookup"><span data-stu-id="5a4f6-118">This property is only required if a relative query is specified.</span></span> <span data-ttu-id="5a4f6-119">Por exemplo, `./manager`.</span><span class="sxs-lookup"><span data-stu-id="5a4f6-119">For example, `./manager`.</span></span>|
|<span data-ttu-id="5a4f6-120">queryType</span><span class="sxs-lookup"><span data-stu-id="5a4f6-120">queryType</span></span>|<span data-ttu-id="5a4f6-121">String</span><span class="sxs-lookup"><span data-stu-id="5a4f6-121">String</span></span>|<span data-ttu-id="5a4f6-122">Indica o tipo de consulta.</span><span class="sxs-lookup"><span data-stu-id="5a4f6-122">Indicates the type of query.</span></span> <span data-ttu-id="5a4f6-123">Os tipos `MicrosoftGraph` incluem `ARM` e .</span><span class="sxs-lookup"><span data-stu-id="5a4f6-123">Types include `MicrosoftGraph` and `ARM`.</span></span>|

<span data-ttu-id="5a4f6-124">A especificação da **propriedade @odata.type** com o valor `#microsoft.graph.accessReviewQueryScope` é altamente recomendada.</span><span class="sxs-lookup"><span data-stu-id="5a4f6-124">Specifying the **@odata.type** type property with the value `#microsoft.graph.accessReviewQueryScope` is highly recommended.</span></span> <span data-ttu-id="5a4f6-125">Para obter mais  informações sobre opções de configuração para escopo usando **accessReviewQueryScope,** consulte Configure the scope of your [access review definition using the Microsoft Graph API](/graph/accessreviews-scope-concept).</span><span class="sxs-lookup"><span data-stu-id="5a4f6-125">For more about configuration options for **scope** using **accessReviewQueryScope**, see [Configure the scope of your access review definition using the Microsoft Graph API](/graph/accessreviews-scope-concept).</span></span>

## <a name="relationships"></a><span data-ttu-id="5a4f6-126">Relações</span><span class="sxs-lookup"><span data-stu-id="5a4f6-126">Relationships</span></span>
<span data-ttu-id="5a4f6-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5a4f6-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5a4f6-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5a4f6-128">JSON representation</span></span>
<span data-ttu-id="5a4f6-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5a4f6-129">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewQueryScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewQueryScope",
  "query": "String",
  "queryType": "String",
  "queryRoot": "String"
}
```
