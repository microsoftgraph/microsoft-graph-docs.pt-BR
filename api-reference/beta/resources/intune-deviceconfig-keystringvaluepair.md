---
title: tipo de recurso keyStringValuePair
description: Um par chave-valor com uma chave de cadeia de caracteres e um valor de cadeia de caracteres.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 029ebbe04532b729b49115fd51cdbcf4ea22a6a3
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42790402"
---
# <a name="keystringvaluepair-resource-type"></a><span data-ttu-id="11b2b-103">tipo de recurso keyStringValuePair</span><span class="sxs-lookup"><span data-stu-id="11b2b-103">keyStringValuePair resource type</span></span>

> <span data-ttu-id="11b2b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="11b2b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="11b2b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="11b2b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11b2b-106">Um par chave-valor com uma chave de cadeia de caracteres e um valor de cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="11b2b-106">A key-value pair with a string key and a string value.</span></span>


<span data-ttu-id="11b2b-107">Herda de [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="11b2b-107">Inherits from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>

## <a name="properties"></a><span data-ttu-id="11b2b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="11b2b-108">Properties</span></span>
|<span data-ttu-id="11b2b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="11b2b-109">Property</span></span>|<span data-ttu-id="11b2b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="11b2b-110">Type</span></span>|<span data-ttu-id="11b2b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="11b2b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11b2b-112">key</span><span class="sxs-lookup"><span data-stu-id="11b2b-112">key</span></span>|<span data-ttu-id="11b2b-113">String</span><span class="sxs-lookup"><span data-stu-id="11b2b-113">String</span></span>|<span data-ttu-id="11b2b-114">A chave de cadeia de caracteres do par chave-valor.</span><span class="sxs-lookup"><span data-stu-id="11b2b-114">The string key of the key-value pair.</span></span> <span data-ttu-id="11b2b-115">Herdado de [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="11b2b-115">Inherited from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>|
|<span data-ttu-id="11b2b-116">value</span><span class="sxs-lookup"><span data-stu-id="11b2b-116">value</span></span>|<span data-ttu-id="11b2b-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="11b2b-117">String</span></span>|<span data-ttu-id="11b2b-118">O valor da cadeia de caracteres do par chave-valor.</span><span class="sxs-lookup"><span data-stu-id="11b2b-118">The string value of the key-value pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="11b2b-119">Relações</span><span class="sxs-lookup"><span data-stu-id="11b2b-119">Relationships</span></span>
<span data-ttu-id="11b2b-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="11b2b-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="11b2b-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="11b2b-121">JSON Representation</span></span>
<span data-ttu-id="11b2b-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="11b2b-122">Here is a JSON representation of the resource.</span></span>
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



