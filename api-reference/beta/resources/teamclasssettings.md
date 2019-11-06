---
title: tipo de recurso teamClassSettings
description: Representa configurações específicas para equipes do tipo classe.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ca8d345cd229c4a6c003c87865b5aaddf01096b4
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37998613"
---
# <a name="teamclasssettings-resource-type"></a><span data-ttu-id="3e36b-103">tipo de recurso teamClassSettings</span><span class="sxs-lookup"><span data-stu-id="3e36b-103">teamClassSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e36b-104">Representa propriedades específicas de classe de uma [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="3e36b-104">Represents class-specific properties of a [team](team.md).</span></span> <span data-ttu-id="3e36b-105">Disponível somente quando a equipe representa uma classe.</span><span class="sxs-lookup"><span data-stu-id="3e36b-105">Available only when the team represents a class.</span></span>

## <a name="properties"></a><span data-ttu-id="3e36b-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3e36b-106">Properties</span></span>
| <span data-ttu-id="3e36b-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3e36b-107">Property</span></span>     | <span data-ttu-id="3e36b-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="3e36b-108">Type</span></span>   |<span data-ttu-id="3e36b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e36b-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3e36b-110">notifyGuardiansAboutAssignments</span><span class="sxs-lookup"><span data-stu-id="3e36b-110">notifyGuardiansAboutAssignments</span></span>|<span data-ttu-id="3e36b-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="3e36b-111">Boolean</span></span>|<span data-ttu-id="3e36b-112">Se for definido `true`como, habilitará o envio de emails de Resumo de atribuições semanais para pais/guardiões, desde que a administração de locatários tenha habilitado a configuração globalmente.</span><span class="sxs-lookup"><span data-stu-id="3e36b-112">If set to `true`, enables sending of weekly assignments digest emails to parents/guardians, provided the tenant admin has enabled the setting globally.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3e36b-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3e36b-113">JSON representation</span></span>

<span data-ttu-id="3e36b-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3e36b-114">The following is a JSON representation of the resource.</span></span>

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
