---
title: tipo de recurso keyStringValuePair
description: Um par chave-valor com uma chave de cadeia de caracteres e um valor de cadeia de caracteres.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5b97ddd3a6b5a163455a1986fa7e15a774f6c79d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092458"
---
# <a name="keystringvaluepair-resource-type"></a><span data-ttu-id="84bc6-103">tipo de recurso keyStringValuePair</span><span class="sxs-lookup"><span data-stu-id="84bc6-103">keyStringValuePair resource type</span></span>

<span data-ttu-id="84bc6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84bc6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="84bc6-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="84bc6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84bc6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="84bc6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84bc6-107">Um par chave-valor com uma chave de cadeia de caracteres e um valor de cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="84bc6-107">A key-value pair with a string key and a string value.</span></span>


<span data-ttu-id="84bc6-108">Herda de [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="84bc6-108">Inherits from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>

## <a name="properties"></a><span data-ttu-id="84bc6-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="84bc6-109">Properties</span></span>
|<span data-ttu-id="84bc6-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="84bc6-110">Property</span></span>|<span data-ttu-id="84bc6-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="84bc6-111">Type</span></span>|<span data-ttu-id="84bc6-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="84bc6-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84bc6-113">key</span><span class="sxs-lookup"><span data-stu-id="84bc6-113">key</span></span>|<span data-ttu-id="84bc6-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="84bc6-114">String</span></span>|<span data-ttu-id="84bc6-115">A chave de cadeia de caracteres do par chave-valor.</span><span class="sxs-lookup"><span data-stu-id="84bc6-115">The string key of the key-value pair.</span></span> <span data-ttu-id="84bc6-116">Herdado de [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="84bc6-116">Inherited from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>|
|<span data-ttu-id="84bc6-117">value</span><span class="sxs-lookup"><span data-stu-id="84bc6-117">value</span></span>|<span data-ttu-id="84bc6-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="84bc6-118">String</span></span>|<span data-ttu-id="84bc6-119">O valor da cadeia de caracteres do par chave-valor.</span><span class="sxs-lookup"><span data-stu-id="84bc6-119">The string value of the key-value pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="84bc6-120">Relações</span><span class="sxs-lookup"><span data-stu-id="84bc6-120">Relationships</span></span>
<span data-ttu-id="84bc6-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="84bc6-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="84bc6-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="84bc6-122">JSON Representation</span></span>
<span data-ttu-id="84bc6-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="84bc6-123">Here is a JSON representation of the resource.</span></span>
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






