---
title: tipo de recurso KeyValue
description: Definição de valor de chave.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a29fcb627a1777b2fc0a4863bbab27d5fa364982
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36325516"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="d2582-103">tipo de recurso KeyValue</span><span class="sxs-lookup"><span data-stu-id="d2582-103">keyValue resource type</span></span>

> <span data-ttu-id="d2582-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d2582-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2582-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d2582-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2582-106">Definição de valor de chave.</span><span class="sxs-lookup"><span data-stu-id="d2582-106">Key Value definition.</span></span>

## <a name="properties"></a><span data-ttu-id="d2582-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d2582-107">Properties</span></span>
|<span data-ttu-id="d2582-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d2582-108">Property</span></span>|<span data-ttu-id="d2582-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="d2582-109">Type</span></span>|<span data-ttu-id="d2582-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2582-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2582-111">key</span><span class="sxs-lookup"><span data-stu-id="d2582-111">key</span></span>|<span data-ttu-id="d2582-112">String</span><span class="sxs-lookup"><span data-stu-id="d2582-112">String</span></span>|<span data-ttu-id="d2582-113">Chave.</span><span class="sxs-lookup"><span data-stu-id="d2582-113">Key.</span></span>|
|<span data-ttu-id="d2582-114">value</span><span class="sxs-lookup"><span data-stu-id="d2582-114">value</span></span>|<span data-ttu-id="d2582-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d2582-115">String</span></span>|<span data-ttu-id="d2582-116">Valor.</span><span class="sxs-lookup"><span data-stu-id="d2582-116">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2582-117">Relações</span><span class="sxs-lookup"><span data-stu-id="d2582-117">Relationships</span></span>
<span data-ttu-id="d2582-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d2582-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d2582-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d2582-119">JSON Representation</span></span>
<span data-ttu-id="d2582-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d2582-120">Here is a JSON representation of the resource.</span></span>
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



