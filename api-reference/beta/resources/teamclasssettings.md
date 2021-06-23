---
title: Tipo de recurso teamClassSettings
description: Representa configurações específicas para equipes do tipo Classe.
localization_priority: Normal
author: akjo
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 10ba45299a8c0d1b28b855aad3a2321930f618e9
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060478"
---
# <a name="teamclasssettings-resource-type"></a><span data-ttu-id="995ac-103">Tipo de recurso teamClassSettings</span><span class="sxs-lookup"><span data-stu-id="995ac-103">teamClassSettings resource type</span></span>

<span data-ttu-id="995ac-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="995ac-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="995ac-105">Representa propriedades específicas da classe de uma [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="995ac-105">Represents class-specific properties of a [team](team.md).</span></span> <span data-ttu-id="995ac-106">Disponível apenas quando a equipe representa uma classe.</span><span class="sxs-lookup"><span data-stu-id="995ac-106">Available only when the team represents a class.</span></span>

## <a name="properties"></a><span data-ttu-id="995ac-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="995ac-107">Properties</span></span>
| <span data-ttu-id="995ac-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="995ac-108">Property</span></span>     | <span data-ttu-id="995ac-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="995ac-109">Type</span></span>   |<span data-ttu-id="995ac-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="995ac-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="995ac-111">notifyGuardiansAboutAssignments</span><span class="sxs-lookup"><span data-stu-id="995ac-111">notifyGuardiansAboutAssignments</span></span>|<span data-ttu-id="995ac-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="995ac-112">Boolean</span></span>|<span data-ttu-id="995ac-113">Se definido como , habilita o envio de atribuições semanais digere emails para pais/responsáveis, desde que o administrador do locatário tenha habilitado a `true` configuração globalmente.</span><span class="sxs-lookup"><span data-stu-id="995ac-113">If set to `true`, enables sending of weekly assignments digest emails to parents/guardians, provided the tenant admin has enabled the setting globally.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="995ac-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="995ac-114">JSON representation</span></span>

<span data-ttu-id="995ac-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="995ac-115">The following is a JSON representation of the resource.</span></span>

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


