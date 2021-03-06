---
title: Tipo de recurso audioConferencing
description: Representa as informações de acesso ao telefone para uma reunião online.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 45ab16c357f8779bdf1a638e1f5a5291eba48e19
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515664"
---
# <a name="audioconferencing-resource-type"></a><span data-ttu-id="d8a9c-103">Tipo de recurso audioConferencing</span><span class="sxs-lookup"><span data-stu-id="d8a9c-103">audioConferencing resource type</span></span>

<span data-ttu-id="d8a9c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8a9c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8a9c-105">Representa as informações de acesso ao telefone para [um onlineMeeting](onlinemeeting.md).</span><span class="sxs-lookup"><span data-stu-id="d8a9c-105">Represents phone access information for an [onlineMeeting](onlinemeeting.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d8a9c-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d8a9c-106">Properties</span></span>

| <span data-ttu-id="d8a9c-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d8a9c-107">Property</span></span>            | <span data-ttu-id="d8a9c-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8a9c-108">Type</span></span>    | <span data-ttu-id="d8a9c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8a9c-109">Description</span></span>                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="d8a9c-110">dialinUrl</span><span class="sxs-lookup"><span data-stu-id="d8a9c-110">dialinUrl</span></span>           | <span data-ttu-id="d8a9c-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8a9c-111">String</span></span>  | <span data-ttu-id="d8a9c-112">Uma URL para a página da Web externamente acessível que contém informações de discagem.</span><span class="sxs-lookup"><span data-stu-id="d8a9c-112">A URL to the externally-accessible web page that contains dial-in information.</span></span> |
| <span data-ttu-id="d8a9c-113">conferenceId</span><span class="sxs-lookup"><span data-stu-id="d8a9c-113">conferenceId</span></span>        | <span data-ttu-id="d8a9c-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8a9c-114">String</span></span>  | <span data-ttu-id="d8a9c-115">A ID da conferência da reunião online.</span><span class="sxs-lookup"><span data-stu-id="d8a9c-115">The conference id of the online meeting.</span></span>      |
| <span data-ttu-id="d8a9c-116">tollFreeNumber</span><span class="sxs-lookup"><span data-stu-id="d8a9c-116">tollFreeNumber</span></span>      | <span data-ttu-id="d8a9c-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8a9c-117">String</span></span>  | <span data-ttu-id="d8a9c-118">O número gratuito que se conecta ao Provedor de Conferência de Áudio.</span><span class="sxs-lookup"><span data-stu-id="d8a9c-118">The toll-free number that connects to the Audio Conference Provider.</span></span>              |
| <span data-ttu-id="d8a9c-119">tollNumber</span><span class="sxs-lookup"><span data-stu-id="d8a9c-119">tollNumber</span></span>          | <span data-ttu-id="d8a9c-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8a9c-120">String</span></span>  | <span data-ttu-id="d8a9c-121">O número de telefone que se conecta ao Provedor de Conferência de Áudio.</span><span class="sxs-lookup"><span data-stu-id="d8a9c-121">The toll number that connects to the Audio Conference Provider.</span></span>                   |

## <a name="json-representation"></a><span data-ttu-id="d8a9c-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d8a9c-122">JSON representation</span></span>

<span data-ttu-id="d8a9c-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d8a9c-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioConferencing"
}-->
```json
{
  "dialinUrl": "String",
  "conferenceId": "String",
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


