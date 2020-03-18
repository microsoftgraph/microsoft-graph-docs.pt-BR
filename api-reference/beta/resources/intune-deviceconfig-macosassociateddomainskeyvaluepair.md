---
title: tipo de recurso macOSAssociatedDomainsKeyValuePair
description: Par chave de valor para domínios associados
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 08a59f0566da2e2dffa64c059cc913923ec5cf58
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42790318"
---
# <a name="macosassociateddomainskeyvaluepair-resource-type"></a><span data-ttu-id="b5f07-103">tipo de recurso macOSAssociatedDomainsKeyValuePair</span><span class="sxs-lookup"><span data-stu-id="b5f07-103">macOSAssociatedDomainsKeyValuePair resource type</span></span>

> <span data-ttu-id="b5f07-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b5f07-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b5f07-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b5f07-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5f07-106">Par chave de valor para domínios associados</span><span class="sxs-lookup"><span data-stu-id="b5f07-106">Key value pair for associated domains</span></span>


<span data-ttu-id="b5f07-107">Herda de [KeyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="b5f07-107">Inherits from [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b5f07-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b5f07-108">Properties</span></span>
|<span data-ttu-id="b5f07-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b5f07-109">Property</span></span>|<span data-ttu-id="b5f07-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b5f07-110">Type</span></span>|<span data-ttu-id="b5f07-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5f07-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5f07-112">nome</span><span class="sxs-lookup"><span data-stu-id="b5f07-112">name</span></span>|<span data-ttu-id="b5f07-113">String</span><span class="sxs-lookup"><span data-stu-id="b5f07-113">String</span></span>|<span data-ttu-id="b5f07-114">Nome para este par chave-valor herdado de [KeyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="b5f07-114">Name for this key-value pair Inherited from [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span></span>|
|<span data-ttu-id="b5f07-115">value</span><span class="sxs-lookup"><span data-stu-id="b5f07-115">value</span></span>|<span data-ttu-id="b5f07-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5f07-116">String</span></span>|<span data-ttu-id="b5f07-117">Valor para este par chave-valor herdado de [KeyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="b5f07-117">Value for this key-value pair Inherited from [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="b5f07-118">Relações</span><span class="sxs-lookup"><span data-stu-id="b5f07-118">Relationships</span></span>
<span data-ttu-id="b5f07-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b5f07-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b5f07-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b5f07-120">JSON Representation</span></span>
<span data-ttu-id="b5f07-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b5f07-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSAssociatedDomainsKeyValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSAssociatedDomainsKeyValuePair",
  "name": "String",
  "value": "String"
}
```



