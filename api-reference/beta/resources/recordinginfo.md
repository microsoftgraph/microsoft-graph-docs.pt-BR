---
title: tipo de recurso de recordingInfo
description: Informações de gravação para um participante.
author: VinodRavichandran
ms.openlocfilehash: 709edcc6d473ce610cbba7f628e4ebc5057b779c
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380300"
---
# <a name="recordinginfo-resource-type"></a><span data-ttu-id="6d4fd-103">tipo de recurso de recordingInfo</span><span class="sxs-lookup"><span data-stu-id="6d4fd-103">recordingInfo resource type</span></span>

> <span data-ttu-id="6d4fd-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6d4fd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6d4fd-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6d4fd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6d4fd-106">Informações de gravação para um participante.</span><span class="sxs-lookup"><span data-stu-id="6d4fd-106">Recording information for a participant.</span></span>

## <a name="properties"></a><span data-ttu-id="6d4fd-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6d4fd-107">Properties</span></span>

| <span data-ttu-id="6d4fd-108">Propriedade	</span><span class="sxs-lookup"><span data-stu-id="6d4fd-108">Property</span></span>       | <span data-ttu-id="6d4fd-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d4fd-109">Type</span></span>    | <span data-ttu-id="6d4fd-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d4fd-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6d4fd-111">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="6d4fd-111">initiatedBy</span></span> | [<span data-ttu-id="6d4fd-112">participantInfo</span><span class="sxs-lookup"><span data-stu-id="6d4fd-112">participantInfo</span></span>](participantinfo.md) | <span data-ttu-id="6d4fd-113">O participante que iniciou a gravação.</span><span class="sxs-lookup"><span data-stu-id="6d4fd-113">The participant who initiated the recording.</span></span> |
| <span data-ttu-id="6d4fd-114">status</span><span class="sxs-lookup"><span data-stu-id="6d4fd-114">status</span></span> | <span data-ttu-id="6d4fd-115">String</span><span class="sxs-lookup"><span data-stu-id="6d4fd-115">String</span></span> | <span data-ttu-id="6d4fd-116">Os valores possíveis são: `recordingCapable`, `notRecording`, `startedRecording`.</span><span class="sxs-lookup"><span data-stu-id="6d4fd-116">Possible values are: `recordingCapable`, `notRecording`, `startedRecording`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6d4fd-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6d4fd-117">JSON representation</span></span>

<span data-ttu-id="6d4fd-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6d4fd-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recordingInfo"
}-->
```json
{
  "initiatedBy": {"@odata.type": "#microsoft.graph.participantInfo"},
  "status": "recordingCapable | notRecording | startedRecording"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recordingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
