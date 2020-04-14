---
title: tipo de recurso keyIntegerValuePair
description: Um par chave-valor com uma chave de cadeia de caracteres e um valor inteiro.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 67a48f48f52c613c13552506d9cc76823bb042f7
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439977"
---
# <a name="keyintegervaluepair-resource-type"></a><span data-ttu-id="c04ed-103">tipo de recurso keyIntegerValuePair</span><span class="sxs-lookup"><span data-stu-id="c04ed-103">keyIntegerValuePair resource type</span></span>

<span data-ttu-id="c04ed-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c04ed-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c04ed-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c04ed-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c04ed-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c04ed-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c04ed-107">Um par chave-valor com uma chave de cadeia de caracteres e um valor inteiro.</span><span class="sxs-lookup"><span data-stu-id="c04ed-107">A key-value pair with a string key and an integer value.</span></span>


<span data-ttu-id="c04ed-108">Herda de [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="c04ed-108">Inherits from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c04ed-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c04ed-109">Properties</span></span>
|<span data-ttu-id="c04ed-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c04ed-110">Property</span></span>|<span data-ttu-id="c04ed-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="c04ed-111">Type</span></span>|<span data-ttu-id="c04ed-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="c04ed-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c04ed-113">key</span><span class="sxs-lookup"><span data-stu-id="c04ed-113">key</span></span>|<span data-ttu-id="c04ed-114">String</span><span class="sxs-lookup"><span data-stu-id="c04ed-114">String</span></span>|<span data-ttu-id="c04ed-115">A chave de cadeia de caracteres do par chave-valor.</span><span class="sxs-lookup"><span data-stu-id="c04ed-115">The string key of the key-value pair.</span></span> <span data-ttu-id="c04ed-116">Herdado de [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="c04ed-116">Inherited from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>|
|<span data-ttu-id="c04ed-117">valor</span><span class="sxs-lookup"><span data-stu-id="c04ed-117">value</span></span>|<span data-ttu-id="c04ed-118">Int32</span><span class="sxs-lookup"><span data-stu-id="c04ed-118">Int32</span></span>|<span data-ttu-id="c04ed-119">O valor inteiro do par chave-valor.</span><span class="sxs-lookup"><span data-stu-id="c04ed-119">The integer value of the key-value pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c04ed-120">Relações</span><span class="sxs-lookup"><span data-stu-id="c04ed-120">Relationships</span></span>
<span data-ttu-id="c04ed-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c04ed-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c04ed-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c04ed-122">JSON Representation</span></span>
<span data-ttu-id="c04ed-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c04ed-123">Here is a JSON representation of the resource.</span></span>
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



