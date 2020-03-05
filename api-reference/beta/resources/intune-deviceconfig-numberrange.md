---
title: tipo de recurso numberRange
description: Definição do intervalo de números.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fee2fe4271b3ce070194a08e2ad7c3022cd42626
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529575"
---
# <a name="numberrange-resource-type"></a><span data-ttu-id="49077-103">tipo de recurso numberRange</span><span class="sxs-lookup"><span data-stu-id="49077-103">numberRange resource type</span></span>

<span data-ttu-id="49077-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="49077-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="49077-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="49077-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49077-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="49077-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49077-107">Definição do intervalo de números.</span><span class="sxs-lookup"><span data-stu-id="49077-107">Number Range definition.</span></span>

## <a name="properties"></a><span data-ttu-id="49077-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="49077-108">Properties</span></span>
|<span data-ttu-id="49077-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="49077-109">Property</span></span>|<span data-ttu-id="49077-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="49077-110">Type</span></span>|<span data-ttu-id="49077-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="49077-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49077-112">lowerNumber</span><span class="sxs-lookup"><span data-stu-id="49077-112">lowerNumber</span></span>|<span data-ttu-id="49077-113">Int32</span><span class="sxs-lookup"><span data-stu-id="49077-113">Int32</span></span>|<span data-ttu-id="49077-114">Número menor.</span><span class="sxs-lookup"><span data-stu-id="49077-114">Lower number.</span></span>|
|<span data-ttu-id="49077-115">upperNumber</span><span class="sxs-lookup"><span data-stu-id="49077-115">upperNumber</span></span>|<span data-ttu-id="49077-116">Int32</span><span class="sxs-lookup"><span data-stu-id="49077-116">Int32</span></span>|<span data-ttu-id="49077-117">Número superior.</span><span class="sxs-lookup"><span data-stu-id="49077-117">Upper number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="49077-118">Relações</span><span class="sxs-lookup"><span data-stu-id="49077-118">Relationships</span></span>
<span data-ttu-id="49077-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="49077-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="49077-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="49077-120">JSON Representation</span></span>
<span data-ttu-id="49077-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="49077-121">Here is a JSON representation of the resource.</span></span>
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



