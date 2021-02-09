---
title: Tipo de recurso androidDeviceOwnerKioskModeManagedFolderReference
description: Uma referência à pasta que contém aplicativos e weblinks na tela inicial gerenciada
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f454abc8edb54e1ee2ed2e9a6984e8e9e39e29d2
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162201"
---
# <a name="androiddeviceownerkioskmodemanagedfolderreference-resource-type"></a><span data-ttu-id="6e095-103">Tipo de recurso androidDeviceOwnerKioskModeManagedFolderReference</span><span class="sxs-lookup"><span data-stu-id="6e095-103">androidDeviceOwnerKioskModeManagedFolderReference resource type</span></span>

<span data-ttu-id="6e095-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e095-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6e095-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6e095-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6e095-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6e095-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e095-107">Uma referência à pasta que contém aplicativos e weblinks na tela inicial gerenciada</span><span class="sxs-lookup"><span data-stu-id="6e095-107">A reference to folder containing apps and weblinks on the Managed Home Screen</span></span>


<span data-ttu-id="6e095-108">Herda de [androidDeviceOwnerKioskModeHomeScreenItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodehomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="6e095-108">Inherits from [androidDeviceOwnerKioskModeHomeScreenItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodehomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6e095-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6e095-109">Properties</span></span>
|<span data-ttu-id="6e095-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6e095-110">Property</span></span>|<span data-ttu-id="6e095-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="6e095-111">Type</span></span>|<span data-ttu-id="6e095-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e095-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e095-113">folderName</span><span class="sxs-lookup"><span data-stu-id="6e095-113">folderName</span></span>|<span data-ttu-id="6e095-114">String</span><span class="sxs-lookup"><span data-stu-id="6e095-114">String</span></span>|<span data-ttu-id="6e095-115">Nome da pasta</span><span class="sxs-lookup"><span data-stu-id="6e095-115">Name of the folder</span></span>|
|<span data-ttu-id="6e095-116">folderIdentifier</span><span class="sxs-lookup"><span data-stu-id="6e095-116">folderIdentifier</span></span>|<span data-ttu-id="6e095-117">String</span><span class="sxs-lookup"><span data-stu-id="6e095-117">String</span></span>|<span data-ttu-id="6e095-118">Identificador exclusivo da pasta</span><span class="sxs-lookup"><span data-stu-id="6e095-118">Unique identifier for the folder</span></span>|

## <a name="relationships"></a><span data-ttu-id="6e095-119">Relações</span><span class="sxs-lookup"><span data-stu-id="6e095-119">Relationships</span></span>
<span data-ttu-id="6e095-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6e095-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6e095-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6e095-121">JSON Representation</span></span>
<span data-ttu-id="6e095-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6e095-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeManagedFolderReference"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerKioskModeManagedFolderReference",
  "folderName": "String",
  "folderIdentifier": "String"
}
```




