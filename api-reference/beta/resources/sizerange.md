---
title: Tipo de recurso sizeRange
description: Especifica os tamanhos mínimo e máximo (em kilobytes) que uma mensagem de entrada deve ter para que a condição ou exceção seja aplicada.
ms.openlocfilehash: c84843116055c8ef13b7961b6ee180c4c896c80f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038656"
---
# <a name="sizerange-resource-type"></a><span data-ttu-id="f3a81-103">Tipo de recurso sizeRange</span><span class="sxs-lookup"><span data-stu-id="f3a81-103">sizeRange resource type</span></span>

> <span data-ttu-id="f3a81-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f3a81-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f3a81-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f3a81-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f3a81-106">Especifica os tamanhos mínimo e máximo (em kilobytes) que uma mensagem de entrada deve ter para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="f3a81-106">Specifies the maximum and minimum sizes (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span>

## <a name="properties"></a><span data-ttu-id="f3a81-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f3a81-107">Properties</span></span>
| <span data-ttu-id="f3a81-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f3a81-108">Property</span></span>     | <span data-ttu-id="f3a81-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f3a81-109">Type</span></span>   |<span data-ttu-id="f3a81-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3a81-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f3a81-111">maximumSize</span><span class="sxs-lookup"><span data-stu-id="f3a81-111">maximumSize</span></span> | <span data-ttu-id="f3a81-112">Int32</span><span class="sxs-lookup"><span data-stu-id="f3a81-112">Int32</span></span> | <span data-ttu-id="f3a81-113">Especifica o tamanho máximo (em kilobytes) que uma mensagem de entrada deve ter para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="f3a81-113">The maximum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |
| <span data-ttu-id="f3a81-114">minimumSize</span><span class="sxs-lookup"><span data-stu-id="f3a81-114">minimumSize</span></span> | <span data-ttu-id="f3a81-115">Int32</span><span class="sxs-lookup"><span data-stu-id="f3a81-115">Int32</span></span> | <span data-ttu-id="f3a81-116">Especifica o tamanho mínimo (em kilobytes) que uma mensagem de entrada deve ter para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="f3a81-116">The minimum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="f3a81-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f3a81-117">JSON representation</span></span>
<span data-ttu-id="f3a81-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f3a81-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.sizeRange"
}-->

```json
{
  "maximumSize": "Int32",
  "minimumSize": "Int32"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sizeRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->