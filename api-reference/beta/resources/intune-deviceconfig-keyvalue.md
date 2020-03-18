---
title: tipo de recurso KeyValue
description: Definição de valor de chave.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e875ba06ff704f01cc2fd7b7dd48c2b8cfcfba63
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42790381"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="88fc8-103">tipo de recurso KeyValue</span><span class="sxs-lookup"><span data-stu-id="88fc8-103">keyValue resource type</span></span>

> <span data-ttu-id="88fc8-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="88fc8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88fc8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="88fc8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88fc8-106">Definição de valor de chave.</span><span class="sxs-lookup"><span data-stu-id="88fc8-106">Key Value definition.</span></span>

## <a name="properties"></a><span data-ttu-id="88fc8-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="88fc8-107">Properties</span></span>
|<span data-ttu-id="88fc8-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="88fc8-108">Property</span></span>|<span data-ttu-id="88fc8-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="88fc8-109">Type</span></span>|<span data-ttu-id="88fc8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="88fc8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88fc8-111">key</span><span class="sxs-lookup"><span data-stu-id="88fc8-111">key</span></span>|<span data-ttu-id="88fc8-112">String</span><span class="sxs-lookup"><span data-stu-id="88fc8-112">String</span></span>|<span data-ttu-id="88fc8-113">Chave.</span><span class="sxs-lookup"><span data-stu-id="88fc8-113">Key.</span></span>|
|<span data-ttu-id="88fc8-114">value</span><span class="sxs-lookup"><span data-stu-id="88fc8-114">value</span></span>|<span data-ttu-id="88fc8-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="88fc8-115">String</span></span>|<span data-ttu-id="88fc8-116">Valor.</span><span class="sxs-lookup"><span data-stu-id="88fc8-116">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="88fc8-117">Relações</span><span class="sxs-lookup"><span data-stu-id="88fc8-117">Relationships</span></span>
<span data-ttu-id="88fc8-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="88fc8-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="88fc8-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="88fc8-119">JSON Representation</span></span>
<span data-ttu-id="88fc8-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="88fc8-120">Here is a JSON representation of the resource.</span></span>
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



