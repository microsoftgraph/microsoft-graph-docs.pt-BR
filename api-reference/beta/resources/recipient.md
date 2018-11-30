---
title: Tipo de recurso recipient
description: 'Representa informações sobre um usuário no envio ou recebimento de um evento, mensagem ou postagem de grupo. '
ms.openlocfilehash: 2ecf92f314c8b29da529b8dc07cada71dd8571f2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038881"
---
# <a name="recipient-resource-type"></a><span data-ttu-id="ffe9e-103">Tipo de recurso recipient</span><span class="sxs-lookup"><span data-stu-id="ffe9e-103">recipient resource type</span></span>

> <span data-ttu-id="ffe9e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ffe9e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ffe9e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ffe9e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ffe9e-106">Representa informações sobre um usuário no envio ou recebimento de um evento, mensagem ou postagem de grupo.</span><span class="sxs-lookup"><span data-stu-id="ffe9e-106">Represents information about a user in the sending or receiving end of an event, message or group post.</span></span> 

## <a name="properties"></a><span data-ttu-id="ffe9e-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ffe9e-107">Properties</span></span>
| <span data-ttu-id="ffe9e-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ffe9e-108">Property</span></span>     | <span data-ttu-id="ffe9e-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ffe9e-109">Type</span></span>   |<span data-ttu-id="ffe9e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ffe9e-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ffe9e-111">emailAddress</span><span class="sxs-lookup"><span data-stu-id="ffe9e-111">emailAddress</span></span>|[<span data-ttu-id="ffe9e-112">EmailAddress</span><span class="sxs-lookup"><span data-stu-id="ffe9e-112">EmailAddress</span></span>](emailaddress.md)|<span data-ttu-id="ffe9e-113">O endereço de email do destinatário.</span><span class="sxs-lookup"><span data-stu-id="ffe9e-113">The recipient's email address.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ffe9e-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ffe9e-114">JSON representation</span></span>

<span data-ttu-id="ffe9e-115">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="ffe9e-115">Here is a JSON representation of the resource</span></span>

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