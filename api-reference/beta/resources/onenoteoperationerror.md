---
title: Tipo de recurso onenoteOperationError
description: Um erro de uma operação do OneNote que falhou.
author: Jewan-microsoft
localization_priority: Normal
ms.openlocfilehash: cfe859bea40f15311a631e8b1d2b3c3a3c179d0c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891529"
---
# <a name="onenoteoperationerror-resource-type"></a><span data-ttu-id="97df7-103">Tipo de recurso onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="97df7-103">onenoteOperationError resource type</span></span>

> <span data-ttu-id="97df7-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="97df7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="97df7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="97df7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="97df7-106">Um erro de uma operação do OneNote que falhou.</span><span class="sxs-lookup"><span data-stu-id="97df7-106">An error from a failed OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="97df7-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="97df7-107">JSON representation</span></span>

<span data-ttu-id="97df7-108">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="97df7-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteOperationError"
}-->

```json
{
  "code": "string",
  "message": "string"
}

```
## <a name="properties"></a><span data-ttu-id="97df7-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="97df7-109">Properties</span></span>
| <span data-ttu-id="97df7-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="97df7-110">Property</span></span>     | <span data-ttu-id="97df7-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="97df7-111">Type</span></span>   |<span data-ttu-id="97df7-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="97df7-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="97df7-113">código</span><span class="sxs-lookup"><span data-stu-id="97df7-113">code</span></span>|<span data-ttu-id="97df7-114">string</span><span class="sxs-lookup"><span data-stu-id="97df7-114">string</span></span>|<span data-ttu-id="97df7-115">O código do erro.</span><span class="sxs-lookup"><span data-stu-id="97df7-115">The error code.</span></span>|
|<span data-ttu-id="97df7-116">message</span><span class="sxs-lookup"><span data-stu-id="97df7-116">message</span></span>|<span data-ttu-id="97df7-117">string</span><span class="sxs-lookup"><span data-stu-id="97df7-117">string</span></span>|<span data-ttu-id="97df7-118">A mensagem de erro.</span><span class="sxs-lookup"><span data-stu-id="97df7-118">The error message.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
