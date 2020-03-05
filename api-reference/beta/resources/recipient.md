---
title: Tipo de recurso recipient
description: 'Representa informações sobre um usuário no envio ou recebimento de um evento, mensagem ou postagem de grupo. '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: e5117517bd9a2d25d5a29de57ab4a5d3c963ca89
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521247"
---
# <a name="recipient-resource-type"></a><span data-ttu-id="9d7db-103">Tipo de recurso recipient</span><span class="sxs-lookup"><span data-stu-id="9d7db-103">recipient resource type</span></span>

<span data-ttu-id="9d7db-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9d7db-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d7db-105">Representa informações sobre um usuário no envio ou recebimento de um evento, mensagem ou postagem de grupo.</span><span class="sxs-lookup"><span data-stu-id="9d7db-105">Represents information about a user in the sending or receiving end of an event, message or group post.</span></span> 

## <a name="properties"></a><span data-ttu-id="9d7db-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9d7db-106">Properties</span></span>
| <span data-ttu-id="9d7db-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9d7db-107">Property</span></span>     | <span data-ttu-id="9d7db-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="9d7db-108">Type</span></span>   |<span data-ttu-id="9d7db-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d7db-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9d7db-110">emailAddress</span><span class="sxs-lookup"><span data-stu-id="9d7db-110">emailAddress</span></span>|[<span data-ttu-id="9d7db-111">EmailAddress</span><span class="sxs-lookup"><span data-stu-id="9d7db-111">EmailAddress</span></span>](emailaddress.md)|<span data-ttu-id="9d7db-112">O endereço de email do destinatário.</span><span class="sxs-lookup"><span data-stu-id="9d7db-112">The recipient's email address.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9d7db-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9d7db-113">JSON representation</span></span>

<span data-ttu-id="9d7db-114">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="9d7db-114">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "recipient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
