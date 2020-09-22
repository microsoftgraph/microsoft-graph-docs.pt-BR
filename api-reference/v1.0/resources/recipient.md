---
title: Tipo de recurso recipient
description: 'Representa informações sobre um usuário no envio ou recebimento de um evento, mensagem ou postagem de grupo. '
localization_priority: Normal
author: svpsiva
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: ef7f459fd345992cb51e8c3ac2742146648772dc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078987"
---
# <a name="recipient-resource-type"></a><span data-ttu-id="b7fc9-103">Tipo de recurso recipient</span><span class="sxs-lookup"><span data-stu-id="b7fc9-103">recipient resource type</span></span>

<span data-ttu-id="b7fc9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7fc9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b7fc9-105">Representa informações sobre um usuário no envio ou recebimento de um evento, mensagem ou postagem de grupo.</span><span class="sxs-lookup"><span data-stu-id="b7fc9-105">Represents information about a user in the sending or receiving end of an event, message or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="b7fc9-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b7fc9-106">Properties</span></span>
| <span data-ttu-id="b7fc9-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b7fc9-107">Property</span></span>     | <span data-ttu-id="b7fc9-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b7fc9-108">Type</span></span>   |<span data-ttu-id="b7fc9-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7fc9-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b7fc9-110">emailAddress</span><span class="sxs-lookup"><span data-stu-id="b7fc9-110">emailAddress</span></span>|[<span data-ttu-id="b7fc9-111">EmailAddress</span><span class="sxs-lookup"><span data-stu-id="b7fc9-111">EmailAddress</span></span>](emailaddress.md)|<span data-ttu-id="b7fc9-112">O endereço de email do destinatário.</span><span class="sxs-lookup"><span data-stu-id="b7fc9-112">The recipient's email address.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b7fc9-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b7fc9-113">JSON representation</span></span>

<span data-ttu-id="b7fc9-114">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="b7fc9-114">Here is a JSON representation of the resource</span></span>

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

