---
title: Tipo de recurso SubscribeToToneOperation
description: Descreve o formato de resposta da criação da assinatura para receber tons DTMF.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 6d1e42d375dd53fcb71ae049622c59d2d31b3406
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913538"
---
# <a name="subscribetotoneoperation-resource-type"></a><span data-ttu-id="1e8e5-103">Tipo de recurso SubscribeToToneOperation</span><span class="sxs-lookup"><span data-stu-id="1e8e5-103">SubscribeToToneOperation resource type</span></span>

<span data-ttu-id="1e8e5-104">Descreve o formato de resposta da criação da assinatura para receber tons DTMF.</span><span class="sxs-lookup"><span data-stu-id="1e8e5-104">Describes the response format of creation of subscription to receive DTMF tones.</span></span>

## <a name="properties"></a><span data-ttu-id="1e8e5-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1e8e5-105">Properties</span></span>

| <span data-ttu-id="1e8e5-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1e8e5-106">Property</span></span>                       | <span data-ttu-id="1e8e5-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="1e8e5-107">Type</span></span>                        | <span data-ttu-id="1e8e5-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e8e5-108">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="1e8e5-109">clientContext</span><span class="sxs-lookup"><span data-stu-id="1e8e5-109">clientContext</span></span>                  | <span data-ttu-id="1e8e5-110">String</span><span class="sxs-lookup"><span data-stu-id="1e8e5-110">String</span></span>                      | <span data-ttu-id="1e8e5-111">O contexto do cliente.</span><span class="sxs-lookup"><span data-stu-id="1e8e5-111">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="1e8e5-112">id</span><span class="sxs-lookup"><span data-stu-id="1e8e5-112">id</span></span>                             | <span data-ttu-id="1e8e5-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e8e5-113">String</span></span>                      | <span data-ttu-id="1e8e5-114">A ID da operação do servidor.</span><span class="sxs-lookup"><span data-stu-id="1e8e5-114">The server operation ID.</span></span> <span data-ttu-id="1e8e5-115">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1e8e5-115">Read-only.</span></span>                                                                                             |
| <span data-ttu-id="1e8e5-116">status</span><span class="sxs-lookup"><span data-stu-id="1e8e5-116">status</span></span>                         | <span data-ttu-id="1e8e5-117">String</span><span class="sxs-lookup"><span data-stu-id="1e8e5-117">String</span></span>                      | <span data-ttu-id="1e8e5-118">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="1e8e5-118">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="1e8e5-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1e8e5-119">Read-only.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="1e8e5-120">Relações</span><span class="sxs-lookup"><span data-stu-id="1e8e5-120">Relationships</span></span>
<span data-ttu-id="1e8e5-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1e8e5-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1e8e5-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1e8e5-122">JSON representation</span></span>

<span data-ttu-id="1e8e5-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1e8e5-123">The following is a JSON representation of the resource.</span></span>

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
