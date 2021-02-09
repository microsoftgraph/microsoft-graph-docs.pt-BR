---
title: Tipo de recurso iosHomeScreenFolder
description: Uma pasta que contém páginas de aplicativos e clipes da Web na tela inicial.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7ad090d7e5a01eaf3dda10c6d9edd5cfafacb1a2
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161814"
---
# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="23f05-103">Tipo de recurso iosHomeScreenFolder</span><span class="sxs-lookup"><span data-stu-id="23f05-103">iosHomeScreenFolder resource type</span></span>

<span data-ttu-id="23f05-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23f05-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="23f05-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="23f05-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="23f05-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="23f05-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23f05-107">Uma pasta que contém páginas de aplicativos e clipes da Web na tela inicial.</span><span class="sxs-lookup"><span data-stu-id="23f05-107">A folder containing pages of apps and web clips on the Home Screen.</span></span>


<span data-ttu-id="23f05-108">Herda de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="23f05-108">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="23f05-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="23f05-109">Properties</span></span>
|<span data-ttu-id="23f05-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="23f05-110">Property</span></span>|<span data-ttu-id="23f05-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="23f05-111">Type</span></span>|<span data-ttu-id="23f05-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="23f05-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23f05-113">displayName</span><span class="sxs-lookup"><span data-stu-id="23f05-113">displayName</span></span>|<span data-ttu-id="23f05-114">String</span><span class="sxs-lookup"><span data-stu-id="23f05-114">String</span></span>|<span data-ttu-id="23f05-115">Nome do aplicativo Herdado de [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="23f05-115">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="23f05-116">páginas</span><span class="sxs-lookup"><span data-stu-id="23f05-116">pages</span></span>|<span data-ttu-id="23f05-117">Conjunto [iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md)</span><span class="sxs-lookup"><span data-stu-id="23f05-117">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="23f05-118">Páginas de Ícones de Layout de Tela Inicial que devem ser aplicativos ou clipes da Web.</span><span class="sxs-lookup"><span data-stu-id="23f05-118">Pages of Home Screen Layout Icons which must be applications or web clips.</span></span> <span data-ttu-id="23f05-119">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="23f05-119">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="23f05-120">Relações</span><span class="sxs-lookup"><span data-stu-id="23f05-120">Relationships</span></span>
<span data-ttu-id="23f05-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="23f05-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="23f05-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="23f05-122">JSON Representation</span></span>
<span data-ttu-id="23f05-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="23f05-123">Here is a JSON representation of the resource.</span></span>
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
          "bundleID": "String",
          "isWebClip": true
        }
      ]
    }
  ]
}
```




