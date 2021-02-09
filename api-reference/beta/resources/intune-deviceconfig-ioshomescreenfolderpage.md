---
title: Tipo de recurso iosHomeScreenFolderPage
description: Uma página para uma pasta que contém aplicativos e clipes da Web na tela inicial.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 45a26205e6a4f03639984e2a72632bb8bfb5a332
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161807"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="bb409-103">Tipo de recurso iosHomeScreenFolderPage</span><span class="sxs-lookup"><span data-stu-id="bb409-103">iosHomeScreenFolderPage resource type</span></span>

<span data-ttu-id="bb409-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb409-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bb409-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bb409-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb409-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bb409-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb409-107">Uma página para uma pasta que contém aplicativos e clipes da Web na tela inicial.</span><span class="sxs-lookup"><span data-stu-id="bb409-107">A page for a folder containing apps and web clips on the Home Screen.</span></span>

## <a name="properties"></a><span data-ttu-id="bb409-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bb409-108">Properties</span></span>
|<span data-ttu-id="bb409-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bb409-109">Property</span></span>|<span data-ttu-id="bb409-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb409-110">Type</span></span>|<span data-ttu-id="bb409-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb409-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb409-112">displayName</span><span class="sxs-lookup"><span data-stu-id="bb409-112">displayName</span></span>|<span data-ttu-id="bb409-113">String</span><span class="sxs-lookup"><span data-stu-id="bb409-113">String</span></span>|<span data-ttu-id="bb409-114">Nome da página da pasta</span><span class="sxs-lookup"><span data-stu-id="bb409-114">Name of the folder page</span></span>|
|<span data-ttu-id="bb409-115">aplicativos</span><span class="sxs-lookup"><span data-stu-id="bb409-115">apps</span></span>|<span data-ttu-id="bb409-116">Conjunto [iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md)</span><span class="sxs-lookup"><span data-stu-id="bb409-116">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="bb409-117">Uma lista de aplicativos e clipes da Web para aparecer em uma página dentro de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="bb409-117">A list of apps and web clips to appear on a page within a folder.</span></span> <span data-ttu-id="bb409-118">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="bb409-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb409-119">Relações</span><span class="sxs-lookup"><span data-stu-id="bb409-119">Relationships</span></span>
<span data-ttu-id="bb409-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bb409-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bb409-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bb409-121">JSON Representation</span></span>
<span data-ttu-id="bb409-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bb409-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenFolderPage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenFolderPage",
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
```




