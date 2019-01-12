---
title: Tipo de recurso iosHomeScreenFolder
description: Uma pasta que contém as páginas de aplicativos na tela inicial
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: dd47562660f2941fbf722f92976817f310ff304f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930415"
---
# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="94c2b-103">Tipo de recurso iosHomeScreenFolder</span><span class="sxs-lookup"><span data-stu-id="94c2b-103">iosHomeScreenFolder resource type</span></span>

> <span data-ttu-id="94c2b-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="94c2b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="94c2b-105">Uma pasta que contém as páginas de aplicativos na tela inicial</span><span class="sxs-lookup"><span data-stu-id="94c2b-105">A folder containing pages of apps on the Home Screen</span></span>

<span data-ttu-id="94c2b-106">Herda de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="94c2b-106">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="94c2b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="94c2b-107">Properties</span></span>
|<span data-ttu-id="94c2b-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="94c2b-108">Property</span></span>|<span data-ttu-id="94c2b-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="94c2b-109">Type</span></span>|<span data-ttu-id="94c2b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="94c2b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94c2b-111">displayName</span><span class="sxs-lookup"><span data-stu-id="94c2b-111">displayName</span></span>|<span data-ttu-id="94c2b-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="94c2b-112">String</span></span>|<span data-ttu-id="94c2b-113">Nome do aplicativo Herdado de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="94c2b-113">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="94c2b-114">páginas</span><span class="sxs-lookup"><span data-stu-id="94c2b-114">pages</span></span>|<span data-ttu-id="94c2b-115">Conjunto [iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md)</span><span class="sxs-lookup"><span data-stu-id="94c2b-115">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="94c2b-116">Páginas de ícones de layout da tela inicial que devem ser do tipo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="94c2b-116">Pages of Home Screen Layout Icons which must be Application Type.</span></span> <span data-ttu-id="94c2b-117">Este conjunto pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="94c2b-117">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="94c2b-118">Relações</span><span class="sxs-lookup"><span data-stu-id="94c2b-118">Relationships</span></span>
<span data-ttu-id="94c2b-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="94c2b-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="94c2b-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="94c2b-120">JSON Representation</span></span>
<span data-ttu-id="94c2b-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="94c2b-121">Here is a JSON representation of the resource.</span></span>
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



