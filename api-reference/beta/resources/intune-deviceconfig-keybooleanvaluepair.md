---
title: tipo de recurso keyBooleanValuePair
description: Um par chave-valor com uma chave de cadeia de caracteres e um valor Boolean.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c525c1880c8a77dd8bf29c1ee5c8fb2864ab928b
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199690"
---
# <a name="keybooleanvaluepair-resource-type"></a><span data-ttu-id="6c368-103">tipo de recurso keyBooleanValuePair</span><span class="sxs-lookup"><span data-stu-id="6c368-103">keyBooleanValuePair resource type</span></span>

> <span data-ttu-id="6c368-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6c368-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c368-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6c368-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c368-106">Um par chave-valor com uma chave de cadeia de caracteres e um valor Boolean.</span><span class="sxs-lookup"><span data-stu-id="6c368-106">A key-value pair with a string key and a Boolean value.</span></span>


<span data-ttu-id="6c368-107">Herda de [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="6c368-107">Inherits from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6c368-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6c368-108">Properties</span></span>
|<span data-ttu-id="6c368-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6c368-109">Property</span></span>|<span data-ttu-id="6c368-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="6c368-110">Type</span></span>|<span data-ttu-id="6c368-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c368-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c368-112">key</span><span class="sxs-lookup"><span data-stu-id="6c368-112">key</span></span>|<span data-ttu-id="6c368-113">String</span><span class="sxs-lookup"><span data-stu-id="6c368-113">String</span></span>|<span data-ttu-id="6c368-114">A chave de cadeia de caracteres do par chave-valor.</span><span class="sxs-lookup"><span data-stu-id="6c368-114">The string key of the key-value pair.</span></span> <span data-ttu-id="6c368-115">Herdado de [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="6c368-115">Inherited from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>|
|<span data-ttu-id="6c368-116">value</span><span class="sxs-lookup"><span data-stu-id="6c368-116">value</span></span>|<span data-ttu-id="6c368-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c368-117">Boolean</span></span>|<span data-ttu-id="6c368-118">O valor booliano do par chave-valor.</span><span class="sxs-lookup"><span data-stu-id="6c368-118">The Boolean value of the key-value pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6c368-119">Relações</span><span class="sxs-lookup"><span data-stu-id="6c368-119">Relationships</span></span>
<span data-ttu-id="6c368-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6c368-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6c368-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6c368-121">JSON Representation</span></span>
<span data-ttu-id="6c368-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6c368-122">Here is a JSON representation of the resource.</span></span>
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



