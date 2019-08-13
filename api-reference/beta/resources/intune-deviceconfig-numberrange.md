---
title: tipo de recurso numberRange
description: Definição do intervalo de números.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2b300f3d0db3a2a310d0a19408750b1dd9ac5c46
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36368545"
---
# <a name="numberrange-resource-type"></a><span data-ttu-id="1f1c0-103">tipo de recurso numberRange</span><span class="sxs-lookup"><span data-stu-id="1f1c0-103">numberRange resource type</span></span>

> <span data-ttu-id="1f1c0-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1f1c0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1f1c0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1f1c0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f1c0-106">Definição do intervalo de números.</span><span class="sxs-lookup"><span data-stu-id="1f1c0-106">Number Range definition.</span></span>

## <a name="properties"></a><span data-ttu-id="1f1c0-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1f1c0-107">Properties</span></span>
|<span data-ttu-id="1f1c0-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1f1c0-108">Property</span></span>|<span data-ttu-id="1f1c0-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="1f1c0-109">Type</span></span>|<span data-ttu-id="1f1c0-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f1c0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f1c0-111">lowerNumber</span><span class="sxs-lookup"><span data-stu-id="1f1c0-111">lowerNumber</span></span>|<span data-ttu-id="1f1c0-112">Int32</span><span class="sxs-lookup"><span data-stu-id="1f1c0-112">Int32</span></span>|<span data-ttu-id="1f1c0-113">Número menor.</span><span class="sxs-lookup"><span data-stu-id="1f1c0-113">Lower number.</span></span>|
|<span data-ttu-id="1f1c0-114">upperNumber</span><span class="sxs-lookup"><span data-stu-id="1f1c0-114">upperNumber</span></span>|<span data-ttu-id="1f1c0-115">Int32</span><span class="sxs-lookup"><span data-stu-id="1f1c0-115">Int32</span></span>|<span data-ttu-id="1f1c0-116">Número superior.</span><span class="sxs-lookup"><span data-stu-id="1f1c0-116">Upper number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1f1c0-117">Relações</span><span class="sxs-lookup"><span data-stu-id="1f1c0-117">Relationships</span></span>
<span data-ttu-id="1f1c0-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1f1c0-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1f1c0-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1f1c0-119">JSON Representation</span></span>
<span data-ttu-id="1f1c0-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1f1c0-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.numberRange"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.numberRange",
  "lowerNumber": 1024,
  "upperNumber": 1024
}
```



