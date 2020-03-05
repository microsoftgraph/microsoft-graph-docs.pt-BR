---
title: tipo de recurso keyStringValuePair
description: Um par chave-valor com uma chave de cadeia de caracteres e um valor de cadeia de caracteres.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7ad2380d84a329d2bfaf9359128944e90a90c393
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529778"
---
# <a name="keystringvaluepair-resource-type"></a><span data-ttu-id="b09b2-103">tipo de recurso keyStringValuePair</span><span class="sxs-lookup"><span data-stu-id="b09b2-103">keyStringValuePair resource type</span></span>

<span data-ttu-id="b09b2-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b09b2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b09b2-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b09b2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b09b2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b09b2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b09b2-107">Um par chave-valor com uma chave de cadeia de caracteres e um valor de cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="b09b2-107">A key-value pair with a string key and a string value.</span></span>


<span data-ttu-id="b09b2-108">Herda de [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="b09b2-108">Inherits from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b09b2-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b09b2-109">Properties</span></span>
|<span data-ttu-id="b09b2-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b09b2-110">Property</span></span>|<span data-ttu-id="b09b2-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="b09b2-111">Type</span></span>|<span data-ttu-id="b09b2-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="b09b2-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b09b2-113">key</span><span class="sxs-lookup"><span data-stu-id="b09b2-113">key</span></span>|<span data-ttu-id="b09b2-114">String</span><span class="sxs-lookup"><span data-stu-id="b09b2-114">String</span></span>|<span data-ttu-id="b09b2-115">A chave de cadeia de caracteres do par chave-valor.</span><span class="sxs-lookup"><span data-stu-id="b09b2-115">The string key of the key-value pair.</span></span> <span data-ttu-id="b09b2-116">Herdado de [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="b09b2-116">Inherited from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>|
|<span data-ttu-id="b09b2-117">value</span><span class="sxs-lookup"><span data-stu-id="b09b2-117">value</span></span>|<span data-ttu-id="b09b2-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b09b2-118">String</span></span>|<span data-ttu-id="b09b2-119">O valor da cadeia de caracteres do par chave-valor.</span><span class="sxs-lookup"><span data-stu-id="b09b2-119">The string value of the key-value pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b09b2-120">Relações</span><span class="sxs-lookup"><span data-stu-id="b09b2-120">Relationships</span></span>
<span data-ttu-id="b09b2-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b09b2-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b09b2-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b09b2-122">JSON Representation</span></span>
<span data-ttu-id="b09b2-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b09b2-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyStringValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyStringValuePair",
  "key": "String",
  "value": "String"
}
```



