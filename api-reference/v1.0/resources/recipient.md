---
title: Tipo de recurso recipient
description: 'Representa informações sobre um usuário no envio ou recebimento de um evento, mensagem ou postagem de grupo. '
localization_priority: Normal
ms.openlocfilehash: 89d1ae7703d5b8b0e2a94027e74fbd4c4ebf9ed8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579426"
---
# <a name="recipient-resource-type"></a><span data-ttu-id="1493b-103">Tipo de recurso recipient</span><span class="sxs-lookup"><span data-stu-id="1493b-103">recipient resource type</span></span>

<span data-ttu-id="1493b-104">Representa informações sobre um usuário no envio ou recebimento de um evento, mensagem ou postagem de grupo.</span><span class="sxs-lookup"><span data-stu-id="1493b-104">Represents information about a user in the sending or receiving end of an event, message or group post.</span></span> 

## <a name="properties"></a><span data-ttu-id="1493b-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1493b-105">Properties</span></span>
| <span data-ttu-id="1493b-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1493b-106">Property</span></span>     | <span data-ttu-id="1493b-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="1493b-107">Type</span></span>   |<span data-ttu-id="1493b-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="1493b-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1493b-109">emailAddress</span><span class="sxs-lookup"><span data-stu-id="1493b-109">emailAddress</span></span>|[<span data-ttu-id="1493b-110">EmailAddress</span><span class="sxs-lookup"><span data-stu-id="1493b-110">EmailAddress</span></span>](emailaddress.md)|<span data-ttu-id="1493b-111">O endereço de email do destinatário.</span><span class="sxs-lookup"><span data-stu-id="1493b-111">The recipient's email address.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1493b-112">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1493b-112">JSON representation</span></span>

<span data-ttu-id="1493b-113">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="1493b-113">Here is a JSON representation of the resource</span></span>

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
