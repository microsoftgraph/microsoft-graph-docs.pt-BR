---
title: Tipo de recurso accessPackageLocalizedContent
description: Um tipo complexo usado para representar texto em localidades diferentes, juntamente com um texto padrão.*
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 155d0ffd8f7f705c79bd753aa26f659968b87829
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137351"
---
# <a name="accesspackagelocalizedcontent-resource-type"></a><span data-ttu-id="0a695-103">Tipo de recurso accessPackageLocalizedContent</span><span class="sxs-lookup"><span data-stu-id="0a695-103">accessPackageLocalizedContent resource type</span></span>

<span data-ttu-id="0a695-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a695-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a695-105">Um tipo complexo usado para representar um texto em vários formulários localizados.</span><span class="sxs-lookup"><span data-stu-id="0a695-105">A complex type used to represent a text in multiple localalized forms.</span></span> <span data-ttu-id="0a695-106">Ele inclui um texto padrão, que é usado em qualquer caso em que a localização solicitada não está disponível.</span><span class="sxs-lookup"><span data-stu-id="0a695-106">It includes a default text, which is used in any case where the requested localization is not available.</span></span>

## <a name="properties"></a><span data-ttu-id="0a695-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0a695-107">Properties</span></span>
|<span data-ttu-id="0a695-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0a695-108">Property</span></span>|<span data-ttu-id="0a695-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="0a695-109">Type</span></span>|<span data-ttu-id="0a695-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a695-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a695-111">defaultText</span><span class="sxs-lookup"><span data-stu-id="0a695-111">defaultText</span></span>|<span data-ttu-id="0a695-112">String</span><span class="sxs-lookup"><span data-stu-id="0a695-112">String</span></span>|<span data-ttu-id="0a695-113">A cadeia de caracteres de fallback, que é usada quando uma localização solicitada não está disponível.</span><span class="sxs-lookup"><span data-stu-id="0a695-113">The fallback string, which is used when a requested localization is not available.</span></span> <span data-ttu-id="0a695-114">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0a695-114">Required.</span></span> |
|<span data-ttu-id="0a695-115">localizedTexts</span><span class="sxs-lookup"><span data-stu-id="0a695-115">localizedTexts</span></span>|<span data-ttu-id="0a695-116">[Coleção accessPackageLocalizedText](../resources/accesspackagelocalizedtext.md)</span><span class="sxs-lookup"><span data-stu-id="0a695-116">[accessPackageLocalizedText](../resources/accesspackagelocalizedtext.md) collection</span></span>|<span data-ttu-id="0a695-117">Conteúdo representado em um formato para uma localidade específica.</span><span class="sxs-lookup"><span data-stu-id="0a695-117">Content represented in a format for a specific locale.</span></span> |

## <a name="relationships"></a><span data-ttu-id="0a695-118">Relações</span><span class="sxs-lookup"><span data-stu-id="0a695-118">Relationships</span></span>
<span data-ttu-id="0a695-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0a695-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0a695-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0a695-120">JSON representation</span></span>
<span data-ttu-id="0a695-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0a695-121">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageLocalizedContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageLocalizedContent",
  "defaultText": "String",
  "localizedTexts": [
    {
      "@odata.type": "microsoft.graph.accessPackageLocalizedText"
    }
  ]
}
```
