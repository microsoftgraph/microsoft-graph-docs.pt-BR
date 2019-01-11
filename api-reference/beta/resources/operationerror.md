---
title: tipo de recurso de operationError
description: Descreve os erros em teamsAsyncOperation.
localization_priority: Normal
ms.openlocfilehash: 423f426df92e99754af0abf4c9c8088eea61d5ea
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890290"
---
# <a name="operationerror-resource-type"></a><span data-ttu-id="3c695-103">tipo de recurso de operationError</span><span class="sxs-lookup"><span data-stu-id="3c695-103">operationError resource type</span></span>

> <span data-ttu-id="3c695-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3c695-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3c695-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3c695-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3c695-106">Descreve os erros em [teamsAsyncOperation](teamsasyncoperation.md).</span><span class="sxs-lookup"><span data-stu-id="3c695-106">Describes errors in [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="operationerror-properties"></a><span data-ttu-id="3c695-107">Propriedades de operationError</span><span class="sxs-lookup"><span data-stu-id="3c695-107">operationError Properties</span></span>
| <span data-ttu-id="3c695-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3c695-108">Property</span></span>     | <span data-ttu-id="3c695-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="3c695-109">Type</span></span>   |<span data-ttu-id="3c695-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c695-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3c695-111">código</span><span class="sxs-lookup"><span data-stu-id="3c695-111">code</span></span>|<span data-ttu-id="3c695-112">cadeia de caracteres (somente leitura)</span><span class="sxs-lookup"><span data-stu-id="3c695-112">string (readonly)</span></span>|<span data-ttu-id="3c695-113">Código de erro de operação.</span><span class="sxs-lookup"><span data-stu-id="3c695-113">Operation error code.</span></span>|
|<span data-ttu-id="3c695-114">message</span><span class="sxs-lookup"><span data-stu-id="3c695-114">message</span></span>|<span data-ttu-id="3c695-115">cadeia de caracteres (somente leitura)</span><span class="sxs-lookup"><span data-stu-id="3c695-115">string (readonly)</span></span>|<span data-ttu-id="3c695-116">Mensagem de erro de operação.</span><span class="sxs-lookup"><span data-stu-id="3c695-116">Operation error message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3c695-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3c695-117">JSON representation</span></span>

<span data-ttu-id="3c695-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3c695-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.operationError"
}-->

```json
{
    "code": "TeamUnavailable",
    "message": "The team was not found."
}
```

<!-- uuid: 069fadaa-52db-4ced-85d5-74f7caa2c66f
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "operation error resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
