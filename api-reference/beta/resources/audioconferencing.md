---
title: tipo de recurso audioConferencing
description: Representa informações de acesso de telefone de uma reunião online.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: ab74b8819cc8dec7d63d5072cee1f1a147accd16
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508119"
---
# <a name="audioconferencing-resource-type"></a><span data-ttu-id="7a2b0-103">tipo de recurso audioConferencing</span><span class="sxs-lookup"><span data-stu-id="7a2b0-103">audioConferencing resource type</span></span>

<span data-ttu-id="7a2b0-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7a2b0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a2b0-105">Representa as informações de acesso de telefone de um [onlineMeeting](onlinemeeting.md).</span><span class="sxs-lookup"><span data-stu-id="7a2b0-105">Represents phone access information for an [onlineMeeting](onlinemeeting.md).</span></span>

## <a name="properties"></a><span data-ttu-id="7a2b0-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7a2b0-106">Properties</span></span>

| <span data-ttu-id="7a2b0-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7a2b0-107">Property</span></span>            | <span data-ttu-id="7a2b0-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="7a2b0-108">Type</span></span>    | <span data-ttu-id="7a2b0-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a2b0-109">Description</span></span>                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="7a2b0-110">dialinUrl</span><span class="sxs-lookup"><span data-stu-id="7a2b0-110">dialinUrl</span></span>           | <span data-ttu-id="7a2b0-111">String</span><span class="sxs-lookup"><span data-stu-id="7a2b0-111">String</span></span>  | <span data-ttu-id="7a2b0-112">Uma URL para a página da Web acessível externamente que contém informações de discagem.</span><span class="sxs-lookup"><span data-stu-id="7a2b0-112">A URL to the externally-accessible web page that contains dial-in information.</span></span> |
| <span data-ttu-id="7a2b0-113">ID</span><span class="sxs-lookup"><span data-stu-id="7a2b0-113">ConferenceId</span></span>        | <span data-ttu-id="7a2b0-114">String</span><span class="sxs-lookup"><span data-stu-id="7a2b0-114">String</span></span>  | <span data-ttu-id="7a2b0-115">A ID de conferência da reunião online.</span><span class="sxs-lookup"><span data-stu-id="7a2b0-115">The conference id of the online meeting.</span></span>      |
| <span data-ttu-id="7a2b0-116">tollFreeNumber</span><span class="sxs-lookup"><span data-stu-id="7a2b0-116">tollFreeNumber</span></span>      | <span data-ttu-id="7a2b0-117">String</span><span class="sxs-lookup"><span data-stu-id="7a2b0-117">String</span></span>  | <span data-ttu-id="7a2b0-118">O número de chamada gratuita que se conecta ao provedor de conferência de áudio.</span><span class="sxs-lookup"><span data-stu-id="7a2b0-118">The toll-free number that connects to the Audio Conference Provider.</span></span>              |
| <span data-ttu-id="7a2b0-119">tollNumber</span><span class="sxs-lookup"><span data-stu-id="7a2b0-119">tollNumber</span></span>          | <span data-ttu-id="7a2b0-120">String</span><span class="sxs-lookup"><span data-stu-id="7a2b0-120">String</span></span>  | <span data-ttu-id="7a2b0-121">O número de chamada tarifada que se conecta ao provedor de conferência de áudio.</span><span class="sxs-lookup"><span data-stu-id="7a2b0-121">The toll number that connects to the Audio Conference Provider.</span></span>                   |

## <a name="json-representation"></a><span data-ttu-id="7a2b0-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7a2b0-122">JSON representation</span></span>

<span data-ttu-id="7a2b0-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7a2b0-123">The following is a JSON representation of the resource.</span></span>

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
