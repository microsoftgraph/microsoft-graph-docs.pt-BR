---
title: tipo de recurso de audioConferencing
description: Representa as informações de acesso telefônicas de um onlineMeeting.
ms.openlocfilehash: dd23c6ade282e081482a8c079491644c663b4054
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035466"
---
# <a name="audioconferencing-resource-type"></a><span data-ttu-id="00ad6-103">tipo de recurso de audioConferencing</span><span class="sxs-lookup"><span data-stu-id="00ad6-103">audioConferencing resource type</span></span>

> <span data-ttu-id="00ad6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="00ad6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="00ad6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="00ad6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="00ad6-106">Representa as informações de acesso telefônicas de um [onlineMeeting](onlinemeeting.md).</span><span class="sxs-lookup"><span data-stu-id="00ad6-106">Represents phone access information for an [onlineMeeting](onlinemeeting.md).</span></span>

## <a name="properties"></a><span data-ttu-id="00ad6-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="00ad6-107">Properties</span></span>

| <span data-ttu-id="00ad6-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="00ad6-108">Property</span></span>            | <span data-ttu-id="00ad6-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="00ad6-109">Type</span></span>    | <span data-ttu-id="00ad6-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="00ad6-110">Description</span></span>                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="00ad6-111">dialinUrl</span><span class="sxs-lookup"><span data-stu-id="00ad6-111">dialinUrl</span></span>           | <span data-ttu-id="00ad6-112">String</span><span class="sxs-lookup"><span data-stu-id="00ad6-112">String</span></span>  | <span data-ttu-id="00ad6-113">Uma URL para a página da web acessível externamente que contém informações de discagem.</span><span class="sxs-lookup"><span data-stu-id="00ad6-113">A URL to the externally-accessible web page that contains dial-in information.</span></span> |
| <span data-ttu-id="00ad6-114">leaderPasscode</span><span class="sxs-lookup"><span data-stu-id="00ad6-114">leaderPasscode</span></span>      | <span data-ttu-id="00ad6-115">String</span><span class="sxs-lookup"><span data-stu-id="00ad6-115">String</span></span>  | <span data-ttu-id="00ad6-116">A senha de líder necessária para conectar ao provedor de conferência de áudio.</span><span class="sxs-lookup"><span data-stu-id="00ad6-116">The leader password required to connect to the Audio Conference Provider.</span></span>      |
| <span data-ttu-id="00ad6-117">participantPasscode</span><span class="sxs-lookup"><span data-stu-id="00ad6-117">participantPasscode</span></span> | <span data-ttu-id="00ad6-118">String</span><span class="sxs-lookup"><span data-stu-id="00ad6-118">String</span></span>  | <span data-ttu-id="00ad6-119">A senha de participante necessária para conectar ao provedor de conferência de áudio.</span><span class="sxs-lookup"><span data-stu-id="00ad6-119">The participant password required to connect to the Audio Conference Provider.</span></span> |
| <span data-ttu-id="00ad6-120">tollFreeNumber</span><span class="sxs-lookup"><span data-stu-id="00ad6-120">tollFreeNumber</span></span>      | <span data-ttu-id="00ad6-121">String</span><span class="sxs-lookup"><span data-stu-id="00ad6-121">String</span></span>  | <span data-ttu-id="00ad6-122">O número de chamada gratuito para conectar ao provedor de conferência de áudio.</span><span class="sxs-lookup"><span data-stu-id="00ad6-122">The toll-free number to connect to the Audio Conference Provider.</span></span>              |
| <span data-ttu-id="00ad6-123">tollNumber</span><span class="sxs-lookup"><span data-stu-id="00ad6-123">tollNumber</span></span>          | <span data-ttu-id="00ad6-124">String</span><span class="sxs-lookup"><span data-stu-id="00ad6-124">String</span></span>  | <span data-ttu-id="00ad6-125">O número de Chamada Tarifada para conectar ao provedor de conferência de áudio.</span><span class="sxs-lookup"><span data-stu-id="00ad6-125">The toll number to connect to the Audio Conference Provider.</span></span>                   |

## <a name="json-representation"></a><span data-ttu-id="00ad6-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="00ad6-126">JSON representation</span></span>

<span data-ttu-id="00ad6-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="00ad6-127">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "audioConferencing resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
