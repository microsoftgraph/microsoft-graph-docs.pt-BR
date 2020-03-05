---
title: Tipo de recurso SubscribeToToneOperation
description: Descreve o formato de resposta da criação da assinatura para receber tons DTMF.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: e35b3fe674c9f92b7dab723325d658facf13962f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520286"
---
# <a name="subscribetotoneoperation-resource-type"></a><span data-ttu-id="c52c6-103">Tipo de recurso SubscribeToToneOperation</span><span class="sxs-lookup"><span data-stu-id="c52c6-103">SubscribeToToneOperation resource type</span></span>

<span data-ttu-id="c52c6-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c52c6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c52c6-105">Descreve o formato de resposta da criação da assinatura para receber tons DTMF.</span><span class="sxs-lookup"><span data-stu-id="c52c6-105">Describes the response format of creation of subscription to receive DTMF tones.</span></span>

## <a name="properties"></a><span data-ttu-id="c52c6-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c52c6-106">Properties</span></span>

| <span data-ttu-id="c52c6-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c52c6-107">Property</span></span>                       | <span data-ttu-id="c52c6-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="c52c6-108">Type</span></span>                        | <span data-ttu-id="c52c6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c52c6-109">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="c52c6-110">clientContext</span><span class="sxs-lookup"><span data-stu-id="c52c6-110">clientContext</span></span>                  | <span data-ttu-id="c52c6-111">String</span><span class="sxs-lookup"><span data-stu-id="c52c6-111">String</span></span>                      | <span data-ttu-id="c52c6-112">O contexto do cliente.</span><span class="sxs-lookup"><span data-stu-id="c52c6-112">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="c52c6-113">id</span><span class="sxs-lookup"><span data-stu-id="c52c6-113">id</span></span>                             | <span data-ttu-id="c52c6-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c52c6-114">String</span></span>                      | <span data-ttu-id="c52c6-115">A ID da operação do servidor.</span><span class="sxs-lookup"><span data-stu-id="c52c6-115">The server operation ID.</span></span> <span data-ttu-id="c52c6-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c52c6-116">Read-only.</span></span>                                                                                             |
| <span data-ttu-id="c52c6-117">resultInfo</span><span class="sxs-lookup"><span data-stu-id="c52c6-117">resultInfo</span></span>                     | [<span data-ttu-id="c52c6-118">resultInfo</span><span class="sxs-lookup"><span data-stu-id="c52c6-118">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="c52c6-119">As informações de resultado.</span><span class="sxs-lookup"><span data-stu-id="c52c6-119">The result information.</span></span>  <span data-ttu-id="c52c6-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c52c6-120">Read-only.</span></span>                                                                                             |
| <span data-ttu-id="c52c6-121">status</span><span class="sxs-lookup"><span data-stu-id="c52c6-121">status</span></span>                         | <span data-ttu-id="c52c6-122">String</span><span class="sxs-lookup"><span data-stu-id="c52c6-122">String</span></span>                      | <span data-ttu-id="c52c6-123">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="c52c6-123">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="c52c6-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c52c6-124">Read-only.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="c52c6-125">Relações</span><span class="sxs-lookup"><span data-stu-id="c52c6-125">Relationships</span></span>
<span data-ttu-id="c52c6-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c52c6-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c52c6-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c52c6-127">JSON representation</span></span>

<span data-ttu-id="c52c6-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c52c6-128">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.subscribeToToneOperation"
}-->
```json
{
  "clientContext": "String",
  "id": "String (identifier)",
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "notStarted | running | completed | failed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscribeToToneOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
