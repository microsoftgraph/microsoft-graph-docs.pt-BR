---
title: Tipo de recurso androidDeviceOwnerKioskModeWeblink
description: Um weblink na tela inicial gerenciada do proprietário do dispositivo Android
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 076e1fc6630856ff937bf85396c70e4461fda2b1
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162200"
---
# <a name="androiddeviceownerkioskmodeweblink-resource-type"></a><span data-ttu-id="d23ed-103">Tipo de recurso androidDeviceOwnerKioskModeWeblink</span><span class="sxs-lookup"><span data-stu-id="d23ed-103">androidDeviceOwnerKioskModeWeblink resource type</span></span>

<span data-ttu-id="d23ed-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d23ed-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d23ed-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d23ed-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d23ed-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d23ed-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d23ed-107">Um weblink na tela inicial gerenciada do proprietário do dispositivo Android</span><span class="sxs-lookup"><span data-stu-id="d23ed-107">A weblink on the Android Device Owner Managed Home Screen</span></span>


<span data-ttu-id="d23ed-108">Herda de [androidDeviceOwnerKioskModeFolderItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodefolderitem.md)</span><span class="sxs-lookup"><span data-stu-id="d23ed-108">Inherits from [androidDeviceOwnerKioskModeFolderItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodefolderitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d23ed-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d23ed-109">Properties</span></span>
|<span data-ttu-id="d23ed-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d23ed-110">Property</span></span>|<span data-ttu-id="d23ed-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="d23ed-111">Type</span></span>|<span data-ttu-id="d23ed-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="d23ed-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d23ed-113">rótulo</span><span class="sxs-lookup"><span data-stu-id="d23ed-113">label</span></span>|<span data-ttu-id="d23ed-114">String</span><span class="sxs-lookup"><span data-stu-id="d23ed-114">String</span></span>|<span data-ttu-id="d23ed-115">Nome para exibição do weblink</span><span class="sxs-lookup"><span data-stu-id="d23ed-115">Display name for weblink</span></span>|
|<span data-ttu-id="d23ed-116">vínculo</span><span class="sxs-lookup"><span data-stu-id="d23ed-116">link</span></span>|<span data-ttu-id="d23ed-117">String</span><span class="sxs-lookup"><span data-stu-id="d23ed-117">String</span></span>|<span data-ttu-id="d23ed-118">Link para weblink</span><span class="sxs-lookup"><span data-stu-id="d23ed-118">Link for weblink</span></span>|

## <a name="relationships"></a><span data-ttu-id="d23ed-119">Relações</span><span class="sxs-lookup"><span data-stu-id="d23ed-119">Relationships</span></span>
<span data-ttu-id="d23ed-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d23ed-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d23ed-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d23ed-121">JSON Representation</span></span>
<span data-ttu-id="d23ed-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d23ed-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeWeblink"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerKioskModeWeblink",
  "label": "String",
  "link": "String"
}
```




