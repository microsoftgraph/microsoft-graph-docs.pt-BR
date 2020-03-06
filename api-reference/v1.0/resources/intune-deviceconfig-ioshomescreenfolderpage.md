---
title: Tipo de recurso iosHomeScreenFolderPage
description: Uma pasta com os aplicativos na tela inicial
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: dd0fc9b8f8818eb73c75ef46b5c8e88639e38752
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532496"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="21500-103">Tipo de recurso iosHomeScreenFolderPage</span><span class="sxs-lookup"><span data-stu-id="21500-103">iosHomeScreenFolderPage resource type</span></span>

<span data-ttu-id="21500-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21500-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="21500-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="21500-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21500-106">Uma pasta com os aplicativos na tela inicial</span><span class="sxs-lookup"><span data-stu-id="21500-106">A folder containing apps on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="21500-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="21500-107">Properties</span></span>
|<span data-ttu-id="21500-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="21500-108">Property</span></span>|<span data-ttu-id="21500-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="21500-109">Type</span></span>|<span data-ttu-id="21500-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="21500-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21500-111">displayName</span><span class="sxs-lookup"><span data-stu-id="21500-111">displayName</span></span>|<span data-ttu-id="21500-112">String</span><span class="sxs-lookup"><span data-stu-id="21500-112">String</span></span>|<span data-ttu-id="21500-113">Nome da página da pasta</span><span class="sxs-lookup"><span data-stu-id="21500-113">Name of the folder page</span></span>|
|<span data-ttu-id="21500-114">aplicativos</span><span class="sxs-lookup"><span data-stu-id="21500-114">apps</span></span>|<span data-ttu-id="21500-115">Conjunto [iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md)</span><span class="sxs-lookup"><span data-stu-id="21500-115">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="21500-116">Uma lista de aplicativos exibidos em uma página dentro de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="21500-116">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="21500-117">Este conjunto pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="21500-117">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="21500-118">Relações</span><span class="sxs-lookup"><span data-stu-id="21500-118">Relationships</span></span>
<span data-ttu-id="21500-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="21500-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="21500-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="21500-120">JSON Representation</span></span>
<span data-ttu-id="21500-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="21500-121">Here is a JSON representation of the resource.</span></span>
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
      "bundleID": "String"
    }
  ]
}
```




