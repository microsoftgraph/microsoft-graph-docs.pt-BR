---
title: Tipo de recurso recipient
description: 'Representa informações sobre um usuário no envio ou recebimento de um evento, mensagem ou postagem de grupo. '
localization_priority: Normal
ms.openlocfilehash: 9718d7e6ce09a42e742303aaed484fa6335f3cbc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563193"
---
# <a name="recipient-resource-type"></a><span data-ttu-id="24007-103">Tipo de recurso recipient</span><span class="sxs-lookup"><span data-stu-id="24007-103">recipient resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24007-104">Representa informações sobre um usuário no envio ou recebimento de um evento, mensagem ou postagem de grupo.</span><span class="sxs-lookup"><span data-stu-id="24007-104">Represents information about a user in the sending or receiving end of an event, message or group post.</span></span> 

## <a name="properties"></a><span data-ttu-id="24007-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="24007-105">Properties</span></span>
| <span data-ttu-id="24007-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="24007-106">Property</span></span>     | <span data-ttu-id="24007-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="24007-107">Type</span></span>   |<span data-ttu-id="24007-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="24007-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="24007-109">emailAddress</span><span class="sxs-lookup"><span data-stu-id="24007-109">emailAddress</span></span>|[<span data-ttu-id="24007-110">EmailAddress</span><span class="sxs-lookup"><span data-stu-id="24007-110">EmailAddress</span></span>](emailaddress.md)|<span data-ttu-id="24007-111">O endereço de email do destinatário.</span><span class="sxs-lookup"><span data-stu-id="24007-111">The recipient's email address.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="24007-112">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="24007-112">JSON representation</span></span>

<span data-ttu-id="24007-113">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="24007-113">Here is a JSON representation of the resource</span></span>

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
