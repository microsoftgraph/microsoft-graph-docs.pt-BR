---
title: tipo de recurso de mailTipsError
description: Um erro que ocorre durante uma ação.
localization_priority: Normal
ms.openlocfilehash: 7df13bb45471d89fdf25b4a251e441bbf2dfad9e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27865621"
---
# <a name="mailtipserror-resource-type"></a><span data-ttu-id="fa991-103">tipo de recurso de mailTipsError</span><span class="sxs-lookup"><span data-stu-id="fa991-103">mailTipsError resource type</span></span>

> <span data-ttu-id="fa991-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fa991-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fa991-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fa991-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fa991-106">Um erro que ocorre durante uma ação.</span><span class="sxs-lookup"><span data-stu-id="fa991-106">An error that occurs during an action.</span></span>

## <a name="properties"></a><span data-ttu-id="fa991-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fa991-107">Properties</span></span>
| <span data-ttu-id="fa991-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fa991-108">Property</span></span>     | <span data-ttu-id="fa991-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="fa991-109">Type</span></span>   |<span data-ttu-id="fa991-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa991-110">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="fa991-111">mensagem</span><span class="sxs-lookup"><span data-stu-id="fa991-111">message</span></span> | <span data-ttu-id="fa991-112">String</span><span class="sxs-lookup"><span data-stu-id="fa991-112">String</span></span> | <span data-ttu-id="fa991-113">A mensagem de erro.</span><span class="sxs-lookup"><span data-stu-id="fa991-113">The error message.</span></span> |
| <span data-ttu-id="fa991-114">código</span><span class="sxs-lookup"><span data-stu-id="fa991-114">code</span></span> | <span data-ttu-id="fa991-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fa991-115">String</span></span> | <span data-ttu-id="fa991-116">O código do erro.</span><span class="sxs-lookup"><span data-stu-id="fa991-116">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fa991-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fa991-117">JSON representation</span></span>

<span data-ttu-id="fa991-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fa991-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mailTipsError"
}-->

```json
{
  "message": "string",
  "code": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailTipsError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
