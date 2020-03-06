---
title: Tipo de recurso SubscribeToToneOperation
description: Descreve o formato de resposta da criação da assinatura para receber tons DTMF.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: f29d385060d93b8de54ee27f9f948f83e3ad2711
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533617"
---
# <a name="subscribetotoneoperation-resource-type"></a><span data-ttu-id="434ac-103">Tipo de recurso SubscribeToToneOperation</span><span class="sxs-lookup"><span data-stu-id="434ac-103">SubscribeToToneOperation resource type</span></span>

<span data-ttu-id="434ac-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="434ac-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="434ac-105">Descreve o formato de resposta da criação da assinatura para receber tons DTMF.</span><span class="sxs-lookup"><span data-stu-id="434ac-105">Describes the response format of creation of subscription to receive DTMF tones.</span></span>

## <a name="properties"></a><span data-ttu-id="434ac-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="434ac-106">Properties</span></span>

| <span data-ttu-id="434ac-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="434ac-107">Property</span></span>                       | <span data-ttu-id="434ac-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="434ac-108">Type</span></span>                        | <span data-ttu-id="434ac-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="434ac-109">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="434ac-110">clientContext</span><span class="sxs-lookup"><span data-stu-id="434ac-110">clientContext</span></span>                  | <span data-ttu-id="434ac-111">String</span><span class="sxs-lookup"><span data-stu-id="434ac-111">String</span></span>                      | <span data-ttu-id="434ac-112">O contexto do cliente.</span><span class="sxs-lookup"><span data-stu-id="434ac-112">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="434ac-113">id</span><span class="sxs-lookup"><span data-stu-id="434ac-113">id</span></span>                             | <span data-ttu-id="434ac-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="434ac-114">String</span></span>                      | <span data-ttu-id="434ac-115">A ID da operação do servidor.</span><span class="sxs-lookup"><span data-stu-id="434ac-115">The server operation ID.</span></span> <span data-ttu-id="434ac-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="434ac-116">Read-only.</span></span>                                                                                             |
| <span data-ttu-id="434ac-117">status</span><span class="sxs-lookup"><span data-stu-id="434ac-117">status</span></span>                         | <span data-ttu-id="434ac-118">String</span><span class="sxs-lookup"><span data-stu-id="434ac-118">String</span></span>                      | <span data-ttu-id="434ac-119">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="434ac-119">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="434ac-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="434ac-120">Read-only.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="434ac-121">Relações</span><span class="sxs-lookup"><span data-stu-id="434ac-121">Relationships</span></span>
<span data-ttu-id="434ac-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="434ac-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="434ac-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="434ac-123">JSON representation</span></span>

<span data-ttu-id="434ac-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="434ac-124">The following is a JSON representation of the resource.</span></span>

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
