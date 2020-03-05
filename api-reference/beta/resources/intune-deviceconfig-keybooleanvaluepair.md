---
title: tipo de recurso keyBooleanValuePair
description: Um par chave-valor com uma chave de cadeia de caracteres e um valor Boolean.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: aabdb6e8eef4e41ec5c9aaf5d1a24fca97ae8c2e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526266"
---
# <a name="keybooleanvaluepair-resource-type"></a><span data-ttu-id="a88f6-103">tipo de recurso keyBooleanValuePair</span><span class="sxs-lookup"><span data-stu-id="a88f6-103">keyBooleanValuePair resource type</span></span>

<span data-ttu-id="a88f6-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a88f6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a88f6-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a88f6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a88f6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a88f6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a88f6-107">Um par chave-valor com uma chave de cadeia de caracteres e um valor Boolean.</span><span class="sxs-lookup"><span data-stu-id="a88f6-107">A key-value pair with a string key and a Boolean value.</span></span>


<span data-ttu-id="a88f6-108">Herda de [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="a88f6-108">Inherits from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a88f6-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a88f6-109">Properties</span></span>
|<span data-ttu-id="a88f6-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a88f6-110">Property</span></span>|<span data-ttu-id="a88f6-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="a88f6-111">Type</span></span>|<span data-ttu-id="a88f6-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="a88f6-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a88f6-113">key</span><span class="sxs-lookup"><span data-stu-id="a88f6-113">key</span></span>|<span data-ttu-id="a88f6-114">String</span><span class="sxs-lookup"><span data-stu-id="a88f6-114">String</span></span>|<span data-ttu-id="a88f6-115">A chave de cadeia de caracteres do par chave-valor.</span><span class="sxs-lookup"><span data-stu-id="a88f6-115">The string key of the key-value pair.</span></span> <span data-ttu-id="a88f6-116">Herdado de [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="a88f6-116">Inherited from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>|
|<span data-ttu-id="a88f6-117">value</span><span class="sxs-lookup"><span data-stu-id="a88f6-117">value</span></span>|<span data-ttu-id="a88f6-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="a88f6-118">Boolean</span></span>|<span data-ttu-id="a88f6-119">O valor booliano do par chave-valor.</span><span class="sxs-lookup"><span data-stu-id="a88f6-119">The Boolean value of the key-value pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a88f6-120">Relações</span><span class="sxs-lookup"><span data-stu-id="a88f6-120">Relationships</span></span>
<span data-ttu-id="a88f6-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a88f6-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a88f6-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a88f6-122">JSON Representation</span></span>
<span data-ttu-id="a88f6-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a88f6-123">Here is a JSON representation of the resource.</span></span>
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



