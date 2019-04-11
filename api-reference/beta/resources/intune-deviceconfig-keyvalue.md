---
title: tipo de recurso KeyValue
description: Definição de valor de chave.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 317736fd016ca457a7fad9536ce71f00b6954b3b
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31776175"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="b9bcf-103">tipo de recurso KeyValue</span><span class="sxs-lookup"><span data-stu-id="b9bcf-103">keyValue resource type</span></span>

> <span data-ttu-id="b9bcf-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b9bcf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9bcf-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b9bcf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9bcf-106">Definição de valor de chave.</span><span class="sxs-lookup"><span data-stu-id="b9bcf-106">Key Value definition.</span></span>

## <a name="properties"></a><span data-ttu-id="b9bcf-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b9bcf-107">Properties</span></span>
|<span data-ttu-id="b9bcf-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b9bcf-108">Property</span></span>|<span data-ttu-id="b9bcf-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="b9bcf-109">Type</span></span>|<span data-ttu-id="b9bcf-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9bcf-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9bcf-111">key</span><span class="sxs-lookup"><span data-stu-id="b9bcf-111">key</span></span>|<span data-ttu-id="b9bcf-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b9bcf-112">String</span></span>|<span data-ttu-id="b9bcf-113">Chave.</span><span class="sxs-lookup"><span data-stu-id="b9bcf-113">Key.</span></span>|
|<span data-ttu-id="b9bcf-114">value</span><span class="sxs-lookup"><span data-stu-id="b9bcf-114">value</span></span>|<span data-ttu-id="b9bcf-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b9bcf-115">String</span></span>|<span data-ttu-id="b9bcf-116">Valor.</span><span class="sxs-lookup"><span data-stu-id="b9bcf-116">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b9bcf-117">Relações</span><span class="sxs-lookup"><span data-stu-id="b9bcf-117">Relationships</span></span>
<span data-ttu-id="b9bcf-118">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="b9bcf-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b9bcf-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b9bcf-119">JSON Representation</span></span>
<span data-ttu-id="b9bcf-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b9bcf-120">Here is a JSON representation of the resource.</span></span>
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





