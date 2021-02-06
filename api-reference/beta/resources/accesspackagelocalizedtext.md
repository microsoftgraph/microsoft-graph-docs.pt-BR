---
title: Tipo de recurso accessPackageLocalizedText
description: Um tipo complexo usado para representar uma cadeia de caracteres em um idioma específico.
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8d493f0909617dcda26546ccc262d7591c6b9309
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137344"
---
# <a name="accesspackagelocalizedtext-resource-type"></a><span data-ttu-id="6d98d-103">Tipo de recurso accessPackageLocalizedText</span><span class="sxs-lookup"><span data-stu-id="6d98d-103">accessPackageLocalizedText resource type</span></span>

<span data-ttu-id="6d98d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d98d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d98d-105">Um tipo complexo usado para representar uma cadeia de caracteres em um idioma específico.</span><span class="sxs-lookup"><span data-stu-id="6d98d-105">A complex type used to represent a string in a specific language.</span></span>

## <a name="properties"></a><span data-ttu-id="6d98d-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6d98d-106">Properties</span></span>
|<span data-ttu-id="6d98d-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6d98d-107">Property</span></span>|<span data-ttu-id="6d98d-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d98d-108">Type</span></span>|<span data-ttu-id="6d98d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d98d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d98d-110">languageCode</span><span class="sxs-lookup"><span data-stu-id="6d98d-110">languageCode</span></span>|<span data-ttu-id="6d98d-111">String</span><span class="sxs-lookup"><span data-stu-id="6d98d-111">String</span></span>|<span data-ttu-id="6d98d-112">O código ISO para o idioma pretendido.</span><span class="sxs-lookup"><span data-stu-id="6d98d-112">The ISO code for the intended language.</span></span> <span data-ttu-id="6d98d-113">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6d98d-113">Required.</span></span> |
|<span data-ttu-id="6d98d-114">texto</span><span class="sxs-lookup"><span data-stu-id="6d98d-114">text</span></span>|<span data-ttu-id="6d98d-115">String</span><span class="sxs-lookup"><span data-stu-id="6d98d-115">String</span></span>|<span data-ttu-id="6d98d-116">O texto no idioma específico.</span><span class="sxs-lookup"><span data-stu-id="6d98d-116">The text in the specific language.</span></span> <span data-ttu-id="6d98d-117">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6d98d-117">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="6d98d-118">Relações</span><span class="sxs-lookup"><span data-stu-id="6d98d-118">Relationships</span></span>
<span data-ttu-id="6d98d-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6d98d-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6d98d-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6d98d-120">JSON representation</span></span>
<span data-ttu-id="6d98d-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6d98d-121">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageLocalizedText"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageLocalizedText",
  "text": "String",
  "languageCode": "String"
}
```
