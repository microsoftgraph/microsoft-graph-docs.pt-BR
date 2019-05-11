---
title: tipo de recurso KeyValue
description: Definição de valor de chave.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 592f3ff070ab7440d5c16d5380b556993915e6ec
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946111"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="fdc51-103">tipo de recurso KeyValue</span><span class="sxs-lookup"><span data-stu-id="fdc51-103">keyValue resource type</span></span>

> <span data-ttu-id="fdc51-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fdc51-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fdc51-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fdc51-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fdc51-106">Definição de valor de chave.</span><span class="sxs-lookup"><span data-stu-id="fdc51-106">Key Value definition.</span></span>

## <a name="properties"></a><span data-ttu-id="fdc51-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fdc51-107">Properties</span></span>
|<span data-ttu-id="fdc51-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fdc51-108">Property</span></span>|<span data-ttu-id="fdc51-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="fdc51-109">Type</span></span>|<span data-ttu-id="fdc51-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="fdc51-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fdc51-111">key</span><span class="sxs-lookup"><span data-stu-id="fdc51-111">key</span></span>|<span data-ttu-id="fdc51-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fdc51-112">String</span></span>|<span data-ttu-id="fdc51-113">Chave.</span><span class="sxs-lookup"><span data-stu-id="fdc51-113">Key.</span></span>|
|<span data-ttu-id="fdc51-114">value</span><span class="sxs-lookup"><span data-stu-id="fdc51-114">value</span></span>|<span data-ttu-id="fdc51-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fdc51-115">String</span></span>|<span data-ttu-id="fdc51-116">Valor.</span><span class="sxs-lookup"><span data-stu-id="fdc51-116">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fdc51-117">Relações</span><span class="sxs-lookup"><span data-stu-id="fdc51-117">Relationships</span></span>
<span data-ttu-id="fdc51-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fdc51-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fdc51-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fdc51-119">JSON Representation</span></span>
<span data-ttu-id="fdc51-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fdc51-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyValue",
  "key": "String",
  "value": "String"
}
```




