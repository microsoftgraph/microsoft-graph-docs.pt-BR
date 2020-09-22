---
title: tipo de recurso keyIntegerValuePair
description: Um par chave-valor com uma chave de cadeia de caracteres e um valor inteiro.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: efba214d6cd6b4e8fb79ddb4df4c9df0e16974bc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092542"
---
# <a name="keyintegervaluepair-resource-type"></a><span data-ttu-id="d4227-103">tipo de recurso keyIntegerValuePair</span><span class="sxs-lookup"><span data-stu-id="d4227-103">keyIntegerValuePair resource type</span></span>

<span data-ttu-id="d4227-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4227-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d4227-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d4227-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4227-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d4227-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4227-107">Um par chave-valor com uma chave de cadeia de caracteres e um valor inteiro.</span><span class="sxs-lookup"><span data-stu-id="d4227-107">A key-value pair with a string key and an integer value.</span></span>


<span data-ttu-id="d4227-108">Herda de [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="d4227-108">Inherits from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d4227-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d4227-109">Properties</span></span>
|<span data-ttu-id="d4227-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d4227-110">Property</span></span>|<span data-ttu-id="d4227-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="d4227-111">Type</span></span>|<span data-ttu-id="d4227-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4227-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4227-113">key</span><span class="sxs-lookup"><span data-stu-id="d4227-113">key</span></span>|<span data-ttu-id="d4227-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d4227-114">String</span></span>|<span data-ttu-id="d4227-115">A chave de cadeia de caracteres do par chave-valor.</span><span class="sxs-lookup"><span data-stu-id="d4227-115">The string key of the key-value pair.</span></span> <span data-ttu-id="d4227-116">Herdado de [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="d4227-116">Inherited from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>|
|<span data-ttu-id="d4227-117">valor</span><span class="sxs-lookup"><span data-stu-id="d4227-117">value</span></span>|<span data-ttu-id="d4227-118">Int32</span><span class="sxs-lookup"><span data-stu-id="d4227-118">Int32</span></span>|<span data-ttu-id="d4227-119">O valor inteiro do par chave-valor.</span><span class="sxs-lookup"><span data-stu-id="d4227-119">The integer value of the key-value pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d4227-120">Relações</span><span class="sxs-lookup"><span data-stu-id="d4227-120">Relationships</span></span>
<span data-ttu-id="d4227-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d4227-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d4227-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d4227-122">JSON Representation</span></span>
<span data-ttu-id="d4227-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d4227-123">Here is a JSON representation of the resource.</span></span>
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






