---
title: tipo de recurso de audioConferencing
description: Representa as informações de acesso telefônicas de um onlineMeeting.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 9bd8343f29a797a24044f02aa2a00bd098c35007
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843621"
---
# <a name="audioconferencing-resource-type"></a><span data-ttu-id="93066-103">tipo de recurso de audioConferencing</span><span class="sxs-lookup"><span data-stu-id="93066-103">audioConferencing resource type</span></span>

> <span data-ttu-id="93066-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="93066-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="93066-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="93066-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="93066-106">Representa as informações de acesso telefônicas de um [onlineMeeting](onlinemeeting.md).</span><span class="sxs-lookup"><span data-stu-id="93066-106">Represents phone access information for an [onlineMeeting](onlinemeeting.md).</span></span>

## <a name="properties"></a><span data-ttu-id="93066-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="93066-107">Properties</span></span>

| <span data-ttu-id="93066-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="93066-108">Property</span></span>            | <span data-ttu-id="93066-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="93066-109">Type</span></span>    | <span data-ttu-id="93066-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="93066-110">Description</span></span>                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="93066-111">dialinUrl</span><span class="sxs-lookup"><span data-stu-id="93066-111">dialinUrl</span></span>           | <span data-ttu-id="93066-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="93066-112">String</span></span>  | <span data-ttu-id="93066-113">Uma URL para a página da web acessível externamente que contém informações de discagem.</span><span class="sxs-lookup"><span data-stu-id="93066-113">A URL to the externally-accessible web page that contains dial-in information.</span></span> |
| <span data-ttu-id="93066-114">leaderPasscode</span><span class="sxs-lookup"><span data-stu-id="93066-114">leaderPasscode</span></span>      | <span data-ttu-id="93066-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="93066-115">String</span></span>  | <span data-ttu-id="93066-116">A senha de líder necessária para conectar ao provedor de conferência de áudio.</span><span class="sxs-lookup"><span data-stu-id="93066-116">The leader password required to connect to the Audio Conference Provider.</span></span>      |
| <span data-ttu-id="93066-117">participantPasscode</span><span class="sxs-lookup"><span data-stu-id="93066-117">participantPasscode</span></span> | <span data-ttu-id="93066-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="93066-118">String</span></span>  | <span data-ttu-id="93066-119">A senha de participante necessária para conectar ao provedor de conferência de áudio.</span><span class="sxs-lookup"><span data-stu-id="93066-119">The participant password required to connect to the Audio Conference Provider.</span></span> |
| <span data-ttu-id="93066-120">tollFreeNumber</span><span class="sxs-lookup"><span data-stu-id="93066-120">tollFreeNumber</span></span>      | <span data-ttu-id="93066-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="93066-121">String</span></span>  | <span data-ttu-id="93066-122">O número de chamada gratuito para conectar ao provedor de conferência de áudio.</span><span class="sxs-lookup"><span data-stu-id="93066-122">The toll-free number to connect to the Audio Conference Provider.</span></span>              |
| <span data-ttu-id="93066-123">tollNumber</span><span class="sxs-lookup"><span data-stu-id="93066-123">tollNumber</span></span>          | <span data-ttu-id="93066-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="93066-124">String</span></span>  | <span data-ttu-id="93066-125">O número de Chamada Tarifada para conectar ao provedor de conferência de áudio.</span><span class="sxs-lookup"><span data-stu-id="93066-125">The toll number to connect to the Audio Conference Provider.</span></span>                   |

## <a name="json-representation"></a><span data-ttu-id="93066-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="93066-126">JSON representation</span></span>

<span data-ttu-id="93066-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="93066-127">The following is a JSON representation of the resource.</span></span>

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
