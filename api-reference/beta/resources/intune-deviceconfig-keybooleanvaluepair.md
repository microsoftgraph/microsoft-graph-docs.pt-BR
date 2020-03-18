---
title: tipo de recurso keyBooleanValuePair
description: Um par chave-valor com uma chave de cadeia de caracteres e um valor Boolean.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6e06d58e1eca3c4f562ab83854dd721162941bc9
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42790437"
---
# <a name="keybooleanvaluepair-resource-type"></a><span data-ttu-id="fbc52-103">tipo de recurso keyBooleanValuePair</span><span class="sxs-lookup"><span data-stu-id="fbc52-103">keyBooleanValuePair resource type</span></span>

> <span data-ttu-id="fbc52-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fbc52-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fbc52-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fbc52-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fbc52-106">Um par chave-valor com uma chave de cadeia de caracteres e um valor Boolean.</span><span class="sxs-lookup"><span data-stu-id="fbc52-106">A key-value pair with a string key and a Boolean value.</span></span>


<span data-ttu-id="fbc52-107">Herda de [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="fbc52-107">Inherits from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fbc52-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fbc52-108">Properties</span></span>
|<span data-ttu-id="fbc52-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fbc52-109">Property</span></span>|<span data-ttu-id="fbc52-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="fbc52-110">Type</span></span>|<span data-ttu-id="fbc52-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="fbc52-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbc52-112">key</span><span class="sxs-lookup"><span data-stu-id="fbc52-112">key</span></span>|<span data-ttu-id="fbc52-113">String</span><span class="sxs-lookup"><span data-stu-id="fbc52-113">String</span></span>|<span data-ttu-id="fbc52-114">A chave de cadeia de caracteres do par chave-valor.</span><span class="sxs-lookup"><span data-stu-id="fbc52-114">The string key of the key-value pair.</span></span> <span data-ttu-id="fbc52-115">Herdado de [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="fbc52-115">Inherited from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>|
|<span data-ttu-id="fbc52-116">value</span><span class="sxs-lookup"><span data-stu-id="fbc52-116">value</span></span>|<span data-ttu-id="fbc52-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="fbc52-117">Boolean</span></span>|<span data-ttu-id="fbc52-118">O valor booliano do par chave-valor.</span><span class="sxs-lookup"><span data-stu-id="fbc52-118">The Boolean value of the key-value pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fbc52-119">Relações</span><span class="sxs-lookup"><span data-stu-id="fbc52-119">Relationships</span></span>
<span data-ttu-id="fbc52-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fbc52-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fbc52-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fbc52-121">JSON Representation</span></span>
<span data-ttu-id="fbc52-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fbc52-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyBooleanValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyBooleanValuePair",
  "key": "String",
  "value": true
}
```



