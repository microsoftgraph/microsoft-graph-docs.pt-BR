---
title: tipo de recurso keyRealValuePair
description: Um par chave-valor com uma chave de cadeia de caracteres e um valor real (ponto flutuante).
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3f8611f5739862e659abaa2581943a30416f2138
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199687"
---
# <a name="keyrealvaluepair-resource-type"></a><span data-ttu-id="0337f-103">tipo de recurso keyRealValuePair</span><span class="sxs-lookup"><span data-stu-id="0337f-103">keyRealValuePair resource type</span></span>

> <span data-ttu-id="0337f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0337f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0337f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0337f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0337f-106">Um par chave-valor com uma chave de cadeia de caracteres e um valor real (ponto flutuante).</span><span class="sxs-lookup"><span data-stu-id="0337f-106">A key-value pair with a string key and a real (floating-point) value.</span></span>


<span data-ttu-id="0337f-107">Herda de [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="0337f-107">Inherits from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0337f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0337f-108">Properties</span></span>
|<span data-ttu-id="0337f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0337f-109">Property</span></span>|<span data-ttu-id="0337f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="0337f-110">Type</span></span>|<span data-ttu-id="0337f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0337f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0337f-112">key</span><span class="sxs-lookup"><span data-stu-id="0337f-112">key</span></span>|<span data-ttu-id="0337f-113">String</span><span class="sxs-lookup"><span data-stu-id="0337f-113">String</span></span>|<span data-ttu-id="0337f-114">A chave de cadeia de caracteres do par chave-valor.</span><span class="sxs-lookup"><span data-stu-id="0337f-114">The string key of the key-value pair.</span></span> <span data-ttu-id="0337f-115">Herdado de [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="0337f-115">Inherited from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>|
|<span data-ttu-id="0337f-116">valor</span><span class="sxs-lookup"><span data-stu-id="0337f-116">value</span></span>|<span data-ttu-id="0337f-117">Duplo</span><span class="sxs-lookup"><span data-stu-id="0337f-117">Double</span></span>|<span data-ttu-id="0337f-118">O valor real (ponto flutuante) do par chave-valor.</span><span class="sxs-lookup"><span data-stu-id="0337f-118">The real (floating-point) value of the key-value pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0337f-119">Relações</span><span class="sxs-lookup"><span data-stu-id="0337f-119">Relationships</span></span>
<span data-ttu-id="0337f-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0337f-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0337f-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0337f-121">JSON Representation</span></span>
<span data-ttu-id="0337f-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0337f-122">Here is a JSON representation of the resource.</span></span>
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



