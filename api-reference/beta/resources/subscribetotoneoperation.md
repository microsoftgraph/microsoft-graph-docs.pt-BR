---
title: Tipo de recurso SubscribeToToneOperation
description: Descreve o formato de resposta da criação da assinatura para receber tons DTMF.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 9f3a2f9cc3e32fd6455e2d692d4d4df2e9d502ac
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006533"
---
# <a name="subscribetotoneoperation-resource-type"></a><span data-ttu-id="e99ac-103">Tipo de recurso SubscribeToToneOperation</span><span class="sxs-lookup"><span data-stu-id="e99ac-103">SubscribeToToneOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e99ac-104">Descreve o formato de resposta da criação da assinatura para receber tons DTMF.</span><span class="sxs-lookup"><span data-stu-id="e99ac-104">Describes the response format of creation of subscription to receive DTMF tones.</span></span>

## <a name="properties"></a><span data-ttu-id="e99ac-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e99ac-105">Properties</span></span>

| <span data-ttu-id="e99ac-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e99ac-106">Property</span></span>                       | <span data-ttu-id="e99ac-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="e99ac-107">Type</span></span>                        | <span data-ttu-id="e99ac-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="e99ac-108">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="e99ac-109">clientContext</span><span class="sxs-lookup"><span data-stu-id="e99ac-109">clientContext</span></span>                  | <span data-ttu-id="e99ac-110">String</span><span class="sxs-lookup"><span data-stu-id="e99ac-110">String</span></span>                      | <span data-ttu-id="e99ac-111">O contexto do cliente.</span><span class="sxs-lookup"><span data-stu-id="e99ac-111">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="e99ac-112">id</span><span class="sxs-lookup"><span data-stu-id="e99ac-112">id</span></span>                             | <span data-ttu-id="e99ac-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e99ac-113">String</span></span>                      | <span data-ttu-id="e99ac-114">A ID da operação do servidor.</span><span class="sxs-lookup"><span data-stu-id="e99ac-114">The server operation ID.</span></span> <span data-ttu-id="e99ac-115">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e99ac-115">Read-only.</span></span>                                                                                             |
| <span data-ttu-id="e99ac-116">resultInfo</span><span class="sxs-lookup"><span data-stu-id="e99ac-116">resultInfo</span></span>                     | [<span data-ttu-id="e99ac-117">resultInfo</span><span class="sxs-lookup"><span data-stu-id="e99ac-117">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="e99ac-118">As informações de resultado.</span><span class="sxs-lookup"><span data-stu-id="e99ac-118">The result information.</span></span>  <span data-ttu-id="e99ac-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e99ac-119">Read-only.</span></span>                                                                                             |
| <span data-ttu-id="e99ac-120">status</span><span class="sxs-lookup"><span data-stu-id="e99ac-120">status</span></span>                         | <span data-ttu-id="e99ac-121">String</span><span class="sxs-lookup"><span data-stu-id="e99ac-121">String</span></span>                      | <span data-ttu-id="e99ac-122">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="e99ac-122">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="e99ac-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e99ac-123">Read-only.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="e99ac-124">Relações</span><span class="sxs-lookup"><span data-stu-id="e99ac-124">Relationships</span></span>
<span data-ttu-id="e99ac-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e99ac-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e99ac-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e99ac-126">JSON representation</span></span>

<span data-ttu-id="e99ac-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e99ac-127">The following is a JSON representation of the resource.</span></span>

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
