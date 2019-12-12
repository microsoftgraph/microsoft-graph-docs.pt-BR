---
title: tipo de recurso keyRealValuePair
description: Um par chave-valor com uma chave de cadeia de caracteres e um valor real (ponto flutuante).
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6d7bbe482d03990a8056e89bbe7608911c1eff9f
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955635"
---
# <a name="keyrealvaluepair-resource-type"></a><span data-ttu-id="8e305-103">tipo de recurso keyRealValuePair</span><span class="sxs-lookup"><span data-stu-id="8e305-103">keyRealValuePair resource type</span></span>

> <span data-ttu-id="8e305-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8e305-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8e305-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8e305-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e305-106">Um par chave-valor com uma chave de cadeia de caracteres e um valor real (ponto flutuante).</span><span class="sxs-lookup"><span data-stu-id="8e305-106">A key-value pair with a string key and a real (floating-point) value.</span></span>


<span data-ttu-id="8e305-107">Herda de [keyTypedValuePair](../resources/intune-shared-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="8e305-107">Inherits from [keyTypedValuePair](../resources/intune-shared-keytypedvaluepair.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8e305-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8e305-108">Properties</span></span>
|<span data-ttu-id="8e305-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8e305-109">Property</span></span>|<span data-ttu-id="8e305-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="8e305-110">Type</span></span>|<span data-ttu-id="8e305-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e305-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e305-112">key</span><span class="sxs-lookup"><span data-stu-id="8e305-112">key</span></span>|<span data-ttu-id="8e305-113">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="8e305-113">String</span></span>|<span data-ttu-id="8e305-114">A chave de cadeia de caracteres do par chave-valor.</span><span class="sxs-lookup"><span data-stu-id="8e305-114">The string key of the key-value pair.</span></span> <span data-ttu-id="8e305-115">Herdado de [keyTypedValuePair](../resources/intune-shared-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="8e305-115">Inherited from [keyTypedValuePair](../resources/intune-shared-keytypedvaluepair.md)</span></span>|
|<span data-ttu-id="8e305-116">valor</span><span class="sxs-lookup"><span data-stu-id="8e305-116">value</span></span>|<span data-ttu-id="8e305-117">Duplo</span><span class="sxs-lookup"><span data-stu-id="8e305-117">Double</span></span>|<span data-ttu-id="8e305-118">O valor real (ponto flutuante) do par chave-valor.</span><span class="sxs-lookup"><span data-stu-id="8e305-118">The real (floating-point) value of the key-value pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8e305-119">Relações</span><span class="sxs-lookup"><span data-stu-id="8e305-119">Relationships</span></span>
<span data-ttu-id="8e305-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8e305-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8e305-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8e305-121">JSON Representation</span></span>
<span data-ttu-id="8e305-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8e305-122">Here is a JSON representation of the resource.</span></span>
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



