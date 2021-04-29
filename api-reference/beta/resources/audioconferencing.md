---
title: Tipo de recurso audioConferencing
description: Representa as informações de acesso ao telefone para uma reunião online.
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 43332de03467b4a5cf9d9cc867718ceafd8c4e82
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080145"
---
# <a name="audioconferencing-resource-type"></a><span data-ttu-id="8e09f-103">Tipo de recurso audioConferencing</span><span class="sxs-lookup"><span data-stu-id="8e09f-103">audioConferencing resource type</span></span>

<span data-ttu-id="8e09f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e09f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e09f-105">Representa as informações de acesso ao telefone para [um onlineMeeting](onlinemeeting.md).</span><span class="sxs-lookup"><span data-stu-id="8e09f-105">Represents phone access information for an [onlineMeeting](onlinemeeting.md).</span></span>

## <a name="properties"></a><span data-ttu-id="8e09f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8e09f-106">Properties</span></span>

| <span data-ttu-id="8e09f-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8e09f-107">Property</span></span>                    | <span data-ttu-id="8e09f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="8e09f-108">Type</span></span>              | <span data-ttu-id="8e09f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e09f-109">Description</span></span>                                                                    |
| :-------------------------- | :---------------- | :----------------------------------------------------------------------------- |
| <span data-ttu-id="8e09f-110">dialinUrl</span><span class="sxs-lookup"><span data-stu-id="8e09f-110">dialinUrl</span></span>                   | <span data-ttu-id="8e09f-111">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="8e09f-111">String</span></span>            | <span data-ttu-id="8e09f-112">Uma URL para a página da Web externamente acessível que contém informações de discagem.</span><span class="sxs-lookup"><span data-stu-id="8e09f-112">A URL to the externally-accessible web page that contains dial-in information.</span></span> |
| <span data-ttu-id="8e09f-113">conferenceId</span><span class="sxs-lookup"><span data-stu-id="8e09f-113">conferenceId</span></span>                | <span data-ttu-id="8e09f-114">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="8e09f-114">String</span></span>            | <span data-ttu-id="8e09f-115">A ID da conferência da reunião online.</span><span class="sxs-lookup"><span data-stu-id="8e09f-115">The conference id of the online meeting.</span></span>                                       |
| <span data-ttu-id="8e09f-116">tollFreeNumber (preterido)</span><span class="sxs-lookup"><span data-stu-id="8e09f-116">tollFreeNumber (deprecated)</span></span> | <span data-ttu-id="8e09f-117">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="8e09f-117">String</span></span>            | <span data-ttu-id="8e09f-118">O número gratuito que se conecta ao Provedor de Conferência de Áudio.</span><span class="sxs-lookup"><span data-stu-id="8e09f-118">The toll-free number that connects to the Audio Conference Provider.</span></span>           |
| <span data-ttu-id="8e09f-119">tollFreeNumbers</span><span class="sxs-lookup"><span data-stu-id="8e09f-119">tollFreeNumbers</span></span>             | <span data-ttu-id="8e09f-120">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8e09f-120">String collection</span></span> | <span data-ttu-id="8e09f-121">Lista de números gratuitos exibidos no convite da reunião.</span><span class="sxs-lookup"><span data-stu-id="8e09f-121">List of toll-free numbers that are displayed in the meeting invite.</span></span>            |
| <span data-ttu-id="8e09f-122">tollNumber (preterido)</span><span class="sxs-lookup"><span data-stu-id="8e09f-122">tollNumber (deprecated)</span></span>     | <span data-ttu-id="8e09f-123">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="8e09f-123">String</span></span>            | <span data-ttu-id="8e09f-124">O número de telefone que se conecta ao Provedor de Conferência de Áudio.</span><span class="sxs-lookup"><span data-stu-id="8e09f-124">The toll number that connects to the Audio Conference Provider.</span></span>                |
| <span data-ttu-id="8e09f-125">tollNumbers</span><span class="sxs-lookup"><span data-stu-id="8e09f-125">tollNumbers</span></span>                 | <span data-ttu-id="8e09f-126">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8e09f-126">String collection</span></span> | <span data-ttu-id="8e09f-127">Lista de números de telefone que são exibidos no convite da reunião.</span><span class="sxs-lookup"><span data-stu-id="8e09f-127">List of toll numbers that are displayed in the meeting invite.</span></span>                 |

> [!CAUTION]
>
>- <span data-ttu-id="8e09f-128">As **propriedades tollFreeNumber** **e tollNumber** são preteridas.</span><span class="sxs-lookup"><span data-stu-id="8e09f-128">The **tollFreeNumber** and **tollNumber** properties are deprecated.</span></span> <span data-ttu-id="8e09f-129">Use as **propriedades tollFreeNumbers** **e tollNumbers.**</span><span class="sxs-lookup"><span data-stu-id="8e09f-129">Use the **tollFreeNumbers** and **tollNumbers** properties instead.</span></span>
>- <span data-ttu-id="8e09f-130">Para compatibilidade com compatibilidade, o **tollFreeNumber** original é adicionado à nova coleção **tollFreeNumbers** e o **tollNumber** original é adicionado à nova coleção **tollNumbers.**</span><span class="sxs-lookup"><span data-stu-id="8e09f-130">For backward compatibility, the original **tollFreeNumber** is added to the new **tollFreeNumbers** collection and the original **tollNumber** is added to the new **tollNumbers** collection.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8e09f-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8e09f-131">JSON representation</span></span>

<span data-ttu-id="8e09f-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8e09f-132">The following is a JSON representation of the resource.</span></span>

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
  "tollFreeNumbers": ["String"],
  "tollNumbers": ["String"]
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


