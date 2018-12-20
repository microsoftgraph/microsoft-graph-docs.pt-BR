---
title: tipo de recurso de meetingParticipantInfo
description: Informações sobre um participante em uma reunião.
author: VinodRavichandran
ms.openlocfilehash: 2bbb410ea26640ec05d66b5beb0c4b4ea24a42bd
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380195"
---
# <a name="meetingparticipantinfo-resource-type"></a><span data-ttu-id="55e6b-103">tipo de recurso de meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="55e6b-103">meetingParticipantInfo resource type</span></span>

> <span data-ttu-id="55e6b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="55e6b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="55e6b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="55e6b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="55e6b-106">Informações sobre um participante em uma reunião.</span><span class="sxs-lookup"><span data-stu-id="55e6b-106">Information about a participant in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="55e6b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="55e6b-107">Properties</span></span>

| <span data-ttu-id="55e6b-108">Propriedade	</span><span class="sxs-lookup"><span data-stu-id="55e6b-108">Property</span></span>       | <span data-ttu-id="55e6b-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="55e6b-109">Type</span></span>                          | <span data-ttu-id="55e6b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="55e6b-110">Description</span></span>                              |
|:---------------|:------------------------------|:-----------------------------------------|
| <span data-ttu-id="55e6b-111">identidade</span><span class="sxs-lookup"><span data-stu-id="55e6b-111">identity</span></span>       | [<span data-ttu-id="55e6b-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="55e6b-112">identitySet</span></span>](identityset.md) | <span data-ttu-id="55e6b-113">Informações de identidade do participante.</span><span class="sxs-lookup"><span data-stu-id="55e6b-113">Identity information of the participant.</span></span> |
| <span data-ttu-id="55e6b-114">UPN</span><span class="sxs-lookup"><span data-stu-id="55e6b-114">upn</span></span>            | <span data-ttu-id="55e6b-115">String</span><span class="sxs-lookup"><span data-stu-id="55e6b-115">String</span></span>                        | <span data-ttu-id="55e6b-116">Nome principal de usuário do participante.</span><span class="sxs-lookup"><span data-stu-id="55e6b-116">User principal name of the participant.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="55e6b-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="55e6b-117">JSON representation</span></span>

<span data-ttu-id="55e6b-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="55e6b-118">The following is a JSON representation of the resource.</span></span>

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
