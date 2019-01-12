---
title: Tipo de recurso iosHomeScreenFolder
description: Uma pasta que contém as páginas de aplicativos na tela inicial
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 97d159b09d8484a88db46ec6d25fa9996127b484
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937947"
---
# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="64225-103">Tipo de recurso iosHomeScreenFolder</span><span class="sxs-lookup"><span data-stu-id="64225-103">iosHomeScreenFolder resource type</span></span>

> <span data-ttu-id="64225-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="64225-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="64225-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="64225-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="64225-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="64225-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="64225-107">Uma pasta que contém as páginas de aplicativos na tela inicial</span><span class="sxs-lookup"><span data-stu-id="64225-107">A folder containing pages of apps on the Home Screen</span></span>

<span data-ttu-id="64225-108">Herda de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="64225-108">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="64225-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="64225-109">Properties</span></span>
|<span data-ttu-id="64225-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="64225-110">Property</span></span>|<span data-ttu-id="64225-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="64225-111">Type</span></span>|<span data-ttu-id="64225-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="64225-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64225-113">displayName</span><span class="sxs-lookup"><span data-stu-id="64225-113">displayName</span></span>|<span data-ttu-id="64225-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="64225-114">String</span></span>|<span data-ttu-id="64225-115">Nome do aplicativo Herdado de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="64225-115">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="64225-116">páginas</span><span class="sxs-lookup"><span data-stu-id="64225-116">pages</span></span>|<span data-ttu-id="64225-117">Conjunto [iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md)</span><span class="sxs-lookup"><span data-stu-id="64225-117">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="64225-118">Páginas de ícones de layout da tela inicial que devem ser do tipo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="64225-118">Pages of Home Screen Layout Icons which must be Application Type.</span></span> <span data-ttu-id="64225-119">Este conjunto pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="64225-119">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="64225-120">Relações</span><span class="sxs-lookup"><span data-stu-id="64225-120">Relationships</span></span>
<span data-ttu-id="64225-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="64225-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="64225-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="64225-122">JSON Representation</span></span>
<span data-ttu-id="64225-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="64225-123">Here is a JSON representation of the resource.</span></span>
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





