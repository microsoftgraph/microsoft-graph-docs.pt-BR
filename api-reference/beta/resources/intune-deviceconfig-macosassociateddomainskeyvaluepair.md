---
title: tipo de recurso macOSAssociatedDomainsKeyValuePair
description: Par chave de valor para domínios associados
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ebf62a01d4a97fde51974ea2e7984b97c39dc5d4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439719"
---
# <a name="macosassociateddomainskeyvaluepair-resource-type"></a><span data-ttu-id="6fc4e-103">tipo de recurso macOSAssociatedDomainsKeyValuePair</span><span class="sxs-lookup"><span data-stu-id="6fc4e-103">macOSAssociatedDomainsKeyValuePair resource type</span></span>

<span data-ttu-id="6fc4e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6fc4e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6fc4e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6fc4e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6fc4e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6fc4e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6fc4e-107">Par chave de valor para domínios associados</span><span class="sxs-lookup"><span data-stu-id="6fc4e-107">Key value pair for associated domains</span></span>


<span data-ttu-id="6fc4e-108">Herda de [KeyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="6fc4e-108">Inherits from [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6fc4e-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6fc4e-109">Properties</span></span>
|<span data-ttu-id="6fc4e-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6fc4e-110">Property</span></span>|<span data-ttu-id="6fc4e-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="6fc4e-111">Type</span></span>|<span data-ttu-id="6fc4e-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="6fc4e-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fc4e-113">nome</span><span class="sxs-lookup"><span data-stu-id="6fc4e-113">name</span></span>|<span data-ttu-id="6fc4e-114">String</span><span class="sxs-lookup"><span data-stu-id="6fc4e-114">String</span></span>|<span data-ttu-id="6fc4e-115">Nome para este par chave-valor herdado de [KeyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="6fc4e-115">Name for this key-value pair Inherited from [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span></span>|
|<span data-ttu-id="6fc4e-116">value</span><span class="sxs-lookup"><span data-stu-id="6fc4e-116">value</span></span>|<span data-ttu-id="6fc4e-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6fc4e-117">String</span></span>|<span data-ttu-id="6fc4e-118">Valor para este par chave-valor herdado de [KeyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="6fc4e-118">Value for this key-value pair Inherited from [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="6fc4e-119">Relações</span><span class="sxs-lookup"><span data-stu-id="6fc4e-119">Relationships</span></span>
<span data-ttu-id="6fc4e-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6fc4e-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6fc4e-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6fc4e-121">JSON Representation</span></span>
<span data-ttu-id="6fc4e-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6fc4e-122">Here is a JSON representation of the resource.</span></span>
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



