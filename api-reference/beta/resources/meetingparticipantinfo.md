---
title: tipo de recurso de meetingParticipantInfo
description: Informações sobre um participante em uma reunião.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 409cf7eff4b1151a0ded11674fcde36a519f0e7f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924479"
---
# <a name="meetingparticipantinfo-resource-type"></a><span data-ttu-id="18abf-103">tipo de recurso de meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="18abf-103">meetingParticipantInfo resource type</span></span>

> <span data-ttu-id="18abf-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="18abf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="18abf-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="18abf-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="18abf-106">Informações sobre um participante em uma reunião.</span><span class="sxs-lookup"><span data-stu-id="18abf-106">Information about a participant in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="18abf-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="18abf-107">Properties</span></span>

| <span data-ttu-id="18abf-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="18abf-108">Property</span></span>       | <span data-ttu-id="18abf-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="18abf-109">Type</span></span>                          | <span data-ttu-id="18abf-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="18abf-110">Description</span></span>                              |
|:---------------|:------------------------------|:-----------------------------------------|
| <span data-ttu-id="18abf-111">identidade</span><span class="sxs-lookup"><span data-stu-id="18abf-111">identity</span></span>       | [<span data-ttu-id="18abf-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="18abf-112">identitySet</span></span>](identityset.md) | <span data-ttu-id="18abf-113">Informações de identidade do participante.</span><span class="sxs-lookup"><span data-stu-id="18abf-113">Identity information of the participant.</span></span> |
| <span data-ttu-id="18abf-114">UPN</span><span class="sxs-lookup"><span data-stu-id="18abf-114">upn</span></span>            | <span data-ttu-id="18abf-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18abf-115">String</span></span>                        | <span data-ttu-id="18abf-116">Nome principal de usuário do participante.</span><span class="sxs-lookup"><span data-stu-id="18abf-116">User principal name of the participant.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="18abf-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="18abf-117">JSON representation</span></span>

<span data-ttu-id="18abf-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="18abf-118">The following is a JSON representation of the resource.</span></span>

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
