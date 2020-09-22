---
title: tipo de recurso teamClassSettings
description: Representa configurações específicas para equipes do tipo classe.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 97a20a312f899db5334003edb1b739bdc3b9e346
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046668"
---
# <a name="teamclasssettings-resource-type"></a><span data-ttu-id="07e3e-103">tipo de recurso teamClassSettings</span><span class="sxs-lookup"><span data-stu-id="07e3e-103">teamClassSettings resource type</span></span>

<span data-ttu-id="07e3e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07e3e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07e3e-105">Representa propriedades específicas de classe de uma [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="07e3e-105">Represents class-specific properties of a [team](team.md).</span></span> <span data-ttu-id="07e3e-106">Disponível apenas quando a equipe representa uma classe.</span><span class="sxs-lookup"><span data-stu-id="07e3e-106">Available only when the team represents a class.</span></span>

## <a name="properties"></a><span data-ttu-id="07e3e-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="07e3e-107">Properties</span></span>
| <span data-ttu-id="07e3e-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="07e3e-108">Property</span></span>     | <span data-ttu-id="07e3e-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="07e3e-109">Type</span></span>   |<span data-ttu-id="07e3e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="07e3e-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="07e3e-111">notifyGuardiansAboutAssignments</span><span class="sxs-lookup"><span data-stu-id="07e3e-111">notifyGuardiansAboutAssignments</span></span>|<span data-ttu-id="07e3e-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="07e3e-112">Boolean</span></span>|<span data-ttu-id="07e3e-113">Se for definido como `true` , habilitará o envio de emails de Resumo de atribuições semanais para pais/guardiões, desde que a administração de locatários tenha habilitado a configuração globalmente.</span><span class="sxs-lookup"><span data-stu-id="07e3e-113">If set to `true`, enables sending of weekly assignments digest emails to parents/guardians, provided the tenant admin has enabled the setting globally.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="07e3e-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="07e3e-114">JSON representation</span></span>

<span data-ttu-id="07e3e-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="07e3e-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamClassSettings"
}-->

```json
{
  "notifyGuardiansAboutAssignments": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "team's classSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


