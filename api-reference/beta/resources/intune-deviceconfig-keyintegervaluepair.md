---
title: tipo de recurso keyIntegerValuePair
description: Um par chave-valor com uma chave de cadeia de caracteres e um valor inteiro.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0cd9c4de9f7c2505b12eada575ebc5d869480758
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199688"
---
# <a name="keyintegervaluepair-resource-type"></a><span data-ttu-id="9ee80-103">tipo de recurso keyIntegerValuePair</span><span class="sxs-lookup"><span data-stu-id="9ee80-103">keyIntegerValuePair resource type</span></span>

> <span data-ttu-id="9ee80-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9ee80-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9ee80-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9ee80-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ee80-106">Um par chave-valor com uma chave de cadeia de caracteres e um valor inteiro.</span><span class="sxs-lookup"><span data-stu-id="9ee80-106">A key-value pair with a string key and an integer value.</span></span>


<span data-ttu-id="9ee80-107">Herda de [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="9ee80-107">Inherits from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9ee80-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9ee80-108">Properties</span></span>
|<span data-ttu-id="9ee80-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9ee80-109">Property</span></span>|<span data-ttu-id="9ee80-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="9ee80-110">Type</span></span>|<span data-ttu-id="9ee80-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ee80-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ee80-112">key</span><span class="sxs-lookup"><span data-stu-id="9ee80-112">key</span></span>|<span data-ttu-id="9ee80-113">String</span><span class="sxs-lookup"><span data-stu-id="9ee80-113">String</span></span>|<span data-ttu-id="9ee80-114">A chave de cadeia de caracteres do par chave-valor.</span><span class="sxs-lookup"><span data-stu-id="9ee80-114">The string key of the key-value pair.</span></span> <span data-ttu-id="9ee80-115">Herdado de [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="9ee80-115">Inherited from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>|
|<span data-ttu-id="9ee80-116">valor</span><span class="sxs-lookup"><span data-stu-id="9ee80-116">value</span></span>|<span data-ttu-id="9ee80-117">Int32</span><span class="sxs-lookup"><span data-stu-id="9ee80-117">Int32</span></span>|<span data-ttu-id="9ee80-118">O valor inteiro do par chave-valor.</span><span class="sxs-lookup"><span data-stu-id="9ee80-118">The integer value of the key-value pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ee80-119">Relações</span><span class="sxs-lookup"><span data-stu-id="9ee80-119">Relationships</span></span>
<span data-ttu-id="9ee80-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9ee80-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9ee80-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9ee80-121">JSON Representation</span></span>
<span data-ttu-id="9ee80-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9ee80-122">Here is a JSON representation of the resource.</span></span>
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



