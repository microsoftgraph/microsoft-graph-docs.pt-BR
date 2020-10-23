---
title: tipo de recurso keyRealValuePair
description: Um par chave-valor com uma chave de cadeia de caracteres e um valor real (ponto flutuante).
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e3e8d7d093c50262ee60784bcfd4b1c348696786
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48726455"
---
# <a name="keyrealvaluepair-resource-type"></a><span data-ttu-id="bbeb1-103">tipo de recurso keyRealValuePair</span><span class="sxs-lookup"><span data-stu-id="bbeb1-103">keyRealValuePair resource type</span></span>

<span data-ttu-id="bbeb1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bbeb1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bbeb1-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bbeb1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bbeb1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bbeb1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bbeb1-107">Um par chave-valor com uma chave de cadeia de caracteres e um valor real (ponto flutuante).</span><span class="sxs-lookup"><span data-stu-id="bbeb1-107">A key-value pair with a string key and a real (floating-point) value.</span></span>


<span data-ttu-id="bbeb1-108">Herda de [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="bbeb1-108">Inherits from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bbeb1-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bbeb1-109">Properties</span></span>
|<span data-ttu-id="bbeb1-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bbeb1-110">Property</span></span>|<span data-ttu-id="bbeb1-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="bbeb1-111">Type</span></span>|<span data-ttu-id="bbeb1-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbeb1-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bbeb1-113">key</span><span class="sxs-lookup"><span data-stu-id="bbeb1-113">key</span></span>|<span data-ttu-id="bbeb1-114">String</span><span class="sxs-lookup"><span data-stu-id="bbeb1-114">String</span></span>|<span data-ttu-id="bbeb1-115">A chave de cadeia de caracteres do par chave-valor.</span><span class="sxs-lookup"><span data-stu-id="bbeb1-115">The string key of the key-value pair.</span></span> <span data-ttu-id="bbeb1-116">Herdado de [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="bbeb1-116">Inherited from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>|
|<span data-ttu-id="bbeb1-117">valor</span><span class="sxs-lookup"><span data-stu-id="bbeb1-117">value</span></span>|<span data-ttu-id="bbeb1-118">Duplo</span><span class="sxs-lookup"><span data-stu-id="bbeb1-118">Double</span></span>|<span data-ttu-id="bbeb1-119">O valor real (ponto flutuante) do par chave-valor.</span><span class="sxs-lookup"><span data-stu-id="bbeb1-119">The real (floating-point) value of the key-value pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bbeb1-120">Relações</span><span class="sxs-lookup"><span data-stu-id="bbeb1-120">Relationships</span></span>
<span data-ttu-id="bbeb1-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bbeb1-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bbeb1-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bbeb1-122">JSON Representation</span></span>
<span data-ttu-id="bbeb1-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bbeb1-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyRealValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyRealValuePair",
  "key": "String",
  "value": "4.2"
}
```





