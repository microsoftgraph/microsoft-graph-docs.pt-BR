---
title: Tipo de recurso accessReviewInactiveUsersQueryScope
description: Um tipo de accessReviewQueryScope que permite que apenas usuários inativos sejam selecionados no escopo de uma revisão de acesso.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 80d415125679ddbb44a08fe75f33b115e4ba1f04
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579743"
---
# <a name="accessreviewinactiveusersqueryscope-resource-type"></a><span data-ttu-id="18906-103">Tipo de recurso accessReviewInactiveUsersQueryScope</span><span class="sxs-lookup"><span data-stu-id="18906-103">accessReviewInactiveUsersQueryScope resource type</span></span>

<span data-ttu-id="18906-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18906-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="18906-105">Um tipo de [accessReviewQueryScope](../resources/accessreviewqueryscope.md) que permite que apenas usuários inativos sejam selecionados no escopo de uma revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="18906-105">A type of [accessReviewQueryScope](../resources/accessreviewqueryscope.md) that allows only inactive users to be selected in the scope of an access review.</span></span> <span data-ttu-id="18906-106">A duração da inatividade é calculada com base na última data de entrada do usuário em relação à data de início da instância de revisão de acesso, conforme definido na propriedade **settings** [de accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="18906-106">The duration of inactivity is calculated based on the user's last sign-in date against the access review instance's start date as defined in the **settings** property of [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md).</span></span>

<span data-ttu-id="18906-107">Herda de [accessReviewQueryScope](../resources/accessreviewqueryscope.md).</span><span class="sxs-lookup"><span data-stu-id="18906-107">Inherits from [accessReviewQueryScope](../resources/accessreviewqueryscope.md).</span></span>

## <a name="properties"></a><span data-ttu-id="18906-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="18906-108">Properties</span></span>
|<span data-ttu-id="18906-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="18906-109">Property</span></span>|<span data-ttu-id="18906-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="18906-110">Type</span></span>|<span data-ttu-id="18906-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="18906-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18906-112">inactiveDuration</span><span class="sxs-lookup"><span data-stu-id="18906-112">inactiveDuration</span></span>|<span data-ttu-id="18906-113">Duration</span><span class="sxs-lookup"><span data-stu-id="18906-113">Duration</span></span>|<span data-ttu-id="18906-114">Define a duração da inatividade.</span><span class="sxs-lookup"><span data-stu-id="18906-114">Defines the duration of inactivity.</span></span> <span data-ttu-id="18906-115">A inatividade é baseada na última data de entrada do usuário em comparação com a data de início da instância de revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="18906-115">Inactivity is based on the last sign in date of the user compared to the access review instance's start date.</span></span> <span data-ttu-id="18906-116">Se essa propriedade não for especificada, ela será atribuída ao valor padrão `PT0S` .</span><span class="sxs-lookup"><span data-stu-id="18906-116">If this property is not specified, it's assigned the default value `PT0S`.</span></span>|
|<span data-ttu-id="18906-117">consulta</span><span class="sxs-lookup"><span data-stu-id="18906-117">query</span></span>|<span data-ttu-id="18906-118">String</span><span class="sxs-lookup"><span data-stu-id="18906-118">String</span></span>|<span data-ttu-id="18906-119">Herdado [de accessReviewQueryScope](../resources/accessreviewqueryscope.md).</span><span class="sxs-lookup"><span data-stu-id="18906-119">Inherited from [accessReviewQueryScope](../resources/accessreviewqueryscope.md).</span></span>|
|<span data-ttu-id="18906-120">queryRoot</span><span class="sxs-lookup"><span data-stu-id="18906-120">queryRoot</span></span>|<span data-ttu-id="18906-121">String</span><span class="sxs-lookup"><span data-stu-id="18906-121">String</span></span>|<span data-ttu-id="18906-122">Herdado [de accessReviewQueryScope](../resources/accessreviewqueryscope.md).</span><span class="sxs-lookup"><span data-stu-id="18906-122">Inherited from [accessReviewQueryScope](../resources/accessreviewqueryscope.md).</span></span>|
|<span data-ttu-id="18906-123">queryType</span><span class="sxs-lookup"><span data-stu-id="18906-123">queryType</span></span>|<span data-ttu-id="18906-124">String</span><span class="sxs-lookup"><span data-stu-id="18906-124">String</span></span>|<span data-ttu-id="18906-125">Herdado [de accessReviewQueryScope](../resources/accessreviewqueryscope.md).</span><span class="sxs-lookup"><span data-stu-id="18906-125">Inherited from [accessReviewQueryScope](../resources/accessreviewqueryscope.md).</span></span>|

<span data-ttu-id="18906-126">Você também deve especificar a **propriedade @odata.type com** o valor `#microsoft.graph.accessReviewInactiveUsersQueryScope` .</span><span class="sxs-lookup"><span data-stu-id="18906-126">You must also specify the **@odata.type** type property with the value `#microsoft.graph.accessReviewInactiveUsersQueryScope`.</span></span> <span data-ttu-id="18906-127">Para obter mais  informações sobre opções de configuração para escopo usando **accessReviewInactiveUsersQueryScope**, consulte Configure the scope of your [access review definition using the Microsoft Graph API](/graph/accessreviews-scope-concept).</span><span class="sxs-lookup"><span data-stu-id="18906-127">For more about configuration options for **scope** using **accessReviewInactiveUsersQueryScope**, see [Configure the scope of your access review definition using the Microsoft Graph API](/graph/accessreviews-scope-concept).</span></span>

## <a name="relationships"></a><span data-ttu-id="18906-128">Relações</span><span class="sxs-lookup"><span data-stu-id="18906-128">Relationships</span></span>
<span data-ttu-id="18906-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="18906-129">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="18906-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="18906-130">JSON representation</span></span>
<span data-ttu-id="18906-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="18906-131">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewInactiveUsersQueryScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewInactiveUsersQueryScope",
  "query": "String",
  "queryType": "String",
  "queryRoot": "String",
  "inactiveDuration": "String (duration)"
}
```
