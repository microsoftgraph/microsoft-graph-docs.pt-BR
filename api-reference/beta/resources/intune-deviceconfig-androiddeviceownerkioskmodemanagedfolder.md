---
title: Tipo de recurso androidDeviceOwnerKioskModeManagedFolder
description: Uma pasta que contém páginas de aplicativos e weblinks na tela inicial gerenciada
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d4e6b373729ffebb3fc7a08ee29e98f3471c8c27
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162202"
---
# <a name="androiddeviceownerkioskmodemanagedfolder-resource-type"></a><span data-ttu-id="1d565-103">Tipo de recurso androidDeviceOwnerKioskModeManagedFolder</span><span class="sxs-lookup"><span data-stu-id="1d565-103">androidDeviceOwnerKioskModeManagedFolder resource type</span></span>

<span data-ttu-id="1d565-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d565-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1d565-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1d565-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1d565-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1d565-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d565-107">Uma pasta que contém páginas de aplicativos e weblinks na tela inicial gerenciada</span><span class="sxs-lookup"><span data-stu-id="1d565-107">A folder containing pages of apps and weblinks on the Managed Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="1d565-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1d565-108">Properties</span></span>
|<span data-ttu-id="1d565-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1d565-109">Property</span></span>|<span data-ttu-id="1d565-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1d565-110">Type</span></span>|<span data-ttu-id="1d565-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d565-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d565-112">folderName</span><span class="sxs-lookup"><span data-stu-id="1d565-112">folderName</span></span>|<span data-ttu-id="1d565-113">String</span><span class="sxs-lookup"><span data-stu-id="1d565-113">String</span></span>|<span data-ttu-id="1d565-114">Nome de exibição da pasta</span><span class="sxs-lookup"><span data-stu-id="1d565-114">Display name for the folder</span></span>|
|<span data-ttu-id="1d565-115">folderIdentifier</span><span class="sxs-lookup"><span data-stu-id="1d565-115">folderIdentifier</span></span>|<span data-ttu-id="1d565-116">String</span><span class="sxs-lookup"><span data-stu-id="1d565-116">String</span></span>|<span data-ttu-id="1d565-117">Identificador exclusivo da pasta</span><span class="sxs-lookup"><span data-stu-id="1d565-117">Unique identifier for the folder</span></span>|
|<span data-ttu-id="1d565-118">items</span><span class="sxs-lookup"><span data-stu-id="1d565-118">items</span></span>|<span data-ttu-id="1d565-119">[Coleção androidDeviceOwnerKioskModeFolderItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodefolderitem.md)</span><span class="sxs-lookup"><span data-stu-id="1d565-119">[androidDeviceOwnerKioskModeFolderItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodefolderitem.md) collection</span></span>|<span data-ttu-id="1d565-120">Itens a serem adicionados à pasta gerenciada.</span><span class="sxs-lookup"><span data-stu-id="1d565-120">Items to be added to managed folder.</span></span> <span data-ttu-id="1d565-121">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="1d565-121">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1d565-122">Relações</span><span class="sxs-lookup"><span data-stu-id="1d565-122">Relationships</span></span>
<span data-ttu-id="1d565-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1d565-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1d565-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1d565-124">JSON Representation</span></span>
<span data-ttu-id="1d565-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1d565-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeManagedFolder"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerKioskModeManagedFolder",
  "folderName": "String",
  "folderIdentifier": "String",
  "items": [
    {
      "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeWeblink",
      "label": "String",
      "link": "String"
    }
  ]
}
```




