---
title: Tipo de recurso recipient
description: 'Representa informações sobre um usuário no envio ou recebimento de um evento, mensagem ou postagem de grupo. '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: abheek-das
ms.openlocfilehash: 7a0f48eecdca77bda7261ed85b3b962550d99ec0
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133183"
---
# <a name="recipient-resource-type"></a><span data-ttu-id="9e153-103">Tipo de recurso recipient</span><span class="sxs-lookup"><span data-stu-id="9e153-103">recipient resource type</span></span>

<span data-ttu-id="9e153-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e153-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e153-105">Representa informações sobre um usuário no envio ou recebimento de um evento, mensagem ou postagem de grupo.</span><span class="sxs-lookup"><span data-stu-id="9e153-105">Represents information about a user in the sending or receiving end of an event, message or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="9e153-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9e153-106">Properties</span></span>
| <span data-ttu-id="9e153-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9e153-107">Property</span></span>     | <span data-ttu-id="9e153-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="9e153-108">Type</span></span>   |<span data-ttu-id="9e153-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e153-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9e153-110">emailAddress</span><span class="sxs-lookup"><span data-stu-id="9e153-110">emailAddress</span></span>|[<span data-ttu-id="9e153-111">EmailAddress</span><span class="sxs-lookup"><span data-stu-id="9e153-111">EmailAddress</span></span>](emailaddress.md)|<span data-ttu-id="9e153-112">O endereço de email do destinatário.</span><span class="sxs-lookup"><span data-stu-id="9e153-112">The recipient's email address.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9e153-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9e153-113">JSON representation</span></span>

<span data-ttu-id="9e153-114">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="9e153-114">Here is a JSON representation of the resource</span></span>

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


