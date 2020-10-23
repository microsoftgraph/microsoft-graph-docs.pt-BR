---
title: Tipo de recurso iosHomeScreenFolder
description: Uma pasta que contém as páginas de aplicativos na tela inicial
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 90bacfccf186da983370ae104c5ba7295016b104
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48705789"
---
# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="4406e-103">Tipo de recurso iosHomeScreenFolder</span><span class="sxs-lookup"><span data-stu-id="4406e-103">iosHomeScreenFolder resource type</span></span>

<span data-ttu-id="4406e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4406e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4406e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4406e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4406e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4406e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4406e-107">Uma pasta que contém as páginas de aplicativos na tela inicial</span><span class="sxs-lookup"><span data-stu-id="4406e-107">A folder containing pages of apps on the Home Screen</span></span>


<span data-ttu-id="4406e-108">Herda de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="4406e-108">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4406e-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4406e-109">Properties</span></span>
|<span data-ttu-id="4406e-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4406e-110">Property</span></span>|<span data-ttu-id="4406e-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="4406e-111">Type</span></span>|<span data-ttu-id="4406e-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="4406e-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4406e-113">displayName</span><span class="sxs-lookup"><span data-stu-id="4406e-113">displayName</span></span>|<span data-ttu-id="4406e-114">String</span><span class="sxs-lookup"><span data-stu-id="4406e-114">String</span></span>|<span data-ttu-id="4406e-115">Nome do aplicativo Herdado de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="4406e-115">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="4406e-116">páginas</span><span class="sxs-lookup"><span data-stu-id="4406e-116">pages</span></span>|<span data-ttu-id="4406e-117">Conjunto [iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md)</span><span class="sxs-lookup"><span data-stu-id="4406e-117">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="4406e-118">Páginas de ícones de layout da tela inicial que devem ser do tipo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4406e-118">Pages of Home Screen Layout Icons which must be Application Type.</span></span> <span data-ttu-id="4406e-119">Este conjunto pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="4406e-119">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4406e-120">Relações</span><span class="sxs-lookup"><span data-stu-id="4406e-120">Relationships</span></span>
<span data-ttu-id="4406e-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4406e-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4406e-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4406e-122">JSON Representation</span></span>
<span data-ttu-id="4406e-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4406e-123">Here is a JSON representation of the resource.</span></span>
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





