---
title: Tipo de recurso recipient
description: 'Representa informações sobre um usuário no envio ou recebimento de um evento, mensagem ou postagem de grupo. '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: svpsiva
ms.openlocfilehash: ccd210eeecd84acf8094f7a55b1733e64c4a5437
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810465"
---
# <a name="recipient-resource-type"></a><span data-ttu-id="29601-103">Tipo de recurso recipient</span><span class="sxs-lookup"><span data-stu-id="29601-103">recipient resource type</span></span>

<span data-ttu-id="29601-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29601-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29601-105">Representa informações sobre um usuário no envio ou recebimento de um evento, mensagem ou postagem de grupo.</span><span class="sxs-lookup"><span data-stu-id="29601-105">Represents information about a user in the sending or receiving end of an event, message or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="29601-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="29601-106">Properties</span></span>
| <span data-ttu-id="29601-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="29601-107">Property</span></span>     | <span data-ttu-id="29601-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="29601-108">Type</span></span>   |<span data-ttu-id="29601-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="29601-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="29601-110">emailAddress</span><span class="sxs-lookup"><span data-stu-id="29601-110">emailAddress</span></span>|[<span data-ttu-id="29601-111">EmailAddress</span><span class="sxs-lookup"><span data-stu-id="29601-111">EmailAddress</span></span>](emailaddress.md)|<span data-ttu-id="29601-112">O endereço de email do destinatário.</span><span class="sxs-lookup"><span data-stu-id="29601-112">The recipient's email address.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="29601-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="29601-113">JSON representation</span></span>

<span data-ttu-id="29601-114">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="29601-114">Here is a JSON representation of the resource</span></span>

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
