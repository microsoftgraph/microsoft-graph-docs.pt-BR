---
title: tipo de recurso audioConferencing
description: Representa informações de acesso de telefone de uma reunião online.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 40bc05ac8aba51e78180256c39bd7a20132c4900
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988518"
---
# <a name="audioconferencing-resource-type"></a><span data-ttu-id="c7fd4-103">tipo de recurso audioConferencing</span><span class="sxs-lookup"><span data-stu-id="c7fd4-103">audioConferencing resource type</span></span>

<span data-ttu-id="c7fd4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7fd4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c7fd4-105">Representa as informações de acesso de telefone de um [onlineMeeting](onlinemeeting.md).</span><span class="sxs-lookup"><span data-stu-id="c7fd4-105">Represents phone access information for an [onlineMeeting](onlinemeeting.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c7fd4-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c7fd4-106">Properties</span></span>

| <span data-ttu-id="c7fd4-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c7fd4-107">Property</span></span>            | <span data-ttu-id="c7fd4-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="c7fd4-108">Type</span></span>    | <span data-ttu-id="c7fd4-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7fd4-109">Description</span></span>                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="c7fd4-110">dialinUrl</span><span class="sxs-lookup"><span data-stu-id="c7fd4-110">dialinUrl</span></span>           | <span data-ttu-id="c7fd4-111">String</span><span class="sxs-lookup"><span data-stu-id="c7fd4-111">String</span></span>  | <span data-ttu-id="c7fd4-112">Uma URL para a página da Web acessível externamente que contém informações de discagem.</span><span class="sxs-lookup"><span data-stu-id="c7fd4-112">A URL to the externally-accessible web page that contains dial-in information.</span></span> |
| <span data-ttu-id="c7fd4-113">ID</span><span class="sxs-lookup"><span data-stu-id="c7fd4-113">ConferenceId</span></span>        | <span data-ttu-id="c7fd4-114">String</span><span class="sxs-lookup"><span data-stu-id="c7fd4-114">String</span></span>  | <span data-ttu-id="c7fd4-115">A ID de conferência da reunião online.</span><span class="sxs-lookup"><span data-stu-id="c7fd4-115">The conference id of the online meeting.</span></span>      |
| <span data-ttu-id="c7fd4-116">tollFreeNumber</span><span class="sxs-lookup"><span data-stu-id="c7fd4-116">tollFreeNumber</span></span>      | <span data-ttu-id="c7fd4-117">String</span><span class="sxs-lookup"><span data-stu-id="c7fd4-117">String</span></span>  | <span data-ttu-id="c7fd4-118">O número de chamada gratuita que se conecta ao provedor de conferência de áudio.</span><span class="sxs-lookup"><span data-stu-id="c7fd4-118">The toll-free number that connects to the Audio Conference Provider.</span></span>              |
| <span data-ttu-id="c7fd4-119">tollNumber</span><span class="sxs-lookup"><span data-stu-id="c7fd4-119">tollNumber</span></span>          | <span data-ttu-id="c7fd4-120">String</span><span class="sxs-lookup"><span data-stu-id="c7fd4-120">String</span></span>  | <span data-ttu-id="c7fd4-121">O número de chamada tarifada que se conecta ao provedor de conferência de áudio.</span><span class="sxs-lookup"><span data-stu-id="c7fd4-121">The toll number that connects to the Audio Conference Provider.</span></span>                   |

## <a name="json-representation"></a><span data-ttu-id="c7fd4-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c7fd4-122">JSON representation</span></span>

<span data-ttu-id="c7fd4-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c7fd4-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioConferencing"
}-->
```json
{
  "dialinUrl": "String",
  "ConferenceId": "String",
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
  "suppressions": []
}
-->

