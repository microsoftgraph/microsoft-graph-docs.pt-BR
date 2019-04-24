---
title: Tipo de recurso iosHomeScreenFolder
description: Uma pasta que contém as páginas de aplicativos na tela inicial
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9526e51b4fa69f0332922481c53648eb7d574c10
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32521625"
---
# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="8cb21-103">Tipo de recurso iosHomeScreenFolder</span><span class="sxs-lookup"><span data-stu-id="8cb21-103">iosHomeScreenFolder resource type</span></span>

> <span data-ttu-id="8cb21-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8cb21-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8cb21-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8cb21-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8cb21-106">Uma pasta que contém as páginas de aplicativos na tela inicial</span><span class="sxs-lookup"><span data-stu-id="8cb21-106">A folder containing pages of apps on the Home Screen</span></span>


<span data-ttu-id="8cb21-107">Herda de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="8cb21-107">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8cb21-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8cb21-108">Properties</span></span>
|<span data-ttu-id="8cb21-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8cb21-109">Property</span></span>|<span data-ttu-id="8cb21-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="8cb21-110">Type</span></span>|<span data-ttu-id="8cb21-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8cb21-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8cb21-112">displayName</span><span class="sxs-lookup"><span data-stu-id="8cb21-112">displayName</span></span>|<span data-ttu-id="8cb21-113">String</span><span class="sxs-lookup"><span data-stu-id="8cb21-113">String</span></span>|<span data-ttu-id="8cb21-114">Nome do aplicativo Herdado de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="8cb21-114">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="8cb21-115">páginas</span><span class="sxs-lookup"><span data-stu-id="8cb21-115">pages</span></span>|<span data-ttu-id="8cb21-116">Conjunto [iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md)</span><span class="sxs-lookup"><span data-stu-id="8cb21-116">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="8cb21-117">Páginas de ícones de layout da tela inicial que devem ser do tipo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8cb21-117">Pages of Home Screen Layout Icons which must be Application Type.</span></span> <span data-ttu-id="8cb21-118">Este conjunto pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="8cb21-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8cb21-119">Relações</span><span class="sxs-lookup"><span data-stu-id="8cb21-119">Relationships</span></span>
<span data-ttu-id="8cb21-120">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="8cb21-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8cb21-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8cb21-121">JSON Representation</span></span>
<span data-ttu-id="8cb21-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8cb21-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenFolder"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenFolder",
  "displayName": "String",
  "pages": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
      "displayName": "String",
      "apps": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenApp",
          "displayName": "String",
          "bundleID": "String"
        }
      ]
    }
  ]
}
```





