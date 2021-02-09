---
title: Tipo de recurso androidDeviceOwnerKioskModeApp
description: Um aplicativo na tela inicial gerenciada do proprietário do dispositivo Android
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: da6adb416c8fd20406c295e56a5d15177e625c30
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160305"
---
# <a name="androiddeviceownerkioskmodeapp-resource-type"></a><span data-ttu-id="6ea4a-103">Tipo de recurso androidDeviceOwnerKioskModeApp</span><span class="sxs-lookup"><span data-stu-id="6ea4a-103">androidDeviceOwnerKioskModeApp resource type</span></span>

<span data-ttu-id="6ea4a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ea4a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6ea4a-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6ea4a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ea4a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6ea4a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ea4a-107">Um aplicativo na tela inicial gerenciada do proprietário do dispositivo Android</span><span class="sxs-lookup"><span data-stu-id="6ea4a-107">An application on the Android Device Owner Managed Home Screen</span></span>


<span data-ttu-id="6ea4a-108">Herda de [androidDeviceOwnerKioskModeFolderItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodefolderitem.md)</span><span class="sxs-lookup"><span data-stu-id="6ea4a-108">Inherits from [androidDeviceOwnerKioskModeFolderItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodefolderitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6ea4a-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6ea4a-109">Properties</span></span>
|<span data-ttu-id="6ea4a-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6ea4a-110">Property</span></span>|<span data-ttu-id="6ea4a-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="6ea4a-111">Type</span></span>|<span data-ttu-id="6ea4a-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ea4a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ea4a-113">pacote</span><span class="sxs-lookup"><span data-stu-id="6ea4a-113">package</span></span>|<span data-ttu-id="6ea4a-114">String</span><span class="sxs-lookup"><span data-stu-id="6ea4a-114">String</span></span>|<span data-ttu-id="6ea4a-115">Nome do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="6ea4a-115">Package name of application</span></span>|
|<span data-ttu-id="6ea4a-116">className</span><span class="sxs-lookup"><span data-stu-id="6ea4a-116">className</span></span>|<span data-ttu-id="6ea4a-117">String</span><span class="sxs-lookup"><span data-stu-id="6ea4a-117">String</span></span>|<span data-ttu-id="6ea4a-118">Nome da classe do aplicativo</span><span class="sxs-lookup"><span data-stu-id="6ea4a-118">Class name of application</span></span>|

## <a name="relationships"></a><span data-ttu-id="6ea4a-119">Relações</span><span class="sxs-lookup"><span data-stu-id="6ea4a-119">Relationships</span></span>
<span data-ttu-id="6ea4a-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6ea4a-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6ea4a-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6ea4a-121">JSON Representation</span></span>
<span data-ttu-id="6ea4a-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6ea4a-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerKioskModeApp",
  "package": "String",
  "className": "String"
}
```




