---
title: Tipo de recurso iosHomeScreenFolder
description: Uma pasta que contém as páginas de aplicativos na tela inicial
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 59d4fe30fd274cd1051de50e225f449570de38ed
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43410697"
---
# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="4dd9d-103">Tipo de recurso iosHomeScreenFolder</span><span class="sxs-lookup"><span data-stu-id="4dd9d-103">iosHomeScreenFolder resource type</span></span>

<span data-ttu-id="4dd9d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4dd9d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4dd9d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4dd9d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4dd9d-106">Uma pasta que contém as páginas de aplicativos na tela inicial</span><span class="sxs-lookup"><span data-stu-id="4dd9d-106">A folder containing pages of apps on the Home Screen</span></span>


<span data-ttu-id="4dd9d-107">Herda de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="4dd9d-107">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4dd9d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4dd9d-108">Properties</span></span>
|<span data-ttu-id="4dd9d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4dd9d-109">Property</span></span>|<span data-ttu-id="4dd9d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="4dd9d-110">Type</span></span>|<span data-ttu-id="4dd9d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4dd9d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4dd9d-112">displayName</span><span class="sxs-lookup"><span data-stu-id="4dd9d-112">displayName</span></span>|<span data-ttu-id="4dd9d-113">String</span><span class="sxs-lookup"><span data-stu-id="4dd9d-113">String</span></span>|<span data-ttu-id="4dd9d-114">Nome do aplicativo Herdado de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="4dd9d-114">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="4dd9d-115">páginas</span><span class="sxs-lookup"><span data-stu-id="4dd9d-115">pages</span></span>|<span data-ttu-id="4dd9d-116">Conjunto [iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md)</span><span class="sxs-lookup"><span data-stu-id="4dd9d-116">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="4dd9d-117">Páginas de ícones de layout da tela inicial que devem ser do tipo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4dd9d-117">Pages of Home Screen Layout Icons which must be Application Type.</span></span> <span data-ttu-id="4dd9d-118">Este conjunto pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="4dd9d-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4dd9d-119">Relações</span><span class="sxs-lookup"><span data-stu-id="4dd9d-119">Relationships</span></span>
<span data-ttu-id="4dd9d-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4dd9d-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4dd9d-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4dd9d-121">JSON Representation</span></span>
<span data-ttu-id="4dd9d-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4dd9d-122">Here is a JSON representation of the resource.</span></span>
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







