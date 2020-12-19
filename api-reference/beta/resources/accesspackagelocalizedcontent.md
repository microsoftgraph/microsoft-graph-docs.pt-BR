---
title: tipo de recurso accessPackageLocalizedContent
description: Um tipo complexo usado para representar texto em diferentes locais, juntamente com um texto padrão. *
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 91ef87428b4171317943e9ecf1ec92e959c7a62b
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720052"
---
# <a name="accesspackagelocalizedcontent-resource-type"></a><span data-ttu-id="acc58-103">tipo de recurso accessPackageLocalizedContent</span><span class="sxs-lookup"><span data-stu-id="acc58-103">accessPackageLocalizedContent resource type</span></span>

<span data-ttu-id="acc58-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="acc58-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="acc58-105">Um tipo complexo usado para representar um texto em vários formulários do localalized.</span><span class="sxs-lookup"><span data-stu-id="acc58-105">A complex type used to represent a text in multiple localalized forms.</span></span> <span data-ttu-id="acc58-106">Ele inclui um texto padrão, que é usado em qualquer caso em que a localização solicitada não está disponível.</span><span class="sxs-lookup"><span data-stu-id="acc58-106">It includes a default text, which is used in any case where the requested localization is not available.</span></span>

## <a name="properties"></a><span data-ttu-id="acc58-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="acc58-107">Properties</span></span>
|<span data-ttu-id="acc58-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="acc58-108">Property</span></span>|<span data-ttu-id="acc58-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="acc58-109">Type</span></span>|<span data-ttu-id="acc58-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="acc58-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="acc58-111">defaultText</span><span class="sxs-lookup"><span data-stu-id="acc58-111">defaultText</span></span>|<span data-ttu-id="acc58-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="acc58-112">String</span></span>|<span data-ttu-id="acc58-113">A cadeia de caracteres de fallback, que é usada quando uma localização solicitada não está disponível.</span><span class="sxs-lookup"><span data-stu-id="acc58-113">The fallback string, which is used when a requested localization is not available.</span></span> <span data-ttu-id="acc58-114">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="acc58-114">Required.</span></span> |
|<span data-ttu-id="acc58-115">localizedTexts</span><span class="sxs-lookup"><span data-stu-id="acc58-115">localizedTexts</span></span>|<span data-ttu-id="acc58-116">coleção [accessPackageLocalizedText](../resources/accesspackagelocalizedtext.md)</span><span class="sxs-lookup"><span data-stu-id="acc58-116">[accessPackageLocalizedText](../resources/accesspackagelocalizedtext.md) collection</span></span>|<span data-ttu-id="acc58-117">Conteúdo representado em um formato para uma localidade específica.</span><span class="sxs-lookup"><span data-stu-id="acc58-117">Content represented in a format for a specific locale.</span></span> |

## <a name="relationships"></a><span data-ttu-id="acc58-118">Relações</span><span class="sxs-lookup"><span data-stu-id="acc58-118">Relationships</span></span>
<span data-ttu-id="acc58-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="acc58-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="acc58-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="acc58-120">JSON representation</span></span>
<span data-ttu-id="acc58-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="acc58-121">The following is a JSON representation of the resource.</span></span>
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
