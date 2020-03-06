---
title: Tipo de recurso iosHomeScreenFolder
description: Uma pasta que contém as páginas de aplicativos na tela inicial
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f06d15dce4ce765111ba02a200b59576a614828e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530674"
---
# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="c434c-103">Tipo de recurso iosHomeScreenFolder</span><span class="sxs-lookup"><span data-stu-id="c434c-103">iosHomeScreenFolder resource type</span></span>

<span data-ttu-id="c434c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c434c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c434c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c434c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c434c-106">Uma pasta que contém as páginas de aplicativos na tela inicial</span><span class="sxs-lookup"><span data-stu-id="c434c-106">A folder containing pages of apps on the Home Screen</span></span>


<span data-ttu-id="c434c-107">Herda de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="c434c-107">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c434c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c434c-108">Properties</span></span>
|<span data-ttu-id="c434c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c434c-109">Property</span></span>|<span data-ttu-id="c434c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c434c-110">Type</span></span>|<span data-ttu-id="c434c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c434c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c434c-112">displayName</span><span class="sxs-lookup"><span data-stu-id="c434c-112">displayName</span></span>|<span data-ttu-id="c434c-113">String</span><span class="sxs-lookup"><span data-stu-id="c434c-113">String</span></span>|<span data-ttu-id="c434c-114">Nome do aplicativo Herdado de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="c434c-114">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="c434c-115">páginas</span><span class="sxs-lookup"><span data-stu-id="c434c-115">pages</span></span>|<span data-ttu-id="c434c-116">Conjunto [iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md)</span><span class="sxs-lookup"><span data-stu-id="c434c-116">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="c434c-117">Páginas de ícones de layout da tela inicial que devem ser do tipo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c434c-117">Pages of Home Screen Layout Icons which must be Application Type.</span></span> <span data-ttu-id="c434c-118">Este conjunto pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="c434c-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c434c-119">Relações</span><span class="sxs-lookup"><span data-stu-id="c434c-119">Relationships</span></span>
<span data-ttu-id="c434c-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c434c-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c434c-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c434c-121">JSON Representation</span></span>
<span data-ttu-id="c434c-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c434c-122">Here is a JSON representation of the resource.</span></span>
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




