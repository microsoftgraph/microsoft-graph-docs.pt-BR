---
title: tipo de recurso audioConferencing
description: Representa informações de acesso de telefone de uma reunião online.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d2eab9732660f53c7e003b49f6c6ca780c8a4610
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865667"
---
# <a name="audioconferencing-resource-type"></a><span data-ttu-id="3e8dc-103">tipo de recurso audioConferencing</span><span class="sxs-lookup"><span data-stu-id="3e8dc-103">audioConferencing resource type</span></span>

<span data-ttu-id="3e8dc-104">Representa as informações de acesso de telefone de um [onlineMeeting](onlinemeeting.md).</span><span class="sxs-lookup"><span data-stu-id="3e8dc-104">Represents phone access information for an [onlineMeeting](onlinemeeting.md).</span></span>

## <a name="properties"></a><span data-ttu-id="3e8dc-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3e8dc-105">Properties</span></span>

| <span data-ttu-id="3e8dc-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3e8dc-106">Property</span></span>            | <span data-ttu-id="3e8dc-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="3e8dc-107">Type</span></span>    | <span data-ttu-id="3e8dc-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e8dc-108">Description</span></span>                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="3e8dc-109">dialinUrl</span><span class="sxs-lookup"><span data-stu-id="3e8dc-109">dialinUrl</span></span>           | <span data-ttu-id="3e8dc-110">String</span><span class="sxs-lookup"><span data-stu-id="3e8dc-110">String</span></span>  | <span data-ttu-id="3e8dc-111">Uma URL para a página da Web acessível externamente que contém informações de discagem.</span><span class="sxs-lookup"><span data-stu-id="3e8dc-111">A URL to the externally-accessible web page that contains dial-in information.</span></span> |
| <span data-ttu-id="3e8dc-112">ID</span><span class="sxs-lookup"><span data-stu-id="3e8dc-112">ConferenceId</span></span>        | <span data-ttu-id="3e8dc-113">String</span><span class="sxs-lookup"><span data-stu-id="3e8dc-113">String</span></span>  | <span data-ttu-id="3e8dc-114">A ID de conferência da reunião online.</span><span class="sxs-lookup"><span data-stu-id="3e8dc-114">The conference id of the online meeting.</span></span>      |
| <span data-ttu-id="3e8dc-115">tollFreeNumber</span><span class="sxs-lookup"><span data-stu-id="3e8dc-115">tollFreeNumber</span></span>      | <span data-ttu-id="3e8dc-116">String</span><span class="sxs-lookup"><span data-stu-id="3e8dc-116">String</span></span>  | <span data-ttu-id="3e8dc-117">O número de chamada gratuita que se conecta ao provedor de conferência de áudio.</span><span class="sxs-lookup"><span data-stu-id="3e8dc-117">The toll-free number that connects to the Audio Conference Provider.</span></span>              |
| <span data-ttu-id="3e8dc-118">tollNumber</span><span class="sxs-lookup"><span data-stu-id="3e8dc-118">tollNumber</span></span>          | <span data-ttu-id="3e8dc-119">String</span><span class="sxs-lookup"><span data-stu-id="3e8dc-119">String</span></span>  | <span data-ttu-id="3e8dc-120">O número de chamada tarifada que se conecta ao provedor de conferência de áudio.</span><span class="sxs-lookup"><span data-stu-id="3e8dc-120">The toll number that connects to the Audio Conference Provider.</span></span>                   |

## <a name="json-representation"></a><span data-ttu-id="3e8dc-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3e8dc-121">JSON representation</span></span>

<span data-ttu-id="3e8dc-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3e8dc-122">The following is a JSON representation of the resource.</span></span>

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
