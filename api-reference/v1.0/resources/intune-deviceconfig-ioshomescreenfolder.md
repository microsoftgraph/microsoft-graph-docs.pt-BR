---
title: Tipo de recurso iosHomeScreenFolder
description: Uma pasta que contém as páginas de aplicativos na tela inicial
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a44800da46d771251a47df676af84ceb778cbbd6
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30257684"
---
# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="1370a-103">Tipo de recurso iosHomeScreenFolder</span><span class="sxs-lookup"><span data-stu-id="1370a-103">iosHomeScreenFolder resource type</span></span>

> <span data-ttu-id="1370a-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1370a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1370a-105">Uma pasta que contém as páginas de aplicativos na tela inicial</span><span class="sxs-lookup"><span data-stu-id="1370a-105">A folder containing pages of apps on the Home Screen</span></span>


<span data-ttu-id="1370a-106">Herda de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="1370a-106">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1370a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1370a-107">Properties</span></span>
|<span data-ttu-id="1370a-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1370a-108">Property</span></span>|<span data-ttu-id="1370a-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="1370a-109">Type</span></span>|<span data-ttu-id="1370a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1370a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1370a-111">displayName</span><span class="sxs-lookup"><span data-stu-id="1370a-111">displayName</span></span>|<span data-ttu-id="1370a-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1370a-112">String</span></span>|<span data-ttu-id="1370a-113">Nome do aplicativo Herdado de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="1370a-113">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="1370a-114">páginas</span><span class="sxs-lookup"><span data-stu-id="1370a-114">pages</span></span>|<span data-ttu-id="1370a-115">Conjunto [iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md)</span><span class="sxs-lookup"><span data-stu-id="1370a-115">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="1370a-116">Páginas de ícones de layout da tela inicial que devem ser do tipo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1370a-116">Pages of Home Screen Layout Icons which must be Application Type.</span></span> <span data-ttu-id="1370a-117">Este conjunto pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="1370a-117">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1370a-118">Relações</span><span class="sxs-lookup"><span data-stu-id="1370a-118">Relationships</span></span>
<span data-ttu-id="1370a-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1370a-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1370a-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1370a-120">JSON Representation</span></span>
<span data-ttu-id="1370a-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1370a-121">Here is a JSON representation of the resource.</span></span>
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



