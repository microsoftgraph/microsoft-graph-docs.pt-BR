---
title: Tipo de recurso teamMembersNotificationRecipient
description: Representa o destinatário de uma notificação enviada em um feed Microsoft Teams atividade. O destinatário consiste nos membros da equipe.
author: eddie-lee-msft
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a025b6c4ecb9c2eba9f6b31f5eedf108f6ed87ed
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211209"
---
# <a name="teammembersnotificationrecipient-resource-type"></a><span data-ttu-id="612f3-104">Tipo de recurso teamMembersNotificationRecipient</span><span class="sxs-lookup"><span data-stu-id="612f3-104">teamMembersNotificationRecipient resource type</span></span>

<span data-ttu-id="612f3-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="612f3-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="612f3-106">Representa o destinatário de uma notificação enviada em um feed Microsoft Teams atividade.</span><span class="sxs-lookup"><span data-stu-id="612f3-106">Represents the recipient of a notification sent in a Microsoft Teams activity feed.</span></span> <span data-ttu-id="612f3-107">O destinatário consiste nos membros da equipe.</span><span class="sxs-lookup"><span data-stu-id="612f3-107">The recipient consists of the team members.</span></span>

<span data-ttu-id="612f3-108">Herda de [teamworkNotificationRecipient](teamworknotificationrecipient.md).</span><span class="sxs-lookup"><span data-stu-id="612f3-108">Inherits from [teamworkNotificationRecipient](teamworknotificationrecipient.md).</span></span>

## <a name="properties"></a><span data-ttu-id="612f3-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="612f3-109">Properties</span></span>
|<span data-ttu-id="612f3-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="612f3-110">Property</span></span>|<span data-ttu-id="612f3-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="612f3-111">Type</span></span>|<span data-ttu-id="612f3-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="612f3-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="612f3-113">teamId</span><span class="sxs-lookup"><span data-stu-id="612f3-113">teamId</span></span>|<span data-ttu-id="612f3-114">String</span><span class="sxs-lookup"><span data-stu-id="612f3-114">String</span></span>|<span data-ttu-id="612f3-115">O identificador da equipe.</span><span class="sxs-lookup"><span data-stu-id="612f3-115">The team's identifier.</span></span>|

## <a name="relationships"></a><span data-ttu-id="612f3-116">Relações</span><span class="sxs-lookup"><span data-stu-id="612f3-116">Relationships</span></span>
<span data-ttu-id="612f3-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="612f3-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="612f3-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="612f3-118">JSON representation</span></span>
<span data-ttu-id="612f3-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="612f3-119">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamMembersNotificationRecipient"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.teamMembersNotificationRecipient",
  "teamId": "String"
}
```

