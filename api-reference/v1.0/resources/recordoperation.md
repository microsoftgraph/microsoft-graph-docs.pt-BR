---
title: tipo de recurso recordOperation
description: Esse tipo de recurso contém informações relacionadas à gravação de áudio.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 508404a3360b2b59656dc31df6ec44f16f682cf4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991891"
---
# <a name="recordoperation-resource-type"></a><span data-ttu-id="29353-103">tipo de recurso recordOperation</span><span class="sxs-lookup"><span data-stu-id="29353-103">recordOperation resource type</span></span>

<span data-ttu-id="29353-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29353-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="29353-105">Esse tipo de recurso contém informações relacionadas à gravação de áudio.</span><span class="sxs-lookup"><span data-stu-id="29353-105">This resource type contains information related to audio recording.</span></span>

## <a name="properties"></a><span data-ttu-id="29353-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="29353-106">Properties</span></span>

| <span data-ttu-id="29353-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="29353-107">Property</span></span>                       | <span data-ttu-id="29353-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="29353-108">Type</span></span>                        | <span data-ttu-id="29353-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="29353-109">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="29353-110">clientContext</span><span class="sxs-lookup"><span data-stu-id="29353-110">clientContext</span></span>                  | <span data-ttu-id="29353-111">String</span><span class="sxs-lookup"><span data-stu-id="29353-111">String</span></span>                      | <span data-ttu-id="29353-112">Cadeia de caracteres de contexto de cliente exclusivo.</span><span class="sxs-lookup"><span data-stu-id="29353-112">Unique Client Context string.</span></span> <span data-ttu-id="29353-113">O limite máximo é de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="29353-113">Max limit is 256 chars.</span></span>                                                                                                                               |
| <span data-ttu-id="29353-114">id</span><span class="sxs-lookup"><span data-stu-id="29353-114">id</span></span>                             | <span data-ttu-id="29353-115">String</span><span class="sxs-lookup"><span data-stu-id="29353-115">String</span></span>                      | <span data-ttu-id="29353-116">A ID da operação do servidor. somente leitura.</span><span class="sxs-lookup"><span data-stu-id="29353-116">The server operation id. Read-only.</span></span>                                                                                              |
| <span data-ttu-id="29353-117">recordingAccessToken</span><span class="sxs-lookup"><span data-stu-id="29353-117">recordingAccessToken</span></span>           | <span data-ttu-id="29353-118">String</span><span class="sxs-lookup"><span data-stu-id="29353-118">String</span></span>                      | <span data-ttu-id="29353-119">O token de acesso necessário para recuperar a gravação.</span><span class="sxs-lookup"><span data-stu-id="29353-119">The access token required to retrieve the recording.</span></span>                                                                                              |
| <span data-ttu-id="29353-120">recordingLocation</span><span class="sxs-lookup"><span data-stu-id="29353-120">recordingLocation</span></span>              | <span data-ttu-id="29353-121">String</span><span class="sxs-lookup"><span data-stu-id="29353-121">String</span></span>                      | <span data-ttu-id="29353-122">O local onde a gravação está localizada.</span><span class="sxs-lookup"><span data-stu-id="29353-122">The location where the recording is located.</span></span>                                                                                                      |
| <span data-ttu-id="29353-123">resultInfo</span><span class="sxs-lookup"><span data-stu-id="29353-123">resultInfo</span></span>                     | [<span data-ttu-id="29353-124">resultInfo</span><span class="sxs-lookup"><span data-stu-id="29353-124">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="29353-125">As informações de resultado.</span><span class="sxs-lookup"><span data-stu-id="29353-125">The result information.</span></span>  <span data-ttu-id="29353-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="29353-126">Read-only.</span></span>                                                                                              |
| <span data-ttu-id="29353-127">status</span><span class="sxs-lookup"><span data-stu-id="29353-127">status</span></span>                         | <span data-ttu-id="29353-128">String</span><span class="sxs-lookup"><span data-stu-id="29353-128">String</span></span>                      | <span data-ttu-id="29353-129">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="29353-129">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="29353-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="29353-130">Read-only.</span></span>                                                |

## <a name="relationships"></a><span data-ttu-id="29353-131">Relações</span><span class="sxs-lookup"><span data-stu-id="29353-131">Relationships</span></span>
<span data-ttu-id="29353-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="29353-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="29353-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="29353-133">JSON representation</span></span>

<span data-ttu-id="29353-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="29353-134">The following is a JSON representation of the resource.</span></span>

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

