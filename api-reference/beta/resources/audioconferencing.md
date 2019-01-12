---
title: tipo de recurso de audioConferencing
description: Representa as informações de acesso telefônicas de um onlineMeeting.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: cd65b094a17ad3fa470471c3ed6dd3908367e578
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977504"
---
# <a name="audioconferencing-resource-type"></a><span data-ttu-id="a69cb-103">tipo de recurso de audioConferencing</span><span class="sxs-lookup"><span data-stu-id="a69cb-103">audioConferencing resource type</span></span>

> <span data-ttu-id="a69cb-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a69cb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a69cb-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a69cb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a69cb-106">Representa as informações de acesso telefônicas de um [onlineMeeting](onlinemeeting.md).</span><span class="sxs-lookup"><span data-stu-id="a69cb-106">Represents phone access information for an [onlineMeeting](onlinemeeting.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a69cb-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a69cb-107">Properties</span></span>

| <span data-ttu-id="a69cb-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a69cb-108">Property</span></span>            | <span data-ttu-id="a69cb-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a69cb-109">Type</span></span>    | <span data-ttu-id="a69cb-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a69cb-110">Description</span></span>                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="a69cb-111">dialinUrl</span><span class="sxs-lookup"><span data-stu-id="a69cb-111">dialinUrl</span></span>           | <span data-ttu-id="a69cb-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a69cb-112">String</span></span>  | <span data-ttu-id="a69cb-113">Uma URL para a página da web acessível externamente que contém informações de discagem.</span><span class="sxs-lookup"><span data-stu-id="a69cb-113">A URL to the externally-accessible web page that contains dial-in information.</span></span> |
| <span data-ttu-id="a69cb-114">leaderPasscode</span><span class="sxs-lookup"><span data-stu-id="a69cb-114">leaderPasscode</span></span>      | <span data-ttu-id="a69cb-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a69cb-115">String</span></span>  | <span data-ttu-id="a69cb-116">A senha de líder necessária para conectar ao provedor de conferência de áudio.</span><span class="sxs-lookup"><span data-stu-id="a69cb-116">The leader password required to connect to the Audio Conference Provider.</span></span>      |
| <span data-ttu-id="a69cb-117">participantPasscode</span><span class="sxs-lookup"><span data-stu-id="a69cb-117">participantPasscode</span></span> | <span data-ttu-id="a69cb-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a69cb-118">String</span></span>  | <span data-ttu-id="a69cb-119">A senha de participante necessária para conectar ao provedor de conferência de áudio.</span><span class="sxs-lookup"><span data-stu-id="a69cb-119">The participant password required to connect to the Audio Conference Provider.</span></span> |
| <span data-ttu-id="a69cb-120">tollFreeNumber</span><span class="sxs-lookup"><span data-stu-id="a69cb-120">tollFreeNumber</span></span>      | <span data-ttu-id="a69cb-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a69cb-121">String</span></span>  | <span data-ttu-id="a69cb-122">O número de chamada gratuito para conectar ao provedor de conferência de áudio.</span><span class="sxs-lookup"><span data-stu-id="a69cb-122">The toll-free number to connect to the Audio Conference Provider.</span></span>              |
| <span data-ttu-id="a69cb-123">tollNumber</span><span class="sxs-lookup"><span data-stu-id="a69cb-123">tollNumber</span></span>          | <span data-ttu-id="a69cb-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a69cb-124">String</span></span>  | <span data-ttu-id="a69cb-125">O número de Chamada Tarifada para conectar ao provedor de conferência de áudio.</span><span class="sxs-lookup"><span data-stu-id="a69cb-125">The toll number to connect to the Audio Conference Provider.</span></span>                   |

## <a name="json-representation"></a><span data-ttu-id="a69cb-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a69cb-126">JSON representation</span></span>

<span data-ttu-id="a69cb-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a69cb-127">The following is a JSON representation of the resource.</span></span>

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
