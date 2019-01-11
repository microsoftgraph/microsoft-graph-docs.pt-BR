---
title: Tipo de recurso iosHomeScreenFolder
description: Uma pasta que contém as páginas de aplicativos na tela inicial
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1a4f7f4180bce05d331fcc116826956f4feed70c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844573"
---
# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="79667-103">Tipo de recurso iosHomeScreenFolder</span><span class="sxs-lookup"><span data-stu-id="79667-103">iosHomeScreenFolder resource type</span></span>

> <span data-ttu-id="79667-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="79667-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="79667-105">Uma pasta que contém as páginas de aplicativos na tela inicial</span><span class="sxs-lookup"><span data-stu-id="79667-105">A folder containing pages of apps on the Home Screen</span></span>

<span data-ttu-id="79667-106">Herda de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="79667-106">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="79667-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="79667-107">Properties</span></span>
|<span data-ttu-id="79667-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="79667-108">Property</span></span>|<span data-ttu-id="79667-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="79667-109">Type</span></span>|<span data-ttu-id="79667-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="79667-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79667-111">displayName</span><span class="sxs-lookup"><span data-stu-id="79667-111">displayName</span></span>|<span data-ttu-id="79667-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="79667-112">String</span></span>|<span data-ttu-id="79667-113">Nome do aplicativo Herdado de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="79667-113">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="79667-114">páginas</span><span class="sxs-lookup"><span data-stu-id="79667-114">pages</span></span>|<span data-ttu-id="79667-115">Conjunto [iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md)</span><span class="sxs-lookup"><span data-stu-id="79667-115">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="79667-116">Páginas de ícones de layout da tela inicial que devem ser do tipo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="79667-116">Pages of Home Screen Layout Icons which must be Application Type.</span></span> <span data-ttu-id="79667-117">Este conjunto pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="79667-117">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="79667-118">Relações</span><span class="sxs-lookup"><span data-stu-id="79667-118">Relationships</span></span>
<span data-ttu-id="79667-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="79667-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="79667-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="79667-120">JSON Representation</span></span>
<span data-ttu-id="79667-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="79667-121">Here is a JSON representation of the resource.</span></span>
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



