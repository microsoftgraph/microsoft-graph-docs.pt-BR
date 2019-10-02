---
title: Tipo de recurso iosHomeScreenFolderPage
description: Uma pasta com os aplicativos na tela inicial
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b80a4f41583617d32e514e29c791e000315593c5
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359100"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="ccf5d-103">Tipo de recurso iosHomeScreenFolderPage</span><span class="sxs-lookup"><span data-stu-id="ccf5d-103">iosHomeScreenFolderPage resource type</span></span>

> <span data-ttu-id="ccf5d-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ccf5d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ccf5d-105">Uma pasta com os aplicativos na tela inicial</span><span class="sxs-lookup"><span data-stu-id="ccf5d-105">A folder containing apps on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="ccf5d-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ccf5d-106">Properties</span></span>
|<span data-ttu-id="ccf5d-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ccf5d-107">Property</span></span>|<span data-ttu-id="ccf5d-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="ccf5d-108">Type</span></span>|<span data-ttu-id="ccf5d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ccf5d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ccf5d-110">displayName</span><span class="sxs-lookup"><span data-stu-id="ccf5d-110">displayName</span></span>|<span data-ttu-id="ccf5d-111">String</span><span class="sxs-lookup"><span data-stu-id="ccf5d-111">String</span></span>|<span data-ttu-id="ccf5d-112">Nome da página da pasta</span><span class="sxs-lookup"><span data-stu-id="ccf5d-112">Name of the folder page</span></span>|
|<span data-ttu-id="ccf5d-113">aplicativos</span><span class="sxs-lookup"><span data-stu-id="ccf5d-113">apps</span></span>|<span data-ttu-id="ccf5d-114">Conjunto [iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md)</span><span class="sxs-lookup"><span data-stu-id="ccf5d-114">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="ccf5d-115">Uma lista de aplicativos exibidos em uma página dentro de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="ccf5d-115">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="ccf5d-116">Este conjunto pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="ccf5d-116">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ccf5d-117">Relações</span><span class="sxs-lookup"><span data-stu-id="ccf5d-117">Relationships</span></span>
<span data-ttu-id="ccf5d-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ccf5d-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ccf5d-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ccf5d-119">JSON Representation</span></span>
<span data-ttu-id="ccf5d-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ccf5d-120">Here is a JSON representation of the resource.</span></span>
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




