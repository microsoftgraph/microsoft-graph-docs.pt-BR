---
title: tipo de recurso de meetingParticipantInfo
description: Veja a seguir uma representação JSON do recurso.
ms.openlocfilehash: 1d9c22924f8f05255b5e01bad4bbcd6ae5957ffe
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036806"
---
# <a name="meetingparticipantinfo-resource-type"></a><span data-ttu-id="e2d1f-103">tipo de recurso de meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="e2d1f-103">meetingParticipantInfo resource type</span></span>

> <span data-ttu-id="e2d1f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e2d1f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e2d1f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e2d1f-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="properties"></a><span data-ttu-id="e2d1f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e2d1f-106">Properties</span></span>

| <span data-ttu-id="e2d1f-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e2d1f-107">Property</span></span>       | <span data-ttu-id="e2d1f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="e2d1f-108">Type</span></span>                          | <span data-ttu-id="e2d1f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2d1f-109">Description</span></span>                              |
|:---------------|:------------------------------|:-----------------------------------------|
| <span data-ttu-id="e2d1f-110">identidade</span><span class="sxs-lookup"><span data-stu-id="e2d1f-110">identity</span></span>       | [<span data-ttu-id="e2d1f-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="e2d1f-111">identitySet</span></span>](identityset.md) | <span data-ttu-id="e2d1f-112">Informações de identidade do participante.</span><span class="sxs-lookup"><span data-stu-id="e2d1f-112">Identity information of the participant.</span></span> |
| <span data-ttu-id="e2d1f-113">UPN</span><span class="sxs-lookup"><span data-stu-id="e2d1f-113">upn</span></span>            | <span data-ttu-id="e2d1f-114">String</span><span class="sxs-lookup"><span data-stu-id="e2d1f-114">String</span></span>                        | <span data-ttu-id="e2d1f-115">Nome principal de usuário do participante.</span><span class="sxs-lookup"><span data-stu-id="e2d1f-115">User principal name of the participant.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="e2d1f-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e2d1f-116">JSON representation</span></span>

<span data-ttu-id="e2d1f-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e2d1f-117">The following is a JSON representation of the resource.</span></span>

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
