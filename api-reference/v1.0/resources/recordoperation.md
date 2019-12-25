---
title: tipo de recurso recordOperation
description: Esse tipo de recurso contém informações relacionadas à gravação de áudio.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: b4f0a62204a6ee1db7e75caf9044288f705a5529
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865646"
---
# <a name="recordoperation-resource-type"></a><span data-ttu-id="0ddec-103">tipo de recurso recordOperation</span><span class="sxs-lookup"><span data-stu-id="0ddec-103">recordOperation resource type</span></span>

<span data-ttu-id="0ddec-104">Esse tipo de recurso contém informações relacionadas à gravação de áudio.</span><span class="sxs-lookup"><span data-stu-id="0ddec-104">This resource type contains information related to audio recording.</span></span>

## <a name="properties"></a><span data-ttu-id="0ddec-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0ddec-105">Properties</span></span>

| <span data-ttu-id="0ddec-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0ddec-106">Property</span></span>                       | <span data-ttu-id="0ddec-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ddec-107">Type</span></span>                        | <span data-ttu-id="0ddec-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ddec-108">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="0ddec-109">clientContext</span><span class="sxs-lookup"><span data-stu-id="0ddec-109">clientContext</span></span>                  | <span data-ttu-id="0ddec-110">String</span><span class="sxs-lookup"><span data-stu-id="0ddec-110">String</span></span>                      | <span data-ttu-id="0ddec-111">Cadeia de caracteres de contexto de cliente exclusivo.</span><span class="sxs-lookup"><span data-stu-id="0ddec-111">Unique Client Context string.</span></span> <span data-ttu-id="0ddec-112">O limite máximo é de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="0ddec-112">Max limit is 256 chars.</span></span>                                                                                                                               |
| <span data-ttu-id="0ddec-113">id</span><span class="sxs-lookup"><span data-stu-id="0ddec-113">id</span></span>                             | <span data-ttu-id="0ddec-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0ddec-114">String</span></span>                      | <span data-ttu-id="0ddec-115">A ID da operação do servidor. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0ddec-115">The server operation id. Read-only.</span></span>                                                                                              |
| <span data-ttu-id="0ddec-116">recordingAccessToken</span><span class="sxs-lookup"><span data-stu-id="0ddec-116">recordingAccessToken</span></span>           | <span data-ttu-id="0ddec-117">String</span><span class="sxs-lookup"><span data-stu-id="0ddec-117">String</span></span>                      | <span data-ttu-id="0ddec-118">O token de acesso necessário para recuperar a gravação.</span><span class="sxs-lookup"><span data-stu-id="0ddec-118">The access token required to retrieve the recording.</span></span>                                                                                              |
| <span data-ttu-id="0ddec-119">recordingLocation</span><span class="sxs-lookup"><span data-stu-id="0ddec-119">recordingLocation</span></span>              | <span data-ttu-id="0ddec-120">String</span><span class="sxs-lookup"><span data-stu-id="0ddec-120">String</span></span>                      | <span data-ttu-id="0ddec-121">O local onde a gravação está localizada.</span><span class="sxs-lookup"><span data-stu-id="0ddec-121">The location where the recording is located.</span></span>                                                                                                      |
| <span data-ttu-id="0ddec-122">resultInfo</span><span class="sxs-lookup"><span data-stu-id="0ddec-122">resultInfo</span></span>                     | [<span data-ttu-id="0ddec-123">resultInfo</span><span class="sxs-lookup"><span data-stu-id="0ddec-123">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="0ddec-124">As informações de resultado.</span><span class="sxs-lookup"><span data-stu-id="0ddec-124">The result information.</span></span>  <span data-ttu-id="0ddec-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0ddec-125">Read-only.</span></span>                                                                                              |
| <span data-ttu-id="0ddec-126">status</span><span class="sxs-lookup"><span data-stu-id="0ddec-126">status</span></span>                         | <span data-ttu-id="0ddec-127">String</span><span class="sxs-lookup"><span data-stu-id="0ddec-127">String</span></span>                      | <span data-ttu-id="0ddec-128">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="0ddec-128">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="0ddec-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0ddec-129">Read-only.</span></span>                                                |

## <a name="relationships"></a><span data-ttu-id="0ddec-130">Relações</span><span class="sxs-lookup"><span data-stu-id="0ddec-130">Relationships</span></span>
<span data-ttu-id="0ddec-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0ddec-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0ddec-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0ddec-132">JSON representation</span></span>

<span data-ttu-id="0ddec-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0ddec-133">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recordOperation"
}-->
```json
{
  "clientContext": "String",
  "id": "String (identifier)",
  "recordingAccessToken": "String",
  "recordingLocation": "String",
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "notStarted | running | completed | failed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "recordOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
