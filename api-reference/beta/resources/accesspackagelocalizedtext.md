---
title: tipo de recurso accessPackageLocalizedText
description: Um tipo complexo usado para representar uma cadeia de caracteres em um idioma específico.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9573ae4118f02abdba5686fd94da96da71d374c2
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720070"
---
# <a name="accesspackagelocalizedtext-resource-type"></a><span data-ttu-id="fa69c-103">tipo de recurso accessPackageLocalizedText</span><span class="sxs-lookup"><span data-stu-id="fa69c-103">accessPackageLocalizedText resource type</span></span>

<span data-ttu-id="fa69c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa69c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa69c-105">Um tipo complexo usado para representar uma cadeia de caracteres em um idioma específico.</span><span class="sxs-lookup"><span data-stu-id="fa69c-105">A complex type used to represent a string in a specific language.</span></span>

## <a name="properties"></a><span data-ttu-id="fa69c-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fa69c-106">Properties</span></span>
|<span data-ttu-id="fa69c-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fa69c-107">Property</span></span>|<span data-ttu-id="fa69c-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="fa69c-108">Type</span></span>|<span data-ttu-id="fa69c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa69c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa69c-110">Campo</span><span class="sxs-lookup"><span data-stu-id="fa69c-110">languageCode</span></span>|<span data-ttu-id="fa69c-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fa69c-111">String</span></span>|<span data-ttu-id="fa69c-112">O código ISO do idioma desejado.</span><span class="sxs-lookup"><span data-stu-id="fa69c-112">The ISO code for the intended language.</span></span> <span data-ttu-id="fa69c-113">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fa69c-113">Required.</span></span> |
|<span data-ttu-id="fa69c-114">texto</span><span class="sxs-lookup"><span data-stu-id="fa69c-114">text</span></span>|<span data-ttu-id="fa69c-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fa69c-115">String</span></span>|<span data-ttu-id="fa69c-116">O texto no idioma específico.</span><span class="sxs-lookup"><span data-stu-id="fa69c-116">The text in the specific language.</span></span> <span data-ttu-id="fa69c-117">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fa69c-117">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="fa69c-118">Relações</span><span class="sxs-lookup"><span data-stu-id="fa69c-118">Relationships</span></span>
<span data-ttu-id="fa69c-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fa69c-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fa69c-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fa69c-120">JSON representation</span></span>
<span data-ttu-id="fa69c-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fa69c-121">The following is a JSON representation of the resource.</span></span>
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
