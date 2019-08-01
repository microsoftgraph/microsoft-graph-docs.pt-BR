---
title: Tipo de recurso recipient
description: 'Representa informações sobre um usuário no envio ou recebimento de um evento, mensagem ou postagem de grupo. '
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 9cce3b701965b819d82fc25a28da7e2627c1e2b9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034822"
---
# <a name="recipient-resource-type"></a><span data-ttu-id="038a6-103">Tipo de recurso recipient</span><span class="sxs-lookup"><span data-stu-id="038a6-103">recipient resource type</span></span>

<span data-ttu-id="038a6-104">Representa informações sobre um usuário no envio ou recebimento de um evento, mensagem ou postagem de grupo.</span><span class="sxs-lookup"><span data-stu-id="038a6-104">Represents information about a user in the sending or receiving end of an event, message or group post.</span></span> 

## <a name="properties"></a><span data-ttu-id="038a6-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="038a6-105">Properties</span></span>
| <span data-ttu-id="038a6-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="038a6-106">Property</span></span>     | <span data-ttu-id="038a6-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="038a6-107">Type</span></span>   |<span data-ttu-id="038a6-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="038a6-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="038a6-109">emailAddress</span><span class="sxs-lookup"><span data-stu-id="038a6-109">emailAddress</span></span>|[<span data-ttu-id="038a6-110">EmailAddress</span><span class="sxs-lookup"><span data-stu-id="038a6-110">EmailAddress</span></span>](emailaddress.md)|<span data-ttu-id="038a6-111">O endereço de email do destinatário.</span><span class="sxs-lookup"><span data-stu-id="038a6-111">The recipient's email address.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="038a6-112">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="038a6-112">JSON representation</span></span>

<span data-ttu-id="038a6-113">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="038a6-113">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recipient"
}-->

```json
{
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recipient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
