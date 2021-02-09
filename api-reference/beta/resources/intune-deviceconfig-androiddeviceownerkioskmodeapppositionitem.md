---
title: Tipo de recurso androidDeviceOwnerKioskModeAppPositionItem
description: Um item na lista de posições do aplicativo que define a ordem dos itens na tela inicial gerenciada
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 788b7ac612fd025bb778c387be2051769de66ccb
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160076"
---
# <a name="androiddeviceownerkioskmodeapppositionitem-resource-type"></a><span data-ttu-id="ead65-103">Tipo de recurso androidDeviceOwnerKioskModeAppPositionItem</span><span class="sxs-lookup"><span data-stu-id="ead65-103">androidDeviceOwnerKioskModeAppPositionItem resource type</span></span>

<span data-ttu-id="ead65-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ead65-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ead65-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ead65-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ead65-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ead65-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ead65-107">Um item na lista de posições do aplicativo que define a ordem dos itens na tela inicial gerenciada</span><span class="sxs-lookup"><span data-stu-id="ead65-107">An item in the list of app positions that sets the order of items on the Managed Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="ead65-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ead65-108">Properties</span></span>
|<span data-ttu-id="ead65-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ead65-109">Property</span></span>|<span data-ttu-id="ead65-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ead65-110">Type</span></span>|<span data-ttu-id="ead65-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ead65-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ead65-112">position</span><span class="sxs-lookup"><span data-stu-id="ead65-112">position</span></span>|<span data-ttu-id="ead65-113">Int32</span><span class="sxs-lookup"><span data-stu-id="ead65-113">Int32</span></span>|<span data-ttu-id="ead65-114">Posição do item na grade.</span><span class="sxs-lookup"><span data-stu-id="ead65-114">Position of the item on the grid.</span></span> <span data-ttu-id="ead65-115">Valores válidos de 0 a 9999999</span><span class="sxs-lookup"><span data-stu-id="ead65-115">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="ead65-116">item</span><span class="sxs-lookup"><span data-stu-id="ead65-116">item</span></span>|[<span data-ttu-id="ead65-117">androidDeviceOwnerKioskModeHomeScreenItem</span><span class="sxs-lookup"><span data-stu-id="ead65-117">androidDeviceOwnerKioskModeHomeScreenItem</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskmodehomescreenitem.md)|<span data-ttu-id="ead65-118">Item a ser organizado</span><span class="sxs-lookup"><span data-stu-id="ead65-118">Item to be arranged</span></span>|

## <a name="relationships"></a><span data-ttu-id="ead65-119">Relações</span><span class="sxs-lookup"><span data-stu-id="ead65-119">Relationships</span></span>
<span data-ttu-id="ead65-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ead65-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ead65-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ead65-121">JSON Representation</span></span>
<span data-ttu-id="ead65-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ead65-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeAppPositionItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerKioskModeAppPositionItem",
  "position": 1024,
  "item": {
    "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeWeblink",
    "label": "String",
    "link": "String"
  }
}
```




