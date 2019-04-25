---
title: tipo de recurso audioConferencing
description: Representa as informações de acesso de telefone de um onlineMeeting.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: cb822f2049d84f9a2460370f05d5dfc85c347f15
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535538"
---
# <a name="audioconferencing-resource-type"></a><span data-ttu-id="d830c-103">tipo de recurso audioConferencing</span><span class="sxs-lookup"><span data-stu-id="d830c-103">audioConferencing resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d830c-104">Representa as informações de acesso de telefone de um [onlineMeeting](onlinemeeting.md).</span><span class="sxs-lookup"><span data-stu-id="d830c-104">Represents phone access information for an [onlineMeeting](onlinemeeting.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d830c-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d830c-105">Properties</span></span>

| <span data-ttu-id="d830c-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d830c-106">Property</span></span>            | <span data-ttu-id="d830c-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="d830c-107">Type</span></span>    | <span data-ttu-id="d830c-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="d830c-108">Description</span></span>                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="d830c-109">dialinUrl</span><span class="sxs-lookup"><span data-stu-id="d830c-109">dialinUrl</span></span>           | <span data-ttu-id="d830c-110">String</span><span class="sxs-lookup"><span data-stu-id="d830c-110">String</span></span>  | <span data-ttu-id="d830c-111">Uma URL para a página da Web acessível externamente que contém informações de discagem.</span><span class="sxs-lookup"><span data-stu-id="d830c-111">A URL to the externally-accessible web page that contains dial-in information.</span></span> |
| <span data-ttu-id="d830c-112">leaderPasscode</span><span class="sxs-lookup"><span data-stu-id="d830c-112">leaderPasscode</span></span>      | <span data-ttu-id="d830c-113">String</span><span class="sxs-lookup"><span data-stu-id="d830c-113">String</span></span>  | <span data-ttu-id="d830c-114">A senha de preenchimento necessária para se conectar ao provedor de conferência de áudio.</span><span class="sxs-lookup"><span data-stu-id="d830c-114">The leader password required to connect to the Audio Conference Provider.</span></span>      |
| <span data-ttu-id="d830c-115">participantPasscode</span><span class="sxs-lookup"><span data-stu-id="d830c-115">participantPasscode</span></span> | <span data-ttu-id="d830c-116">String</span><span class="sxs-lookup"><span data-stu-id="d830c-116">String</span></span>  | <span data-ttu-id="d830c-117">A senha do participante necessária para se conectar ao provedor de conferência de áudio.</span><span class="sxs-lookup"><span data-stu-id="d830c-117">The participant password required to connect to the Audio Conference Provider.</span></span> |
| <span data-ttu-id="d830c-118">tollFreeNumber</span><span class="sxs-lookup"><span data-stu-id="d830c-118">tollFreeNumber</span></span>      | <span data-ttu-id="d830c-119">String</span><span class="sxs-lookup"><span data-stu-id="d830c-119">String</span></span>  | <span data-ttu-id="d830c-120">O número de chamada gratuita para se conectar ao provedor de conferência de áudio.</span><span class="sxs-lookup"><span data-stu-id="d830c-120">The toll-free number to connect to the Audio Conference Provider.</span></span>              |
| <span data-ttu-id="d830c-121">tollNumber</span><span class="sxs-lookup"><span data-stu-id="d830c-121">tollNumber</span></span>          | <span data-ttu-id="d830c-122">String</span><span class="sxs-lookup"><span data-stu-id="d830c-122">String</span></span>  | <span data-ttu-id="d830c-123">O número de chamada tarifada para se conectar ao provedor de conferência de áudio.</span><span class="sxs-lookup"><span data-stu-id="d830c-123">The toll number to connect to the Audio Conference Provider.</span></span>                   |

## <a name="json-representation"></a><span data-ttu-id="d830c-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d830c-124">JSON representation</span></span>

<span data-ttu-id="d830c-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d830c-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioConferencing"
}-->
```json
{
  "dialinUrl": "String",
  "leaderPasscode": "String",
  "participantPasscode": "String",
  "tollFreeNumber": "String",
  "tollNumber": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "audioConferencing resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/audioconferencing.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
