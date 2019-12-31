---
title: tipo de recurso audioConferencing
description: Representa informações de acesso de telefone de uma reunião online.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: f1c58fb5cbf65b73aed2978fd0b3be45d7d30aec
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913475"
---
# <a name="audioconferencing-resource-type"></a><span data-ttu-id="1cc31-103">tipo de recurso audioConferencing</span><span class="sxs-lookup"><span data-stu-id="1cc31-103">audioConferencing resource type</span></span>

<span data-ttu-id="1cc31-104">Representa as informações de acesso de telefone de um [onlineMeeting](onlinemeeting.md).</span><span class="sxs-lookup"><span data-stu-id="1cc31-104">Represents phone access information for an [onlineMeeting](onlinemeeting.md).</span></span>

## <a name="properties"></a><span data-ttu-id="1cc31-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1cc31-105">Properties</span></span>

| <span data-ttu-id="1cc31-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1cc31-106">Property</span></span>            | <span data-ttu-id="1cc31-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="1cc31-107">Type</span></span>    | <span data-ttu-id="1cc31-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="1cc31-108">Description</span></span>                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="1cc31-109">dialinUrl</span><span class="sxs-lookup"><span data-stu-id="1cc31-109">dialinUrl</span></span>           | <span data-ttu-id="1cc31-110">String</span><span class="sxs-lookup"><span data-stu-id="1cc31-110">String</span></span>  | <span data-ttu-id="1cc31-111">Uma URL para a página da Web acessível externamente que contém informações de discagem.</span><span class="sxs-lookup"><span data-stu-id="1cc31-111">A URL to the externally-accessible web page that contains dial-in information.</span></span> |
| <span data-ttu-id="1cc31-112">ID</span><span class="sxs-lookup"><span data-stu-id="1cc31-112">ConferenceId</span></span>        | <span data-ttu-id="1cc31-113">String</span><span class="sxs-lookup"><span data-stu-id="1cc31-113">String</span></span>  | <span data-ttu-id="1cc31-114">A ID de conferência da reunião online.</span><span class="sxs-lookup"><span data-stu-id="1cc31-114">The conference id of the online meeting.</span></span>      |
| <span data-ttu-id="1cc31-115">tollFreeNumber</span><span class="sxs-lookup"><span data-stu-id="1cc31-115">tollFreeNumber</span></span>      | <span data-ttu-id="1cc31-116">String</span><span class="sxs-lookup"><span data-stu-id="1cc31-116">String</span></span>  | <span data-ttu-id="1cc31-117">O número de chamada gratuita que se conecta ao provedor de conferência de áudio.</span><span class="sxs-lookup"><span data-stu-id="1cc31-117">The toll-free number that connects to the Audio Conference Provider.</span></span>              |
| <span data-ttu-id="1cc31-118">tollNumber</span><span class="sxs-lookup"><span data-stu-id="1cc31-118">tollNumber</span></span>          | <span data-ttu-id="1cc31-119">String</span><span class="sxs-lookup"><span data-stu-id="1cc31-119">String</span></span>  | <span data-ttu-id="1cc31-120">O número de chamada tarifada que se conecta ao provedor de conferência de áudio.</span><span class="sxs-lookup"><span data-stu-id="1cc31-120">The toll number that connects to the Audio Conference Provider.</span></span>                   |

## <a name="json-representation"></a><span data-ttu-id="1cc31-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1cc31-121">JSON representation</span></span>

<span data-ttu-id="1cc31-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1cc31-122">The following is a JSON representation of the resource.</span></span>

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
