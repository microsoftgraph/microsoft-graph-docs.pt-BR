---
title: Tipo de recurso accessReviewnotificationrecipientqueryscope
description: Representa os usuários que receberão notificações para avaliações de acesso.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 19b619b7479212e5fc055f5ab19b025d8d512dc1
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896730"
---
# <a name="accessreviewnotificationrecipientqueryscope-resource-type"></a><span data-ttu-id="fa3ab-103">Tipo de recurso accessReviewnotificationrecipientqueryscope</span><span class="sxs-lookup"><span data-stu-id="fa3ab-103">accessReviewnotificationrecipientqueryscope resource type</span></span>

<span data-ttu-id="fa3ab-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa3ab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="fa3ab-105">Especifica uma lista estática de destinatários (por exemplo, usuários específicos, proprietários de grupo ou membros do grupo) para receber notificações de revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="fa3ab-105">Specifies a static list of recipients (for example, specific users, group owners, or group members) to receive access review notifications.</span></span>

<span data-ttu-id="fa3ab-106">Herda de [accessReviewNotificationRecipientScope](../resources/accessreviewnotificationrecipientscope.md).</span><span class="sxs-lookup"><span data-stu-id="fa3ab-106">Inherits from [accessReviewNotificationRecipientScope](../resources/accessreviewnotificationrecipientscope.md).</span></span>

## <a name="properties"></a><span data-ttu-id="fa3ab-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fa3ab-107">Properties</span></span>
| <span data-ttu-id="fa3ab-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fa3ab-108">Property</span></span> | <span data-ttu-id="fa3ab-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="fa3ab-109">Type</span></span> | <span data-ttu-id="fa3ab-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa3ab-110">Description</span></span> |
| :-------------------------| :---------- | :---------- |
| <span data-ttu-id="fa3ab-111">consulta</span><span class="sxs-lookup"><span data-stu-id="fa3ab-111">query</span></span> | <span data-ttu-id="fa3ab-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fa3ab-112">String</span></span> | <span data-ttu-id="fa3ab-113">Isso representa a consulta para quem são os destinatários.</span><span class="sxs-lookup"><span data-stu-id="fa3ab-113">This represents the query for who the recipients are.</span></span> <span data-ttu-id="fa3ab-114">Por exemplo, `/groups/{group id}/members` para membros do grupo e para um usuário `/users/{user id}` específico.</span><span class="sxs-lookup"><span data-stu-id="fa3ab-114">For example, `/groups/{group id}/members` for group members and `/users/{user id}` for a specific user.</span></span> |
| <span data-ttu-id="fa3ab-115">queryType</span><span class="sxs-lookup"><span data-stu-id="fa3ab-115">queryType</span></span> | <span data-ttu-id="fa3ab-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fa3ab-116">String</span></span> | <span data-ttu-id="fa3ab-117">Indica o tipo de consulta.</span><span class="sxs-lookup"><span data-stu-id="fa3ab-117">Indicates the type of query.</span></span> <span data-ttu-id="fa3ab-118">O valor permitido é `MicrosoftGraph` .</span><span class="sxs-lookup"><span data-stu-id="fa3ab-118">Allowed value is `MicrosoftGraph`.</span></span> |
| <span data-ttu-id="fa3ab-119">queryRoot</span><span class="sxs-lookup"><span data-stu-id="fa3ab-119">queryRoot</span></span> | <span data-ttu-id="fa3ab-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fa3ab-120">String</span></span> | <span data-ttu-id="fa3ab-121">No cenário em que os revisadores precisam ser especificados dinamicamente, essa propriedade é usada para indicar a fonte relativa da consulta.</span><span class="sxs-lookup"><span data-stu-id="fa3ab-121">In the scenario where reviewers need to be specified dynamically, this property is used to indicate the relative source of the query.</span></span> <span data-ttu-id="fa3ab-122">Essa propriedade só será necessária se uma consulta relativa, ou seja, `./manager` ) for especificada.</span><span class="sxs-lookup"><span data-stu-id="fa3ab-122">This property is only required if a relative query that is, `./manager`) is specified.</span></span> |


## <a name="relationships"></a><span data-ttu-id="fa3ab-123">Relações</span><span class="sxs-lookup"><span data-stu-id="fa3ab-123">Relationships</span></span>
<span data-ttu-id="fa3ab-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fa3ab-124">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fa3ab-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fa3ab-125">JSON representation</span></span>
<span data-ttu-id="fa3ab-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fa3ab-126">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewNotificationRecipientQueryScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewNotificationRecipientQueryScope",
  "query": "String",
  "queryType": "String",
  "queryRoot": "String"
}
```
