---
title: tipo de recurso de meetingParticipantInfo
description: Informações sobre um participante em uma reunião.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: d7b5ae17bd3bfb566bce0da9814b86aab98173da
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834255"
---
# <a name="meetingparticipantinfo-resource-type"></a><span data-ttu-id="c0514-103">tipo de recurso de meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="c0514-103">meetingParticipantInfo resource type</span></span>

> <span data-ttu-id="c0514-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c0514-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c0514-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c0514-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c0514-106">Informações sobre um participante em uma reunião.</span><span class="sxs-lookup"><span data-stu-id="c0514-106">Information about a participant in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="c0514-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c0514-107">Properties</span></span>

| <span data-ttu-id="c0514-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c0514-108">Property</span></span>       | <span data-ttu-id="c0514-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="c0514-109">Type</span></span>                          | <span data-ttu-id="c0514-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0514-110">Description</span></span>                              |
|:---------------|:------------------------------|:-----------------------------------------|
| <span data-ttu-id="c0514-111">identidade</span><span class="sxs-lookup"><span data-stu-id="c0514-111">identity</span></span>       | [<span data-ttu-id="c0514-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="c0514-112">identitySet</span></span>](identityset.md) | <span data-ttu-id="c0514-113">Informações de identidade do participante.</span><span class="sxs-lookup"><span data-stu-id="c0514-113">Identity information of the participant.</span></span> |
| <span data-ttu-id="c0514-114">UPN</span><span class="sxs-lookup"><span data-stu-id="c0514-114">upn</span></span>            | <span data-ttu-id="c0514-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c0514-115">String</span></span>                        | <span data-ttu-id="c0514-116">Nome principal de usuário do participante.</span><span class="sxs-lookup"><span data-stu-id="c0514-116">User principal name of the participant.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="c0514-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c0514-117">JSON representation</span></span>

<span data-ttu-id="c0514-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c0514-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingParticipantInfo"
}-->
```json
{
  "identity": {"@odata.type": "#microsoft.graph.identitySet"},
  "upn": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingParticipantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
