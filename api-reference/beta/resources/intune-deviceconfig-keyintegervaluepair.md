---
title: tipo de recurso keyIntegerValuePair
description: Um par chave-valor com uma chave de cadeia de caracteres e um valor inteiro.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0f2a3f4201956db2cbca001f8d94f6ae6ecc90d7
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42790430"
---
# <a name="keyintegervaluepair-resource-type"></a><span data-ttu-id="544dd-103">tipo de recurso keyIntegerValuePair</span><span class="sxs-lookup"><span data-stu-id="544dd-103">keyIntegerValuePair resource type</span></span>

> <span data-ttu-id="544dd-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="544dd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="544dd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="544dd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="544dd-106">Um par chave-valor com uma chave de cadeia de caracteres e um valor inteiro.</span><span class="sxs-lookup"><span data-stu-id="544dd-106">A key-value pair with a string key and an integer value.</span></span>


<span data-ttu-id="544dd-107">Herda de [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="544dd-107">Inherits from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>

## <a name="properties"></a><span data-ttu-id="544dd-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="544dd-108">Properties</span></span>
|<span data-ttu-id="544dd-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="544dd-109">Property</span></span>|<span data-ttu-id="544dd-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="544dd-110">Type</span></span>|<span data-ttu-id="544dd-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="544dd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="544dd-112">key</span><span class="sxs-lookup"><span data-stu-id="544dd-112">key</span></span>|<span data-ttu-id="544dd-113">String</span><span class="sxs-lookup"><span data-stu-id="544dd-113">String</span></span>|<span data-ttu-id="544dd-114">A chave de cadeia de caracteres do par chave-valor.</span><span class="sxs-lookup"><span data-stu-id="544dd-114">The string key of the key-value pair.</span></span> <span data-ttu-id="544dd-115">Herdado de [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="544dd-115">Inherited from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>|
|<span data-ttu-id="544dd-116">valor</span><span class="sxs-lookup"><span data-stu-id="544dd-116">value</span></span>|<span data-ttu-id="544dd-117">Int32</span><span class="sxs-lookup"><span data-stu-id="544dd-117">Int32</span></span>|<span data-ttu-id="544dd-118">O valor inteiro do par chave-valor.</span><span class="sxs-lookup"><span data-stu-id="544dd-118">The integer value of the key-value pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="544dd-119">Relações</span><span class="sxs-lookup"><span data-stu-id="544dd-119">Relationships</span></span>
<span data-ttu-id="544dd-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="544dd-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="544dd-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="544dd-121">JSON Representation</span></span>
<span data-ttu-id="544dd-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="544dd-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyIntegerValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyIntegerValuePair",
  "key": "String",
  "value": 1024
}
```



