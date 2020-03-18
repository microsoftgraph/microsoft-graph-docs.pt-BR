---
title: tipo de recurso keyRealValuePair
description: Um par chave-valor com uma chave de cadeia de caracteres e um valor real (ponto flutuante).
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6b90c7faa0bb3ffabe5b057d03503745801af8c8
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42790423"
---
# <a name="keyrealvaluepair-resource-type"></a><span data-ttu-id="d8876-103">tipo de recurso keyRealValuePair</span><span class="sxs-lookup"><span data-stu-id="d8876-103">keyRealValuePair resource type</span></span>

> <span data-ttu-id="d8876-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d8876-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d8876-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d8876-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8876-106">Um par chave-valor com uma chave de cadeia de caracteres e um valor real (ponto flutuante).</span><span class="sxs-lookup"><span data-stu-id="d8876-106">A key-value pair with a string key and a real (floating-point) value.</span></span>


<span data-ttu-id="d8876-107">Herda de [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="d8876-107">Inherits from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d8876-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d8876-108">Properties</span></span>
|<span data-ttu-id="d8876-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d8876-109">Property</span></span>|<span data-ttu-id="d8876-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8876-110">Type</span></span>|<span data-ttu-id="d8876-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8876-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8876-112">key</span><span class="sxs-lookup"><span data-stu-id="d8876-112">key</span></span>|<span data-ttu-id="d8876-113">String</span><span class="sxs-lookup"><span data-stu-id="d8876-113">String</span></span>|<span data-ttu-id="d8876-114">A chave de cadeia de caracteres do par chave-valor.</span><span class="sxs-lookup"><span data-stu-id="d8876-114">The string key of the key-value pair.</span></span> <span data-ttu-id="d8876-115">Herdado de [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="d8876-115">Inherited from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>|
|<span data-ttu-id="d8876-116">valor</span><span class="sxs-lookup"><span data-stu-id="d8876-116">value</span></span>|<span data-ttu-id="d8876-117">Duplo</span><span class="sxs-lookup"><span data-stu-id="d8876-117">Double</span></span>|<span data-ttu-id="d8876-118">O valor real (ponto flutuante) do par chave-valor.</span><span class="sxs-lookup"><span data-stu-id="d8876-118">The real (floating-point) value of the key-value pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d8876-119">Relações</span><span class="sxs-lookup"><span data-stu-id="d8876-119">Relationships</span></span>
<span data-ttu-id="d8876-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d8876-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d8876-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d8876-121">JSON Representation</span></span>
<span data-ttu-id="d8876-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d8876-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyRealValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyRealValuePair",
  "key": "String",
  "value": "<Unknown Primitive Type Edm.Double>"
}
```



